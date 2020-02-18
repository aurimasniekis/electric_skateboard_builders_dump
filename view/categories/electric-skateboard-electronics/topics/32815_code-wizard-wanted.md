# Code Wizard wanted!

### Replies: 11 Views: 630

## \#1 Posted by: MysticalDork Posted at: 2017-09-10T20:31:57.218Z Reads: 138

```
I have a small project in mind to improve the headlight on my skateboard, requiring a little bit of arduino code, and I suck at coding. I wonder if anyone in the forum that is competent with the C programming language would be willing to assist me with my project's source code.

The project is simple: I have a LED driver in my board that runs the front headlight, but it's **WAY** too bright right now for normal street use. The LED driver I'm using can do dimming using a PWM signal.

I have a spare channel on my GT2B receiver, which outputs a PWM signal. 

Unfortunately, the PWM signal required by the LED driver is different than the receiver produces, so the project is to make a "translator" board, to convert the 1-2ms@50hz PWM from the receiver into the 1-99%@1khz PWM the driver needs. 

I plan to use an attiny85 or similar 8-pin low-power microcontroller.

The general idea is to set an interrupt on the input pin, and start counting when it goes high, then once it goes low, calculate the value corresponding to the time the signal was high, and then output that to another pin as a 1-99% PWM signal at 1khz. It should be a very simple piece of coding, but I can't for the life of me wrap my brain around C.

Any constructive criticism or help would be greatly appreciated.
```

---
## \#2 Posted by: Deckoz Posted at: 2017-09-10T21:52:02.663Z Reads: 116

```
Dude dont do that. 

Here's what I'm doing

Channel 2 mini remote, pinky button is high low ppm. Connect arduino to analog channel, define ppm, if input stream is high set a variable to 1. When its high again set it to 0. Or make as many as you want

Separate method, analog write a pwm value to your dimmer pin, ie if  ppm_high=1  analogwrite 100. Again making as many as you want for example

1=100
2=200
3=255
0=0

Then you can define the brightness by a number of clicks with nothing but the arduino, driver and a signal from the receiver.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-10T22:43:48.381Z Reads: 99

```
I was planning to use channel 3 (steering) because I'm already using channel 2 (button) to turn the driver on and off. my plan was to have a pot on the remote that could be turned to adjust the brightness smoothly. Either that, or a 1p3t switch and some resistors to allow low/med/high beams. 

Either way, I've never succeeded in writing C. Would you mind writing the program? I'd be willing to pay you for your time.
```

---
## \#4 Posted by: Clonkex Posted at: 2017-09-10T22:47:20.021Z Reads: 91

```
I'm sure I could whip something up for you. No need for payment :)
```

---
## \#5 Posted by: Clonkex Posted at: 2017-09-11T00:01:52.760Z Reads: 69

```
Hmm I'm at work and I don't have time to sneakily write you some code until I get home, but you can have this theory to start with :P

So to simplify the goal a bit, you want to do two distinct things: 1) read an RC receiver signal as a range, let's say 0 - 1023, and 2) output a 1KHz PWM signal at a duty cycle of 0 - 100%, mapped from the earlier range.

Reading a receiver signal is pretty easy, but not as easy to do efficiently. You can easily [use pulseIn()](https://www.sparkfun.com/tutorials/348) to read a receiver's signal, but that has the disadvantage of making the code wait until the next signal starts every time, which means you won't be able to generate the PWM output signal (because the code will be spending most of its time waiting). Instead you should [use interrupts](https://ryanboland.com/blog/reading-rc-receiver-values/).

To generate a 1KHz PWM signal, we can't use any automatic solutions without changing the timer frequencies of the Arduino, which messes with the `millis()` and other timer functions. That wouldn't be a problem except that we need the timer functions for writing the PWM signal to the LEDs.

Actually you know what. This doesn't seem that hard. Here, try this code. Plug your receiver channel into pin A0 (and the ground of the receiver into a GND pin on the Arduino obviously - I'm hoping you know the hardware side of this well enough). Plug the LED controller's PWM pin into pin 9 of the Arduino (idk why pin 9, I just picked one at random). Then just try out the code! It's totally untested but I'm hoping it should _just work_. The PWM signal _might_ be too rough; I'm just hoping the Arduino will be fast enough that a C-coded 1KHz PWM signal generator should work fine. This is one of these "suck it and see" situations.

Full disclosure, I didn't write most of this code. I just grabbed the code off the page linked above on the interrupt method and modified it. I wrote the PWM bit myself though. Only the `doPWM()` section and the associated variables are written in my style; everything else is gross and messy-looking :P

    #include <EnableInterrupt.h>

    #define SERIAL_PORT_SPEED 57600
    #define RC_NUM_CHANNELS  1

    #define RC_CH3  0

    #define RC_CH3_INPUT  2

    uint16_t rc_values[RC_NUM_CHANNELS];
    uint32_t rc_start[RC_NUM_CHANNELS];
    volatile uint16_t rc_shared[RC_NUM_CHANNELS];

    int percentage = 0;
    unsigned long lastPwmStart = 0;
    const byte pwmPin = 0;

    void rc_read_values() {
      noInterrupts();
      memcpy(rc_values, (const void *)rc_shared, sizeof(rc_shared));
      interrupts();
    }

    void calc_input(uint8_t channel, uint8_t input_pin) {
      if (digitalRead(input_pin) == HIGH) {
        rc_start[channel] = micros();
      } else {
        uint16_t rc_compare = (uint16_t)(micros() - rc_start[channel]);
        rc_shared[channel] = rc_compare;
      }
    }

    void calc_ch3() { calc_input(RC_CH3, RC_CH3_INPUT); }

    void setup() {
      //Serial.begin(SERIAL_PORT_SPEED);

      pinMode(RC_CH3_INPUT, INPUT);
      pinMode(pwmPin, OUTPUT);

      enableInterrupt(RC_CH3_INPUT, calc_ch3, CHANGE);
    }

    void loop() {
      rc_read_values();
      
      percentage = map(percentage, 1000, 2000, 0, 100); //assume the receiver is outputting exactly in spec between 1000 and 2000; it's probably not but should be close enough
      
      doPWM();

      //Serial.print("CH3:"); Serial.println(rc_values[RC_CH3]);

      //delay(200);
    }

    void doPWM() {
    	//1KHz PWM signal means beginning a new pulse every 1000 microseconds or 1 millisecond
    	//then we just vary the length of the pulse between 0 and 1000 microseconds
    	unsigned long microseconds = micros();
    	if(microseconds - lastPwmStart >= 1000) { //begin new pulse
    		lastPwmStart = microseconds;
    		digitalWrite(pwmPin, HIGH);
    	} else {
    		int targetLength = percentage * 10; //0 - 100 times 10 will be 0 - 1000
    		if(microseconds - lastPwmStart >= targetLength) { //reached the target pulse length, time to turn off the pin
    			digitalWrite(pwmPin, LOW);
    		}
    	}
    }
```

---
## \#6 Posted by: Clonkex Posted at: 2017-09-11T00:14:12.420Z Reads: 54

```
That 4th paragraph was totally screwed up and made no sense. Fixed it ;)
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2017-09-11T02:01:25.279Z Reads: 46

```
i always add some type of a delay "delay(10);" in my programs generally at the end if one is not provided throughout. programs tend to run more stable and if its just switching light brightness, you wont be missing the 10 milliseconds.

and what type of light are you using that you have to "tone it down" ?

nice project
nice code
```

---
## \#8 Posted by: Clonkex Posted at: 2017-09-11T03:04:16.844Z Reads: 43

```
There should be no reason for a program to be unstable running as fast as the CPU can go unless it's coded poorly, or relies on smaller floating point values the faster it goes. That kind of thing. Arduinos also don't generate any noticeable amount of heat (or even any at all in my experience) when running full pelt. The other reason we can't use a delay is that the PWM code has to run as often as possible or it will stop being PWM :P
```

---
## \#9 Posted by: Scoo_B_SK8 Posted at: 2017-09-11T04:12:32.263Z Reads: 40

```
was laying in bed thinking about it...came back to correct myself, but Clonkex already set it straight.  thanks for doing so.
```

---
## \#10 Posted by: dotruongq Posted at: 2017-09-11T05:05:20.425Z Reads: 38

```
I did this project with an ARM mcu, use  channel3 for front headlight. for brake light i used timer to capture 1ms to 2ms, if less than 1.5ms than full pwm, if not throw in low pwm, kinda clunky since i havent invest too much time to it, fun thread to start :)
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-09-11T05:37:58.656Z Reads: 38

```
Thanks guys! @clonkex as soon as I dig up a suitable micro, I'll give it a try, I really appreciate the help. @Scoo_B_SK8 I'm using a Cree XHP50 running at  ~8.5 watts, or about 850 lumens. It's **REALLY** bright, and since it doesn't have a nice horizon cutoff, it tends to blind oncoming traffic. Not that big of a deal for long range high-beams, but I want to not be a dick to other pedestrians and/or vehicles. I'll probably angle it down a little bit as well when I get things back together. 

If I can fit it, I may add a second lower power driver and dimmer setup to run the brake lights that I plan to add at some point, using the throttle signal, just inverted.

This is the datasheet for the LED driver: http://www.xppower.com/Portals/0/pdfs/SF_LDU56.pdf mine is the 700mA version, and I have a 150mA version in reserve for the tail light.
```

---

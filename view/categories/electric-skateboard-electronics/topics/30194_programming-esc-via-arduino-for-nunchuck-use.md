# Programming ESC via Arduino (for nunchuck use)

### Replies: 7 Views: 1288

## \#1 Posted by: TheSupremeLobster Posted at: 2017-08-09T21:02:07.731Z Reads: 88

```
Hi guys!

I'm brand new to RC builds, in fact this long board build will be my first ever! Please excuse me if I say something wrong or doesn't make sense!

Currently I am trying to control my setup via a Nunchuck. I've seen some tutorials out there about how to calibrate the ESC via an arduino, and I have been successful in doing so. However, is there anyway I can customize the controls?

Ideally I would like a setup where the "Z" button is trigger so the motor will only run if the user holds down the "Z" button.

The code I attached only allows control of the motor speed when "Z" is pressed, however, if a user pushes the throttle to a certain point and lets go of "Z" the motor will cruise at that speed. The motor will not stop until the user pushes "Z" AND the throttle is in the neutral position on the nunchuck. 

Looking at the code it makes sense why this happens, but the problem arises when I add the code that is commented out. I figured this would work (which it kinda does) in terms of making the nunchuck function how i want it to, but there seems to be some sort of delay. Basically I have to tap the "Z" button multiple times in order for me to re-accelerate the motor again. 

I hope that makes sense, if not I can try to clarify.

     #include <Servo.h>
    #include <Wire.h>
    #include "nunchuk.h"


    Servo esc;
    int motor;

    void setup() {
      // put your setup code here, to run once:
      esc.attach(9);
      esc.writeMicroseconds(1000);
      Serial.begin(9600);
      nunchuck_setpowerpins();
      nunchuck_init();
      Serial.print("Ready\n");
      

    }

    void loop() {
      // put your main code here, to run repeatedly:


      nunchuck_get_data();                                        //Get data from nunchcuk.

      int joystick_Y = nunchuck_joyy();                           //Variable to store joystick vertical information
      int Button_Z = nunchuck_zbutton();                          //Variable to store "Z" button information
      int Button_C = nunchuck_cbutton();                          //Variable to store "C" button information

      

    if(Button_Z == 1)                                             //Only if the "Z" button is pressesd excute the following code
    {
        Serial.print("Pressed\t");                  
        motor = map(joystick_Y, 122,213,1000,2000);               //map the joystick postion to motor speed
        esc.writeMicroseconds(motor);                             //output information to the motor
        Serial.print("sensor = ");                                //report information to serial monitor
        Serial.print(joystick_Y);
        Serial.print("\t output = ");
        Serial.println(motor);
    }
    //else if (Button_Z == 0)                                   //If the "Z" button IS NOT pressed excute this code
    //{
    //  Serial.print("NOT Pressed\t");
    //    motor = map(joystick_Y, 122,213,1000,2000);
    //    esc.write(0);                                        //send 0 to the motor
    //    Serial.print("sensor = ");
    //    Serial.print(joystick_Y);
    //    Serial.print("\t output = ");
    //    Serial.println(motor);
    //}

      delay(1); 

    }


Could anyone guide me with this? or is there a better way to do this sort of thing?

Any help is appreciated!!

ESC: https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

Best,
-H
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2017-08-10T11:00:17.631Z Reads: 61

```
I can't type a full code right now, but you basically do this:
if (button==1){
esc.writemicroseconds(whateveryourthrottleis)
}
else 
{
esc.writemicroseconds(value you want when no button pressed)
}

So if the button is pressed the value gets sent, if not another fixed value is sent. I have it so that when no button is pressed it goes neutral, no acceleration and no braking.
```

---
## \#3 Posted by: TheSupremeLobster Posted at: 2017-08-11T00:25:03.847Z Reads: 49

```
I see, I tried to do what you recommended, but my ESC wouldn't arm. I'm not really sure why that is though.

Would you know why I am experiencing a delay in the code I wrote?

what happens is that every time I let go of the the "Z" trigger button the motor will stop, but if I wish to re-engage the throttle i need to hold down the "Z" button for at least 4 seconds before  moving the throttle (If I move the throttle before 4 seconds the motor won't start). I don't understand why it wouldn't be instantaneous.

Thanks!!
-H
```

---
## \#4 Posted by: Der6FingerJo Posted at: 2017-08-11T04:16:00.240Z Reads: 47

```
Most hobby ESCs only initialize when the throttle is low for safety reasons. Or maybe you even enter calibration each time you start, assuming your non button pressed value is at 1500ish microseconds
```

---
## \#5 Posted by: TheSupremeLobster Posted at: 2017-08-12T01:19:03.343Z Reads: 45

```
Gotcha, I was actually able to figure out how to arm the ESC and send values to the motor without the nunchuck.

I also tried flipping my nunchuck control. Basically what i did was make it so that now if a user ever pressed Z then the motor would stop. For some reason that seems to work, but doing it the other way does not.

Any thought on why this occurs?

Many Thanks,
-H
```

---
## \#6 Posted by: Waiboard Posted at: 2018-04-07T18:30:55.538Z Reads: 32

```
Hello, I have the same ESC X-car 120a and I would like to know how you did it to program it using Arduino. Could you tell me how to do it?
Thank you!
```

---
## \#7 Posted by: TheSupremeLobster Posted at: 2018-05-15T20:52:30.523Z Reads: 27

```
There should be a female pinout on the ESC that has ground, power and data pins. I believe you only connect the ground and data pin to your arduino. After that it is just about sending the correct data values to the ESC (Unfortunately these can vary with different ESCs so its a trial and error process).

I used this as a guide:
http://www.instructables.com/id/ESC-Programming-on-Arduino-Hobbyking-ESC/

Ultimately i am using a wii nunchuk to control my esc, but you should just be able to control it via code. Hope that helps

-H
```

---

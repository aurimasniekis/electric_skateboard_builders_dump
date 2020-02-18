# Aruino Nano rgb LED Volt indicator

### Replies: 4 Views: 683

## \#1 Posted by: pvcaesbroeck Posted at: 2017-07-31T15:29:24.364Z Reads: 141

```
Hello all,
I managed to make my own eBoard, thanks to all people like you who share their knowledge online. My setup is very simple: 2 x 3s batteries (lipo 11.1V, 35rc, 6000mAh) in series, connected to the vesc. If I understand the theory correctly, this gives me 22.2V and 6000 mAh. This setup gives me a range of 13km (8 miles).

While riding, I would like to see the capacity of the batteries. 
So, with an Arduino Nano, I made a circuit with a rgb LED and programmed it to different colors, depending on the Voltage it reads. Example: when battery is between 100 and 90% the LED is green, between 89 and 70% the LED is blue,...

Now I would like to add this setting (Arduino) to my eBoard, but I really don't know how and where I must connect it. I guess it has to be connected to the VESC?

Can someone help me out with this please?

Tnx
```

---
## \#2 Posted by: Sander Posted at: 2017-07-31T21:19:34.993Z Reads: 119

```
You will need to communicate with the VESC via using UART with the Serial Port of Arduino. 

Here is a good start for you with using Rolling Gecko's library.
https://github.com/RollingGecko/ArduBoardControler

So your highest cell voltage might be 4.2
And the lowest 3.4 so:

So max voltage = 6S*4.2V = 25.2V
And the lowest will be = 6S*3.3V = 20.4V

So the gap between them will be:
25.2V - 20.4V = 4.8.


So for your instance (you need to add the library in the code, I just gave you a little boost):



----------

    #include "VescUart.h"
    #include "datatypes.h"
    #include "local_datatypes.h"

    #define RED        3
    #define YELLOW     4
    #define GREEN      5

    struct bldcMeasure VescMeasuredValues;
    #define SERIALIO Serial

    void setup() {
      SERIALIO.begin(115200);
      while (!SERIALIO);
      
      pinMode(RED, OUTPUT);
      pinMode(YELLOW, OUTPUT);
      pinMode(GREEN, OUTPUT);
    }

    //VESC Voltage:
    float voltage = 0.0;

    //Your max voltage
    float battVMax = 25.2;

    void loop() {
      if (VescUartGetValue(VescMeasuredValues)) {
        voltage = VescMeasuredValues.inpVoltage;
      }
      
      int voltDiff = (float)battVMax - (float)voltage; //Rounding the number from 5 to 0
      switch (voltDiff) {
        case 0: //25V GREEN
          digitalWrite(GREEN, HIGH);
          digitalWrite(YELLOW, LOW);
          digitalWrite(RED, LOW);
          break;
        case 1: //24V GREEN
          digitalWrite(GREEN, HIGH);
          digitalWrite(YELLOW, LOW);
          digitalWrite(RED, LOW);
          break;
        case 2: //23V YELLOW
          digitalWrite(GREEN, LOW);
          digitalWrite(YELLOW, HIGH);
          digitalWrite(RED, LOW);
          break;
        case 3: //22V YELLOW
          digitalWrite(GREEN, LOW);
          digitalWrite(YELLOW, HIGH);
          digitalWrite(RED, LOW);
          break;
        case 4: //21V RED
          digitalWrite(GREEN, LOW);
          digitalWrite(YELLOW, LOW);
          digitalWrite(RED, HIGH);
          break;
        case 5: //20V RED
          digitalWrite(GREEN, LOW);
          digitalWrite(YELLOW, LOW);
          digitalWrite(RED, HIGH);
          break;
      }

    }



----------

Press CTRL+T in the Arduino IDE to autoformat.
CMD+T on mac.
```

---
## \#3 Posted by: pvcaesbroeck Posted at: 2017-08-02T10:38:54.826Z Reads: 58

```
Sander,
THANK you for helping me. 
Sorry, but I must confess that I don’t know anything about electronics and programming.
Could you please indicate what I should connect where, from the VESC to the Arduino?

What I wrote in Ardiono is:
_________

int potPin = A0;

int LEDGroenPin = 7;
int LEDBlauwPin = 5;
int LEDRoodPin = 3;

int LEDlong = 2000;
int LEDshort = 200;

float readValue;
float writeValue;

int LEDGroenMin1 = 800;  //995.37;  100% -> 90%
int LEDGroenMin2 = 600;  //954.75;  89% -> 70%
int LEDBlauwMin1 = 400;  //914.12;  69% -> 50%
int LEDBlauwMin2 = 200;  //873.49;  49% -> 30%
int LEDRoodMin1 = 50 ;   //832.86;  29% -> 10%

void setup() {
 pinMode(potPin, INPUT);
 pinMode(LEDGroenPin, OUTPUT);
 pinMode(LEDBlauwPin, OUTPUT);
 pinMode(LEDRoodPin, OUTPUT);

}

void loop() {
 readValue = analogRead (potPin);

 if (readValue >= LEDGroenMin1) {
   digitalWrite(LEDGroenPin, HIGH);
   delay(LEDlong);
   digitalWrite(LEDGroenPin, LOW);
   delay(LEDlong);
 }
 else  if (readValue >= LEDGroenMin2) {
   digitalWrite(LEDGroenPin, HIGH);
   delay (LEDshort);
   digitalWrite(LEDGroenPin, LOW);
   delay (LEDshort);
 }
 else if (readValue >= LEDBlauwMin1) {
   digitalWrite(LEDBlauwPin, HIGH );
   delay(LEDlong);
   digitalWrite(LEDBlauwPin, LOW);
   delay (LEDlong);
 }
 else if (readValue >= LEDBlauwMin2) {
   digitalWrite(LEDBlauwPin, HIGH);
   delay(LEDshort);
   digitalWrite(LEDBlauwPin, LOW);
   delay(LEDshort);
 }
 else if (readValue >= LEDRoodMin1) {
   digitalWrite(LEDRoodPin, HIGH);
   delay(LEDlong);
   digitalWrite(LEDRoodPin, LOW);
   delay(LEDlong);
 }
 else {
   digitalWrite(LEDRoodPin, HIGH);
   delay(LEDshort);
   digitalWrite(LEDRoodPin, LOW);
   delay(LEDshort);
 }

}

___________

is this useable?

And this is what I have:

<img src="/uploads/db1493/original/3X/c/d/cd299e2883c168f653f7e7f2e9f47bd132cdbcc4.jpg" width="690" height="459"><img src="/uploads/db1493/original/3X/8/8/88edadceb9f3603d02423cc36107c18dae8f0314.png" width="610" height="500">
```

---
## \#4 Posted by: Sander Posted at: 2017-08-02T17:53:36.967Z Reads: 43

```
connect the RX of Arduino the the TX on the VESC, same with the Arduino TX to the RX on the VESC. On the underside of the VESC where the UART is, it stands what is TX and RX.

I believe its like this, 5V, 3.3V, GND, RX, TX, AD2, AD3.
You can use the 5V pin connect it to the VIN in the arduino and the GND to the GND.

But you cant upload the sketch if you are connected with the UART with the power on of the VESC.
```

---

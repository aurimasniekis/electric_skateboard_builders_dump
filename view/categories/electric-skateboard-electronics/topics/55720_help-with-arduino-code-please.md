# Help with arduino code please

### Replies: 9 Views: 496

## \#1 Posted by: jasonlove199450 Posted at: 2018-05-17T02:04:38.816Z Reads: 111

```
I need help with my Arduino code. I'm using a arduino wii nunchuck and home made arduino receiver both using the nrf2401 .I have got it all working fine like I want but I don't really know a lot about Arduino code that's why I'm here. I would like it so when I press the 'C' Button it remembers the 'throttle' anolog input and instead if outputting the anolog input to the esc it instead outputs the last anolog input . so basictally a cruse control . so when i click the c button it stays at the speed the anolog was last at and when i release the c button it goes back to reading the anolog input again . NOTE only remember last anolog IF the anolog value is 127 or higher   (if the value was under 127 the motor would be in reverse and id go backwards) also I have dyslexia so sorry about the poor writing lol . Thanks :D      

If i get help I will post the wiring diagrams and the transmitter code To thank the community.

THE CODE:


#include <SPI.h>
#include <nRF24L01.h>
#include <RF24.h>
#include <Servo.h>  //To create PWM signals we need this lybrary

const uint64_t pipeIn = 0xE8E8F0F0E1LL;     //Remember that this code is the same as in the transmitter
RF24 radio(9, 10);  //CSN and CE pins

// The sizeof this struct should not exceed 32 bytes
struct Received_data {
  byte ch1;              //Throttle
  byte ch2;              //Z
  byte ch3;              //C
  byte ch4;
  byte ch5;
  byte ch6;
  byte ch7;
};

Received_data received_data;

Servo channel_1;    //Throttle
Servo channel_2;    //Z
Servo channel_3;    //C
Servo channel_4;
Servo channel_5;
Servo channel_6;
Servo channel_7;

int ch1_value = 0;     //Throttle
int ch2_value = 0;     //Z
int ch3_value = 0;     //C
int ch4_value = 0;
int ch5_value = 0;
int ch6_value = 0;
int ch7_value = 0;




/**************************************************/

void setup()
{

  //Break lights output
  pinMode(A1, OUTPUT);


//For Testing
//Serial.begin(9600);   //make sure the same is selected in serial monitor!!

  //Attach the servo signal on pins from D2 to D8
  channel_1.attach(2);     //Throttle
  channel_2.attach(3);     //Z
  channel_3.attach(4);     //C
  channel_4.attach(5);
  channel_5.attach(6);
  channel_6.attach(7);
  channel_7.attach(8);
  
  //We reset the received values
  received_data.ch1 = 127;        //Throttle
  received_data.ch2 = 0;            //Z
  received_data.ch3 = 0;            //C
  received_data.ch4 = 0;
  received_data.ch5 = 0;
  received_data.ch6 = 0;
  received_data.ch7 = 0;

  //Once again, begin and radio configuration
  radio.begin();
  radio.setAutoAck(false);
  radio.setDataRate(RF24_250KBPS);  
  radio.openReadingPipe(1,pipeIn);
  
  //We start the radio comunication
  radio.startListening();

}

/**************************************************/

unsigned long last_Time = 0;

//We create the function that will read the data each certain time
void receive_the_data()
{
  while ( radio.available() ) {
  radio.read(&received_data, sizeof(Received_data));
  last_Time = millis(); //Here we receive the data
}
}

/**************************************************/

void loop()
{
  //Receive the radio data
  receive_the_data();

  
  ch1_value = map(received_data.ch1,0,255,1000,2000);           //Throttle
  ch2_value = map(received_data.ch2,0,255,1000,2000);           //Z
  ch3_value = map(received_data.ch3,0,255,1000,2000);           //C
  ch4_value = map(received_data.ch4,0,255,1000,2000);
  ch5_value = map(received_data.ch5,0,1,1000,2000);
  ch6_value = map(received_data.ch6,0,1,1000,2000);
  ch7_value = map(received_data.ch7,0,255,1000,2000);

  //Creathe the PWM signals
  channel_1.writeMicroseconds(ch1_value);              //Throttle
  channel_2.writeMicroseconds(ch2_value);              //Z
  channel_3.writeMicroseconds(ch3_value);              //C
  channel_4.writeMicroseconds(ch4_value);  
  channel_5.writeMicroseconds(ch5_value);  
  channel_6.writeMicroseconds(ch6_value);  
  channel_7.writeMicroseconds(ch7_value);  



//For Testing
//Serial.print("ch1: ");     Serial.print(received_data.ch1);      Serial.print("    ");      //Throttle
//Serial.print("ch2: ");     Serial.print(received_data.ch2);      Serial.print("    ");      //Z
//Serial.print("ch3: ");     Serial.print(received_data.ch3);      Serial.print("    ");      //C
//Serial.print("ch4: ");     Serial.print(received_data.ch4);      Serial.print("    ");
//Serial.print("ch5: ");     Serial.print(received_data.ch5);      Serial.print("    ");
//Serial.print("ch6: ");     Serial.print(received_data.ch6);      Serial.print("\n  ");



//If the throttle is equal or below 90 turn Break lights on.
if (received_data.ch1 <= 90){
digitalWrite(A1, HIGH);
//Serial.print("Led: High   ");
}else{
digitalWrite(A1, LOW);
//Serial.print("Led: Low    ");
}}

//Loop end
```

---
## \#2 Posted by: skelstar Posted at: 2018-05-17T02:54:31.023Z Reads: 82

```
So this is the receiver code (on the board side) and it turns the value from the controller into a PWM signal? (nice idea BTW).
```

---
## \#3 Posted by: skelstar Posted at: 2018-05-17T03:00:52.704Z Reads: 85

```
Just very quickly: this is what I came up with.
![image|690x492](upload://8Y79ayJLumwq0Nl06zWKzw4HHv6.png)
```

---
## \#4 Posted by: jasonlove199450 Posted at: 2018-05-17T16:11:58.276Z Reads: 61

```
tried that and i have a problem :(       

CODE:      


#include <SPI.h>
#include <nRF24L01.h>
#include <RF24.h>
#include <Servo.h>  //To create PWM signals we need this lybrary

const uint64_t pipeIn = 0xE8E8F0F0E1LL;     //Remember that this code is the same as in the transmitter
RF24 radio(9, 10);  //CSN and CE pins

// The sizeof this struct should not exceed 32 bytes
struct Received_data {
  byte ch1;
  byte ch2;
  byte ch3;
  byte ch4;
  byte ch5;
  byte ch6;
  byte ch7;
};

Received_data received_data;

Servo channel_1;
Servo channel_2;
Servo channel_3;
Servo channel_4;
Servo channel_5;
Servo channel_6;
Servo channel_7;

int ch1_value = 0;
int ch2_value = 0;
int ch3_value = 0;
int ch4_value = 0;
int ch5_value = 0;
int ch6_value = 0;
int ch7_value = 0;

int lastch1Value = 0;
bool oldCButtonIsPressed = false;




/**************************************************/

void setup()
{

  //Break lights output
  pinMode(A1, OUTPUT);


//For Testing
//Serial.begin(9600);   //make sure the same is selected in serial monitor!!

  //Attach the servo signal on pins from D2 to D8
  channel_1.attach(2);     //Throttle
  channel_2.attach(3);     //Z
  channel_3.attach(4);     //C
  channel_4.attach(5);
  channel_5.attach(6);
  channel_6.attach(7);
  channel_7.attach(8);
  
  //We reset the received values
  received_data.ch1 = 127;
  received_data.ch2 = 0;
  received_data.ch3 = 0;
  received_data.ch4 = 0;
  received_data.ch5 = 0;
  received_data.ch6 = 0;
  received_data.ch7 = 0;

  //Once again, begin and radio configuration
  radio.begin();
  radio.setAutoAck(false);
  radio.setDataRate(RF24_250KBPS);  
  radio.openReadingPipe(1,pipeIn);
  
  //We start the radio comunication
  radio.startListening();

}

/**************************************************/

unsigned long last_Time = 0;

//We create the function that will read the data each certain time
void receive_the_data()
{
  while ( radio.available() ) {
  radio.read(&received_data, sizeof(Received_data));
  last_Time = millis(); //Here we receive the data
}
}

/**************************************************/

void loop()
{

  //Receive the radio data
  receive_the_data();

var cButtonIsPressed = /* logic here */

//store throttle value if cButton newly pressed
if (oldCButtonIsPressed == false && cButtonIsPressed) {
    oldCButtonIsPressed = true;
    lastCh1Value = map(received_data.ch1,0,255,1000,2000);
}

if (cButtonIsPressed) {
    ch1_value = map(received_data.ch1,0,255,1000,2000); //Throttle
} else {
    ch1_value = map(lastCh1Value,0,255,1000,2000);  //Throttle
}
  ch2_value = map(received_data.ch2,0,255,1000,2000);
  ch3_value = map(received_data.ch3,0,255,1000,2000);
  ch4_value = map(received_data.ch4,0,255,1000,2000);
  ch5_value = map(received_data.ch5,0,1,1000,2000);
  ch6_value = map(received_data.ch6,0,1,1000,2000);
  ch7_value = map(received_data.ch7,0,255,1000,2000);

  //Creathe the PWM signals
  channel_1.writeMicroseconds(ch1_value);  
  channel_2.writeMicroseconds(ch2_value);  
  channel_3.writeMicroseconds(ch3_value);  
  channel_4.writeMicroseconds(ch4_value);  
  channel_5.writeMicroseconds(ch5_value);  
  channel_6.writeMicroseconds(ch6_value);  
  channel_7.writeMicroseconds(ch7_value);  



//For Testing
//Serial.print("ch1: ");     Serial.print(received_data.ch1);      Serial.print("    ");      //Throttle
//Serial.print("ch2: ");     Serial.print(received_data.ch2);      Serial.print("    ");  //Z
//Serial.print("ch3: ");     Serial.print(received_data.ch3);      Serial.print("    ");  //C
//Serial.print("ch4: ");     Serial.print(received_data.ch4);      Serial.print("    ");
//Serial.print("ch5: ");     Serial.print(received_data.ch5);      Serial.print("    ");
//Serial.print("ch6: ");     Serial.print(received_data.ch6);      Serial.print("\n  ");



//If the throttle is equal or below 90 turn Break lights on.
if (received_data.ch1 <= 90){
digitalWrite(A1, HIGH);
//Serial.print("Led: High   ");
}else{
digitalWrite(A1, LOW);
//Serial.print("Led: Low    ");
}}

//Loop end







ERROR MESSAGE:



Arduino: 1.8.5 (Windows 10), Board: "Arduino Nano, ATmega328P"

C:\Users\Jays\Desktop\longboard transmitter\NRF24_receiver_7channels_edited\NRF24_receiver_7channels_edited.ino: In function 'void loop()':

NRF24_receiver_7channels_edited:126: error: 'var' was not declared in this scope

 var cButtonIsPressed = /* logic here */

 ^

NRF24_receiver_7channels_edited:134: error: 'cButtonIsPressed' was not declared in this scope

 if (cButtonIsPressed) {

     ^

NRF24_receiver_7channels_edited:137: error: 'lastCh1Value' was not declared in this scope

     ch1_value = map(lastCh1Value,0,255,1000,2000);  //Throttle

                     ^

exit status 1
'var' was not declared in this scope

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.
```

---
## \#5 Posted by: skelstar Posted at: 2018-05-17T18:21:38.622Z Reads: 35

```
Ah yeah, can't be 'var'. I was working in another programming language at the time (I was at work).

Make it "bool cButtonIsPressed = map(received_data.ch3,0,255,1000,2000);".
```

---
## \#6 Posted by: skelstar Posted at: 2018-05-17T18:22:57.974Z Reads: 34

```
There can be more optimisation done, but this would get you over the line. For example we shouldn't be doing the "map" more than once for each "channel". We would do it once then do our logic.

Give this a go first.
```

---
## \#7 Posted by: jasonlove199450 Posted at: 2018-05-17T20:15:13.962Z Reads: 36

```
I tired what you recomended and got this error

CODE: 

#include <SPI.h>
#include <nRF24L01.h>
#include <RF24.h>
#include <Servo.h>  //To create PWM signals we need this lybrary

const uint64_t pipeIn = 0xE8E8F0F0E1LL;     //Remember that this code is the same as in the transmitter
RF24 radio(9, 10);  //CSN and CE pins

// The sizeof this struct should not exceed 32 bytes
struct Received_data {
  byte ch1;
  byte ch2;
  byte ch3;
  byte ch4;
  byte ch5;
  byte ch6;
  byte ch7;
};

Received_data received_data;

Servo channel_1;
Servo channel_2;
Servo channel_3;
Servo channel_4;
Servo channel_5;
Servo channel_6;
Servo channel_7;

int ch1_value = 0;
int ch2_value = 0;
int ch3_value = 0;
int ch4_value = 0;
int ch5_value = 0;
int ch6_value = 0;
int ch7_value = 0;

int lastch1Value = 0;
bool oldCButtonIsPressed = false;




/**************************************************/

void setup()
{

  //Break lights output
  pinMode(A1, OUTPUT);


//For Testing
//Serial.begin(9600);   //make sure the same is selected in serial monitor!!

  //Attach the servo signal on pins from D2 to D8
  channel_1.attach(2);     //Throttle
  channel_2.attach(3);     //Z
  channel_3.attach(4);     //C
  channel_4.attach(5);
  channel_5.attach(6);
  channel_6.attach(7);
  channel_7.attach(8);
  
  //We reset the received values
  received_data.ch1 = 127;
  received_data.ch2 = 0;
  received_data.ch3 = 0;
  received_data.ch4 = 0;
  received_data.ch5 = 0;
  received_data.ch6 = 0;
  received_data.ch7 = 0;

  //Once again, begin and radio configuration
  radio.begin();
  radio.setAutoAck(false);
  radio.setDataRate(RF24_250KBPS);  
  radio.openReadingPipe(1,pipeIn);
  
  //We start the radio comunication
  radio.startListening();

}

/**************************************************/

unsigned long last_Time = 0;

//We create the function that will read the data each certain time
void receive_the_data()
{
  while ( radio.available() ) {
  radio.read(&received_data, sizeof(Received_data));
  last_Time = millis(); //Here we receive the data
}
}

/**************************************************/

void loop()
{

  //Receive the radio data
  receive_the_data();

bool cButtonIsPressed = map(received_data.ch3,0,255,1000,2000);

//store throttle value if cButton newly pressed
if (oldCButtonIsPressed == false && cButtonIsPressed) {
    oldCButtonIsPressed = true;
    lastCh1Value = map(received_data.ch1,0,255,1000,2000);
}

if (cButtonIsPressed) {
    ch1_value = map(received_data.ch1,0,255,1000,2000); //Throttle
} else {
    ch1_value = map(lastCh1Value,0,255,1000,2000);  //Throttle
}
  ch2_value = map(received_data.ch2,0,255,1000,2000);
  ch3_value = map(received_data.ch3,0,255,1000,2000);
  ch4_value = map(received_data.ch4,0,255,1000,2000);
  ch5_value = map(received_data.ch5,0,1,1000,2000);
  ch6_value = map(received_data.ch6,0,1,1000,2000);
  ch7_value = map(received_data.ch7,0,255,1000,2000);

  //Creathe the PWM signals
  channel_1.writeMicroseconds(ch1_value);  
  channel_2.writeMicroseconds(ch2_value);  
  channel_3.writeMicroseconds(ch3_value);  
  channel_4.writeMicroseconds(ch4_value);  
  channel_5.writeMicroseconds(ch5_value);  
  channel_6.writeMicroseconds(ch6_value);  
  channel_7.writeMicroseconds(ch7_value);  



//For Testing
//Serial.print("ch1: ");     Serial.print(received_data.ch1);      Serial.print("    ");      //Throttle
//Serial.print("ch2: ");     Serial.print(received_data.ch2);      Serial.print("    ");  //Z
//Serial.print("ch3: ");     Serial.print(received_data.ch3);      Serial.print("    ");  //C
//Serial.print("ch4: ");     Serial.print(received_data.ch4);      Serial.print("    ");
//Serial.print("ch5: ");     Serial.print(received_data.ch5);      Serial.print("    ");
//Serial.print("ch6: ");     Serial.print(received_data.ch6);      Serial.print("\n  ");



//If the throttle is equal or below 90 turn Break lights on.
if (received_data.ch1 <= 90){
digitalWrite(A1, HIGH);
//Serial.print("Led: High   ");
}else{
digitalWrite(A1, LOW);
//Serial.print("Led: Low    ");
}}

//Loop end





ERROR MESSAGE:  



Arduino: 1.8.5 (Windows 10), Board: "Arduino Nano, ATmega328P"

C:\Users\Jays\Desktop\longboard transmitter\NRF24_receiver_7channels_edited\NRF24_receiver_7channels_edited.ino: In function 'void loop()':

NRF24_receiver_7channels_edited:131: error: 'lastCh1Value' was not declared in this scope

     lastCh1Value = map(received_data.ch1,0,255,1000,2000);

     ^

NRF24_receiver_7channels_edited:137: error: 'lastCh1Value' was not declared in this scope

     ch1_value = map(lastCh1Value,0,255,1000,2000);  //Throttle

                     ^

exit status 1
'lastCh1Value' was not declared in this scope

This report would have more information with
"Show verbose output during compilation"
option enabled in File -> Preferences.
```

---
## \#8 Posted by: jasonlove199450 Posted at: 2018-05-17T22:06:56.094Z Reads: 22

```
Forget it im a moron and i spelled lastch1Value like this lastCh1Value .. haha but now a problem . when i click the c button it doesnt do anything at all . i did a ''Serial.print(lastch1Value);''  and it always has an output of 1498. when i press the c button it stays the same where ever the anolog is :( im soo confused !!1
```

---
## \#9 Posted by: skelstar Posted at: 2018-05-17T22:09:30.031Z Reads: 24

```
Ok. Tricky for me to concentrate on this and work (code) at the same time :) ... arduino code is hard when you can't debug.

Try putting Serial.println() code where you expect code to change/flow. Put meaningful messages in the print message and debug it that way.
```

---

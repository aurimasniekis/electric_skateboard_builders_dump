# RC Servo PPM Controller with Arduino

### Replies: 2 Views: 1064

## \#1 Posted by: catalin.dragosh Posted at: 2017-07-25T08:09:54.492Z Reads: 71

```
Hello,

I've been working on setting up a controller for VESC using an arduino board.

I am using the Servo library to send PWM signals to the VESC but I am having trouble tuning it.

I have set the min and max pulse width from 1ms to 2ms in VESC PPM tab and also in my arduino program but VESC seems to respond only to a small range of values between 1.5ms and 1.6ms. Anything above that value gives the same speed.

Am I doing sth wrong? Is it suppose to be like that

I have attached my arduino code as well. It receives commands over bluetooth in the format "value in microseconds" followed by "n"


    #include <Servo.h> 
    #include <SoftwareSerial.h>
    #include <Arduino.h>

    SoftwareSerial mySerial(5, 6); 

    Servo myservo; // create servo object to control a servo

    double pos = 0; // variable to store the servo position
    int delayTime = 15; // this variable sets the delay time between each step

    String inString = "";
    int prev = 1500;

    char tbs[16];

    void setup() {
    myservo.attach(9, 1000, 2000); // attaches the servo on pin 9 to the servo object
    myservo.writeMicroseconds(1500); // sets the servo to mid point
    mySerial.begin(115200);
    }

    void loop() {

      if (mySerial.available())
      {
        int inChar = mySerial.read();    
       
        if (isDigit(inChar)) {
          inString += (char)inChar;       
        }

        if (inChar == 'n') {
          int x = inString.toInt();      

          if (x >= 1000 && x <= 2000)
          {        
            sprintf(tbs, "Current input value %d", x);
            mySerial.println(tbs);  

            sprintf(tbs, "Prev input value %d", prev);
            mySerial.println(tbs); 

            if  (prev <= x)
            {
              mySerial.println("Forward");  
              for (pos = prev; pos <= x; pos += 1) {  // accelerates from prev position to current one
                myservo.writeMicroseconds(pos);       // tell servo to go to position in variable 'pos'
                delay(delayTime);                     // delays the time before moving to the next position
              }
              prev = x;
            }
            else
            {
              mySerial.println("Back");  
              for (pos = prev; pos >= x; pos -= 1) {  // decelerates from prev position to current one
                myservo.writeMicroseconds(pos);       // tell servo to go to position in variable 'pos'
                delay(delayTime);                     // delays the time before moving to the next position
              }
              prev = x;
            }
          }
          inString = "";
        }    
      }
    }
```

---
## \#2 Posted by: saul Posted at: 2017-07-26T03:38:12.823Z Reads: 50

```
your vesc is probably on current control. and it should be. but there won't be any speed control when the motor is unloaded.

try pid mode. or better yet get a servo or an led and control that till its ready for a live test on the vesc.
```

---

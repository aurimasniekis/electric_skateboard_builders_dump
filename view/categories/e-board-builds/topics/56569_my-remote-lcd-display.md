# My remote LCD display

### Replies: 6 Views: 909

## \#1 Posted by: spork Posted at: 2018-05-24T06:13:07.423Z Reads: 195

```
I wanted a wireless display to tell me my speed and battery remaining, so I built one using an Arduino, an HC-05 bluetooth module, and an LCD display from Ebay.  I also show the condition of the battery in the remote.  It would be easy to add additional fields and add a button to see multiple pages.

This communicates with one of my two VESC controllers on my homemade electric mountain board.

If anyone is interested I'd be happy to share all the details.

![Controller 3|374x500](upload://3YWN5PIcxceTfyx9w0sfmuSp0xo.JPG)

![Controller 1|521x500](upload://tQmYUS2zElRsn7K1GsxqooXxUY.JPG)

![Board 3|466x500](upload://iHKwbMowrgc3DxsRm73EIEoUXzJ.JPG)
```

---
## \#2 Posted by: High-roller Posted at: 2018-05-24T09:11:26.892Z Reads: 153

```
Nice and simple, I like it!
Do you have a build log or a BOM we can see? I'd be curious to try making one myself!
```

---
## \#3 Posted by: mmaner Posted at: 2018-05-24T13:03:02.534Z Reads: 119

```
That's pretty damned inventive, good job :slight_smile:
```

---
## \#4 Posted by: egzplicit Posted at: 2018-05-24T13:06:03.511Z Reads: 119

```
Would be nice to see the arduino code, yes.
```

---
## \#5 Posted by: spork Posted at: 2018-05-24T13:16:56.291Z Reads: 110

```
Do you want a build-log for the controller or the whole board?  I can post either (or both).
```

---
## \#6 Posted by: spork Posted at: 2018-05-24T13:29:16.228Z Reads: 104

```
The code is based on a program written by Sascha Ederer (roboshack.wordpress.com), which 
was based on the code of jenkie (pedelecforum.de), Andreas Chaitidis 
(Andreas.Chaitidis@gmail.com) and Benjamin Vedder (www.vedder.se)

I changed only the .ino module.   I tried to upload the whole thing as a .zip file, but it doesn't like that.  So here is the main module.  Let me know if you'd like me to upload the other modules as well...

    
/*===================================================================================
  This sketch supports the wireless LCD dashboard for my electric skateboard.
  The arduino communicates with one of the VESC speed controllers via it's UART
  port.  The serial communication will take place over a pair of bluetooth HC-05
  modules. 
  
  VESC UART pinout (starting from capacitor side)
  - 5V 
  - 3.3V
  - GND
  - ADC 
  - TX
  - RX
  - ADC2

  The VESC serial port RX and TX pins are 3.3V.  This matches the RX and TX pins
  of the HC-05 bluetooth module.  But the bluetooth module VCC is 5V.
  The wiring between the VESC UART and the Bluetooth module is as follows:
  
  VESC UART      Bluetooth module
     5V             5V
     GND            GND
     TX             RX
     RX             TX

  On the hand controller end the wiring looks like this:

  Arduino Pro-mini                      Bluetooth module
     5V                                      5V
     GND                                     GND
     TX    thru 5K/10K voltage divider  ->   RX
     RX                                      TX
  

 Things I'd like to see on the LCD dashboard...
 - Speed
 - Battery voltage
 - Battery percentage remaining
 - Total mAh's used (will have to save this in static ram and allow user to reset manually)
 - Hand controller battery voltage
 
This is based on a program written by Sascha Ederer (roboshack.wordpress.com), which 
was based on the code of jenkie (pedelecforum.de), Andreas Chaitidis 
(Andreas.Chaitidis@gmail.com) and Benjamin Vedder (www.vedder.se).
===================================================================================*/
#include "config.h"
//#include "printf.h"
#include "datatypes.h"
#include "vesc_uart.h"
#include <SPI.h>
#include <LiquidCrystal_PCF8574.h>
#include <Wire.h>

float compute_battery_remaining(float volts);

LiquidCrystal_PCF8574 lcd(0x27);  // set the LCD address to 0x27 for a 16 chars and 2 line display


mc_values VescMeasuredValues;

int odd_even = 0;

float current = 0.0;           //measured battery current
float motor_current = 0.0;     //measured motor current
float voltage = 0.0;           //measured battery voltage
float c_speed = 0.0;           //measured rpm * Pi * wheel diameter [km] * 60 [minutes]
float c_dist = 0.00;           //measured odometry tachometer [turns] * Pi * wheel diameter [km] 
double power = 0.0;            //calculated power





void setup()
    {
    int error;
      
    Serial.begin(9600);
    while (! Serial);

    Wire.begin();
    Wire.beginTransmission(0x27);
    error = Wire.endTransmission();

    lcd.begin(16, 2); // Initialize the LCD
    }





/*======================================================================================================================     
        speed = VescMeasuredValues.rpm / 7.0;    RPM of motor - accounting for the fact the motor has 14 magnetic poles.
        speed = speed * 13 / 72;                 RPM of wheel after 13:72 gear reduction
        speed = speed / 60.0;                    Revs/Sec of wheel
        speed = speed * 2.666667;                Ft/Sec of wheel given its 32" circumference
        speed = speed * .6818;                   MPH of wheel
        In the end... 
        speed = VescMeasuredValues.rpm /1279.4;
========================================================================================================================*/
void loop()
    {
    delay(500);
    float battery_remaining;
    int remote_voltage;
    float rem_v;
    
    remote_voltage = analogRead(0);
    rem_v = 10.0 * (float)remote_voltage / 1024.0;  // this takes into account a 2:1 voltage divider on the input
    
    if (vesc_get_values(VescMeasuredValues)) 
        {
        // calculation of several values to be displayed later on
        voltage = VescMeasuredValues.v_in;
        battery_remaining = compute_battery_remaining(voltage);
        current = VescMeasuredValues.current_in;
        motor_current = VescMeasuredValues.current_motor;
        power = current*voltage;
        c_speed = VescMeasuredValues.rpm /1279.4;
        c_dist = (VescMeasuredValues.tachometer/38)*3.14159265359*0.000083;

        
        
        lcd.clear();
        
        lcd.setCursor(0, 0);
        if (c_speed < 10) lcd.print(" ");
        lcd.print(c_speed);
        lcd.setCursor(4, 0);
        lcd.print(" MPH     ");

        lcd.setCursor(10, 0);
        if (rem_v < 10) lcd.print(" ");
        lcd.print(rem_v);
        lcd.setCursor(14, 0);
        lcd.print(" V");

        // lcd.setCursor(10, 0);
        // lcd.print(current);
        // lcd.print(" Amps     ");

        lcd.setCursor(0, 1);
        if (battery_remaining < 100) lcd.print(" ");
        if (battery_remaining < 10) lcd.print(" ");
        lcd.print(battery_remaining);
        lcd.setCursor(5, 1);
        lcd.print(" \%   ");
        }
    else
        {
        // Error message when VESC is not connected or UART data
        // can not be read by the Arduino.
        lcd.clear();
        lcd.setCursor(0, 0);
        if (odd_even == 0)
           {
           lcd.print("Error");
           odd_even = 1;
           }
        else
           {
           lcd.print("Error * ");
           odd_even = 0;
           }
        }
    }








/*--------------------------------------------------------------------------------------------*
A 6S lipo pack is considered fully charged at 25.2V   I consider it fully discharged at 21.0V

Discharge %   Voltage/6S-pack
-----------   ---------------
 0.0          25.2000   (fully charged)
 0.948        24.5496
 11.11        23.6912
 22.09        23.1808
 33.33        22.7400
 44.31        22.4152
 55.42        22.1136
 66.40        21.9048
 77.51        21.7192
 88.48        21.5568
 94.99        21.3480
 100.0        21.0000   (fully discharged)
*--------------------------------------------------------------------------------------------*/
float compute_battery_remaining(float volts)
   {
   int i;
   float x;
   float discharge[12] = {0.0, 0.948, 11.11, 22.09, 33.33, 44.31, 55.42, 66.40, 77.51, 88.48, 94.99, 100.0};
   float voltage[12] = {25.2000, 24.5496, 23.6912, 23.1808, 22.7400, 22.4152, 22.1136, 21.9048, 21.7192, 21.5568, 21.3480, 21.0000};
   
   if (volts > 25.2) volts = 25.2;
   if (volts < 21.0) volts = 21.0;

   for(i=0; i<12; i++)
      {
      if (volts >= voltage[i]) break;
      }

   if (i == 0) return(100);
   x  =  discharge[i-1] + (discharge[i] - discharge[i-1]) * (volts - voltage[i-1]) / (voltage[i] - voltage[i-1]);

   return(100-x);  
   }
```

---

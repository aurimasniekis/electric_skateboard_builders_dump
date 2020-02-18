# Help needed for Arduino multiple LM35 temperature sensor

### Replies: 1 Views: 717

## \#1 Posted by: nikoli280 Posted at: 2017-06-18T19:33:12.724Z Reads: 22

```
Hi everyone.

I am building my first electric skateboard. And i want to monitor the temperature of the BMS, VESC and Batteries.

I have bought a Arduino Uno and 3x LM35 sensor.

I have found a stock code to get 1 sensor to work. Now my problem is how to get the other two to work. The sensor are connected to A0, A1, A2. Here is the code

I hope someone can help me


#include <LiquidCrystal.h>         

LiquidCrystal lcd(12, 11, 5, 4, 3, 2); //Digital pins to which you connect the LCD
const int inPin = 0;                   // A0 is where you connect the sensor
void setup()
{
  lcd.begin(16,2);
}
void loop()
{
  int value = analogRead(inPin); // read the value from the sensor
  lcd.setCursor(0,1);
  float millivolts = (value / 1024.0) * 5000; 
  float celsius = millivolts / 10;
  lcd.clear();
  lcd.setCursor(0,0);
  lcd.print("BMS");
  lcd.setCursor(0,1);
  lcd.print(celsius);
  lcd.print("C");
  lcd.setCursor(0,1);
  
   delay(1000);
}
```

---

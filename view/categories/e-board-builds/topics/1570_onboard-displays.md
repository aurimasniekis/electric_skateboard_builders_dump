# Onboard displays

### Replies: 25 Views: 4962

## \#1 Posted by: DougM Posted at: 2016-02-28T04:14:07.583Z Reads: 283

```
Pun fully intended.  

Huge step today, got my 3.2" TFT up and running and displaying data streamed from VESC!  Piccies:

<img src="/uploads/db1493/original/2X/8/80f27ae6757a6dd763021ae5d9a6efca7ebd2836.jpg" width="281" height="500"><br><img src="/uploads/db1493/original/2X/f/fad839f922a706f44233a161b9f774da07abc81e.jpg" width="281" height="500"><br><img src="/uploads/db1493/original/2X/d/d2233ebde2c4d4644531a1d24584c11706332a8c.JPG" width="666" height="500">

First piccie is a closeup of the display, second you can see one of the motors spinning in the upper-left.  Third piccie is the board it'll get mounted to - it'll be inset in the front riser, right in front of the footpad.

DougM
```

---
## \#2 Posted by: cmatson Posted at: 2016-02-28T04:47:13.930Z Reads: 267

```
Looks super sick man!!

I also really like you custom drop deck- this is going to be one he'll of a board
```

---
## \#3 Posted by: mostwanted Posted at: 2016-02-28T07:40:24.809Z Reads: 260

```
can you put a video ? cant seem to figure out how you'd turn .
```

---
## \#4 Posted by: psychotiller Posted at: 2016-02-28T16:14:05.845Z Reads: 257

```
It's on skate trucks. Leaning=Turning
```

---
## \#5 Posted by: DougM Posted at: 2016-02-28T16:22:09.442Z Reads: 257

```
Correct, they are Revenges up front and Caliber's in the back.  Caliber's are great because it's easy to mount a motor to them for those of us who don't weld.

<img src="/uploads/db1493/original/2X/9/95e4c5292e5b3fefa5e34ebc6310990790f2d867.jpg" width="281" height="500">

Thanks CMatson, I'm trying to build the ultimate carving machine.  I'm going to create a blog somewhere with all the build details - will post linkies.

DougM
```

---
## \#6 Posted by: trbt555 Posted at: 2016-02-28T18:33:58.749Z Reads: 239

```
Good work. Are you streaming data back over UART ?
```

---
## \#7 Posted by: DougM Posted at: 2016-02-28T20:04:47.516Z Reads: 242

```
Yes, after a little initial drama it turned out to be pretty easy.  I'm using RollingGecko's VESCUart to pull the data down as well as control the motor.

https://github.com/RollingGecko/VescUartControl

The only thing I'm not able to do yet is get Fault information from VESC.

DougM
```

---
## \#8 Posted by: onloop Posted at: 2016-02-29T07:01:19.507Z Reads: 244

```
THIS IS VERY COOL BROTHER! having this info is nice. should display wattage in real time.
```

---
## \#9 Posted by: mohammedex Posted at: 2016-03-01T00:10:58.776Z Reads: 238

```
Yeah, seems to be really sweet :smiley: How does the VESC know how fast you're spinning though? I would think that that requires a sensored setup. I've been meaning to make a speedometer for my build using an arduino, external battery, a magnet attached to the wheel and a magnetic switch sensor. Im still waiting for my VESC and don't know nearly enough about it! could you perhaps explain how you made the speedometer?
```

---
## \#10 Posted by: DougM Posted at: 2016-03-01T16:39:33.581Z Reads: 226

```
VESC returns the current RPM of the motor so then it's just a matter of maths to convert that to MPH.  The number I used was an approximation for display purposes.  I'll do it the easy way, crank the board up to full speed, record the RPM, then use the GPS on my phone to get my current speed and divide RPM by MP/H to get a conversion factor and use that in the firmware.

DougM
```

---
## \#11 Posted by: evoheyax Posted at: 2016-03-01T17:25:01.804Z Reads: 214

```
I've been reading up on vedders VESC code. I'm interested in how you pull the data to create a tachometer, as that is something I'm actively working on.
```

---
## \#12 Posted by: DougM Posted at: 2016-03-01T19:02:35.677Z Reads: 207

```
Configure your VESC for UART, wire it up and run RollingGecko's VESCUart sample code - it will demonstrate how to set the current for the motor and how to retrieve state data.

If you get stuck let me know,

DougM
```

---
## \#13 Posted by: evoheyax Posted at: 2016-03-04T01:05:29.836Z Reads: 198

```
will do when I get a chance (schools crazy right now). What wheels are you using? those look alot like the good year tires I have and have no way of using.
```

---
## \#14 Posted by: DougM Posted at: 2016-03-04T16:02:28.437Z Reads: 206

```
They are 4" wheelchair casters from a place called FrogLegs.  (froglegsinc.com)

The upside is they use the same bearings as skate wheels and are the same width so bolt right on.  The downside is they are heavy and pretty spendy.

Are your goodyear tires pneumatic?  These are solid rubber.

DougM
```

---
## \#15 Posted by: psychotiller Posted at: 2016-03-04T17:32:10.641Z Reads: 202

```
You need a set of pneumatics.<img src="/uploads/db1493/original/2X/5/5a862244df50d03bb33f6518f882f68ffe443f21.jpg" width="689" height="390">
```

---
## \#16 Posted by: DougM Posted at: 2016-03-04T18:49:18.135Z Reads: 199

```
I do!  but for a lot of reasons I'm limited to 4" tires.  If anyone can source 4" x 1" (or 1.25") pneumatics please let me know.

Also, finally got a break in the weather, so took the above board for its inaugural run.  It is fast but not as stable as I was expecting.  I'm beginning to think that for an "ultimate carving board" standard skate trucks are not going to do it.  I'm going to have to start thinking about a suspension similar to BajaBoards but with much less travel.

Thanks,


DougM
```

---
## \#17 Posted by: evoheyax Posted at: 2016-03-06T02:19:24.370Z Reads: 188

```
My good year tires are all rubber. I have been told they will suck for range, but I can use a larger battery to make up for it. I just want a smooth ride, and that I don't have right now with then enertion wheels.
```

---
## \#18 Posted by: DougM Posted at: 2016-03-06T04:05:42.887Z Reads: 194

```
Another reason to think about a different suspension.  You can't see it in the pictures, but my wood deck is floating about a half inch above the aluminum frame, suspended by rubber grommets.  this allows the flex in the wood and the squishyness of the grommets to take up small vibrations, but the frame itself gets rattled pretty harshly.

DougM
```

---
## \#19 Posted by: mcfly777 Posted at: 2016-05-13T17:06:16.848Z Reads: 181

```
hi @DougM I want to build a display (wired), but I know very little Arduino programming. Would it be possible to share your Arduino code?
thanks
Leo
```

---
## \#20 Posted by: DougM Posted at: 2016-05-13T22:34:15.885Z Reads: 183

```
Yes, there's been a lot of demand for more information, so I'll start posting details here.

Starting with this:

Order the display and the Zif connector:
http://www.buydisplay.com/default/serial-spi-3-2-inch-tft-lcd-module-display-ili9341-power-than-sainsmart

Order the PCB here:
https://oshpark.com/shared_projects/lZdlzNWj

You'll also need to order a Teensy 3.2 - you can get them from OshPark when you order the PCB.

Next I'll post a BOM.

If you want to just drive the display and don't want any of the other stuff google "adafruit ili9341" 

DougM
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-05-17T14:27:28.952Z Reads: 169

```
[quote="DougM, post:20, topic:1570"]
Next I'll post a BOM.
[/quote]

Any update on the BOM?
```

---
## \#22 Posted by: DougM Posted at: 2016-05-17T15:17:39.624Z Reads: 164

```
Yes, thanks for the reminder - I am going to build up a couple of these boards this week, so at that time will post.

Thanks,

DougM
```

---
## \#23 Posted by: DougM Posted at: 2016-05-19T02:31:01.293Z Reads: 165

```
Ok here we go:

R1, R3, R6 - these are the three resistors directly underneath the uSD card holder - 0603 47 ohm resistors.  They are the current limiters for the TFT backlight

C48 is an 0603 0.1uF cap

U$33 is a TPS73633DBVR regulator - drops 5v from VESC down to 3.3v

Q1 is a BSS215P - turns the TFT backlight on and off

R7 is 100k 0603

The Teensy you can solder directly, but I would get a chip carrier like a Digi-Key AE10004-ND

you will need to use GND, +5V (not +5V1!), TX3 and RX3 to talk to the VESC.  I use 3.5mm screwterms like digi-key 277-8588-ND which is comprised of 2- and 3- position screwterms that you can configure any way you want.

The FFC40 is going to be tricky to solder - it helps if you have some solder-wick to clean up any accidental bridges.  

That should be everything you need to drive the display.  All other components are for comms with my remote and other purposes.

I'll post code next. 

Assuming you've already looked at the ILI9341 library the next library is RollingGecko's VESCUartControl here. 

https://github.com/RollingGecko/VescUartControl

In the VescUart.h you will need to configure:

"#define SERIALIO Serial1"
 to
"#define SERIALIO Serial3"

Thanks,

DougM
```

---
## \#24 Posted by: DougM Posted at: 2016-05-21T18:35:29.882Z Reads: 146

```
Ok, here's some code.  I trimmed it down to just the parts that pull the data from VESC and drive the display.

DougM

    /* *************************************************************************************************
    2016 Doug Metzler
    
    DisplayOnly - drive VESC serial messages to a TFT display
    
    ************************************************************************************************* */
    #include <SPI.h>
    #include "ILI9341_t3.h"
    #include "font_ArialBold.h"
    #include "VescUart.h"
    
    // pin defines
    #define TFT_DC           9
    #define TFT_CS          10
    #define TFT_RST         22
    #define TFT_Backlight   21
    
    ILI9341_t3 tft = ILI9341_t3(TFT_CS, TFT_DC, TFT_RST);
    struct bldcMeasure measuredValues;
    
    void setup() 
    {
      pinMode(TFT_Backlight, OUTPUT);
      analogWrite(TFT_Backlight, 0);  // full bright
      
      Serial3.begin(115200);  // VESC
    
      // splash screen
      tft.begin();
      tft.fillScreen(ILI9341_BLUE);
      tft.setTextColor(ILI9341_YELLOW);
      tft.setRotation(4);
      tft.setFont(Arial_24_Bold);
      tft.setCursor(5,20);
      tft.print("eLongboard");
      tft.setCursor(5,60);  
      tft.print("0.1");
      tft.setCursor(5,100);  
      delay(5000);
    
      // operating screen
      tft.fillScreen(ILI9341_BLUE);
      tft.setTextColor(ILI9341_YELLOW);
      tft.setRotation(4);
      tft.setFont(Arial_40_Bold);
      tft.setCursor(5,10);
      tft.print("V");
      tft.setCursor(5,70);  
      tft.print("I");
      tft.setCursor(5,130);  
      //tft.println("MPH");
      tft.print("R");
      tft.setCursor(5,190);  
      tft.print("AH");
      tft.setFont(Arial_12_Bold);
      tft.setCursor(5,300);
      tft.print("Power = ");
    }  
    
    void loop()
    {
      if (VescUartGetValue(measuredValues)) 
      {
        tft.setFont(Arial_40_Bold);
        tft.fillRect(60, 10, 160, 41, ILI9341_BLUE);
        tft.setCursor(60,10);
        tft.print(measuredValues.inpVoltage, 2);
    
        tft.fillRect(60, 70, 160, 41, ILI9341_BLUE);  
        tft.setCursor(60,70);
        tft.print(measuredValues.avgMotorCurrent, 2);
    
        tft.fillRect(60, 130, 160, 41, ILI9341_BLUE);    
        tft.setCursor(60,130);  
        tft.print(measuredValues.rpm, DEC);
    
        tft.fillRect(100, 190, 160, 41, ILI9341_BLUE);
        tft.setCursor(100,190);
        tft.print(measuredValues.ampHours, 3);
      }
      tft.setFont(Arial_24_Bold);
      tft.fillRect(5, 245, 230, 50, ILI9341_RED);
      tft.setCursor(5,250);
      delay(1000);
    }
```

---
## \#25 Posted by: AbrownMN Posted at: 2016-05-23T20:47:27.403Z Reads: 119

```
I was thinking about achieving a similar idea, but maybe with even more potential for improvement by using a Raspberry Pi and essentialy making it into a small tablet using this kit. From there you could code in these same parameters or just install/code some sort of simple app to track them, you could download BDLC to change settings right from the board etc...

Here is the whole tutorial for the 7 inch display. I think it's a perfect, simple solution that offers a lot of function for a reasonable price.

https://learn.adafruit.com/7-portable-raspberry-pi-multitouch-tablet/overview
```

---

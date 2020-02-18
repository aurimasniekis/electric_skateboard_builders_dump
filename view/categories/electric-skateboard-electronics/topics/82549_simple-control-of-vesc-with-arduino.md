# Simple Control of VESC with Arduino

### Replies: 10 Views: 1263

## \#1 Posted by: neverpush Posted at: 2019-01-30T06:30:21.435Z Reads: 115

```
Hey guys! 

I am doing a project for school and was wondering if there is anyone who could help with some arduino code. 

The goal is simple; control the speed or position of the motor by communicating to the vesc via uart. 

I have been looking at libraries from the ArduBoard, RollingGecko, and others but I cant seem to get the code to compile properly. 

If anyone has done such a project or knows a lot about communication with VESC's  please reach out and Ill send you my code.
```

---
## \#2 Posted by: neverpush Posted at: 2019-01-30T06:33:00.208Z Reads: 115

```
@solidgeek Is this something you could help with?
```

---
## \#3 Posted by: hazza Posted at: 2019-01-30T06:42:12.865Z Reads: 110

```
you may be able to find something helpful or someone to help you in this thread
https://www.electric-skateboard.builders/t/arduino-help-and-ideas-thread/11900/53
```

---
## \#4 Posted by: pat.speed Posted at: 2019-01-30T06:48:28.797Z Reads: 104

```
Does it have to be controlled by uart? If you can use ppm it should be very simple and you could even just use the knob/sweep examples
```

---
## \#5 Posted by: neverpush Posted at: 2019-01-30T06:59:14.227Z Reads: 97

```
I does not need to be controlled via uart but I would like to be able to read the back emf on the motor eventually.
```

---
## \#6 Posted by: neverpush Posted at: 2019-01-30T07:05:02.835Z Reads: 98

```
#include <SPI.h>

#include "Config.h"

//Library for VESC UART
#include "VescUart.h"
#include "datatypes.h"
#include "local_datatypes.h"


int8_t Throttle = 0;
int8_t Brake = 0;

void setup()
{
	
	#ifdef DEBUG
	  DEBUGSERIAL.begin(115200);
	#endif
	  //Initial for Radio
	  Serial.begin(115200);
	  delay(1000);
}

void loop()
{
if (digitalRead(10) == HIGH){

		VescUartSetCurrent(((float)Throttle / 100) * 40.0));
    delay(1000);
}
else 
{
		VescUartSetCurrent(0.0);
		VescUartSetCurrentBrake(0.0);
	delay(1000);
}
}
```

---
## \#7 Posted by: janpom Posted at: 2019-01-30T07:06:24.004Z Reads: 89

```
There's https://github.com/RollingGecko/VescUartControl. AFAIK, it doesn't work with the latest VESC FW (3.40), but it should work with an older FW or you can try to fix it.
```

---
## \#8 Posted by: solidgeek Posted at: 2019-02-09T01:43:18.193Z Reads: 52

```
You can use my updated version of the VescUart library, it should be very ease to use 😊

https://github.com/SolidGeek/VescUart

However it only works for the newest vesc firmware +v3.40, so make sure your vesc is updated.
```

---
## \#9 Posted by: ZachTetra Posted at: 2019-02-09T01:58:09.689Z Reads: 43

```
Does this library have all ESC interactions?  I'm trying to do a similar project too (not gonna be ready for a while though) and I'm hoping for full feedback (like the DAVEga) and control (gonna try to rig it up to a 9 axis for turn based speed control and possibly try to get it to balance on the back wheels like a segway for point turns) or is the feed back time to long for that?
```

---
## \#10 Posted by: solidgeek Posted at: 2019-02-09T09:52:47.571Z Reads: 39

```
No it does not support all VESC features, but it has the most basic. You can see the functions in the class header (VescUart.h). I am not sure how fast the telemetry works, but as far as I remember it is not the fastest. Give it a try 😊
```

---

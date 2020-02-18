# Focbox: Motor temp. fault

### Replies: 17 Views: 294

## \#1 Posted by: Koppernikus Posted at: 2018-07-16T19:48:17.929Z Reads: 105

```
Hey there

I just uploaded the boot loader with my st-link.

Now I wanted to make a new motor detection but It doesn't work. The motor isn't able to spin. The reason is that the focbox means that the actual "T Motor" value is about 180 degrees,  Is there a function to reset or calibrate that value?

Thanks for help 
Thore

PS: I use ackmaniacs firmware
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-07-17T09:03:43.754Z Reads: 79

```
If nothing helps, just don´t use the motor temp cable. Unplug it from the connector and do your detection.
```

---
## \#3 Posted by: Koppernikus Posted at: 2018-07-17T10:45:28.948Z Reads: 71

```
I already unplugged the sensor plug but it still shows something like 179 degrees.
When I'm back home I will try to upload another firmware and hope that this doesn't show up again.

Or Could it be a hardware failure?
Could I disable the over temp. Function?
And are somewhere here some schematics about the focbox available?
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-07-17T11:51:20.937Z Reads: 62

```
you should not unplug the whole sensor plug, only the temp cable (most of the time white). Then try again
```

---
## \#5 Posted by: briman05 Posted at: 2018-07-17T12:32:51.210Z Reads: 54

```
Why did you load the bootloader? the focbox has one built in
```

---
## \#6 Posted by: Koppernikus Posted at: 2018-07-17T12:42:12.901Z Reads: 50

```
Ok i'll try that when I'm home 

Because I got some problems with the focbox and messed up the bootloader.
```

---
## \#7 Posted by: Koppernikus Posted at: 2018-07-17T14:03:16.700Z Reads: 41

```
I connected the sensor plug to the focbox without the temp Wire. But still 170 degrees motor temperature.
You have another idea?
```

---
## \#8 Posted by: TarzanHBK Posted at: 2018-07-17T14:15:44.350Z Reads: 42

```
if it still shows motor temp, then something is wrong with your focbox..
Does a sensorless detection work fine?
```

---
## \#9 Posted by: Koppernikus Posted at: 2018-07-17T14:20:24.557Z Reads: 38

```
No that's the problem. The motor temp is always to high so the motor isn't allowed to spin
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2018-07-17T14:25:36.775Z Reads: 37

```
[quote="Koppernikus, post:1, topic:62035"]
I just uploaded the boot loader with my st-link.
[/quote]

Which firmware did you put in?
```

---
## \#11 Posted by: Koppernikus Posted at: 2018-07-17T14:53:10.490Z Reads: 32

```
The actual firmware from ackmaniac. The version 3.101
```

---
## \#12 Posted by: briman05 Posted at: 2018-07-17T15:12:44.302Z Reads: 31

```
You downloaded the default 412 firmware correct
```

---
## \#13 Posted by: Koppernikus Posted at: 2018-07-17T15:23:51.279Z Reads: 30

```
Yes. I choose 410 & 411 & 412 and then on the right side VESC_default.bin

Is it possible that that's a hardware failure?
```

---
## \#14 Posted by: briman05 Posted at: 2018-07-17T16:02:54.765Z Reads: 27

```
It seems like you did everything right maybe besides messing up the bootloader the first time.  Why did you have to reload the bootloader what did you do the first time?
```

---
## \#15 Posted by: Koppernikus Posted at: 2018-07-17T16:23:42.915Z Reads: 26

```
A couple weeks ago, the last time it was alright, I was on a ride and while that it stopped and the ackmaniac app shows that abnormal motor temperature.
Then I went back home and wanted to reset the as because I thought that a bad sensor wire was the fault. And in that trouble I did something wrong while installing the new firmware and the bootloader was corrupted. So that happens first while riding
```

---
## \#16 Posted by: JohnnyMeduse Posted at: 2018-07-17T16:23:44.899Z Reads: 26

```
[quote="Koppernikus, post:11, topic:62035"]
The version 3.101
[/quote]

Ackmaniac is now at 3.102, maybe try to updated it
```

---
## \#17 Posted by: Koppernikus Posted at: 2018-07-17T18:18:53.252Z Reads: 20

```
Now I made a mistake.
I got a short between the temp wire and the 5v. Now the LEDs are out and I can't connect the ESC anymore... 😵

If I try to turn it on the Board U2 gets got. It's an GH12E, an voltage regulator for 3,3 Volts. 
I could solder a new one but do you think that's the only broken part?
Does anyone has schematics for the focbox?
```

---

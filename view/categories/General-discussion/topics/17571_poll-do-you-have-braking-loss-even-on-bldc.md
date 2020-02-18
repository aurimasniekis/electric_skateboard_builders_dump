# \[POLL\] Do you have braking loss? Even on BLDC?

### Replies: 14 Views: 1082

## \#1 Posted by: Pedrodemio Posted at: 2017-02-11T20:45:21.190Z Reads: 166

```
So, here is whats happened today, after more than a year using my board on firmware 2.10 i upgrade to @Ackmaniac 2.53 custom firmware, that is based on firmware 2.18

Straight to FOC shall we? on the first test i had several brake cutoff happens and the VESC resets, so no faults to see, went to a fresh install and  configured everything again using BLDC, went to test, same problem again, brake and sometimes the VESC resets

At this point i was freaking out about screwing my VESC a week from a trip that the main purpose was to take my board

As a last resort went back to 2.10, went to test and everything went back to normal

In the last few days i saw at least one people reporting this problem on BLDC but no one suspected of the vesc

Whats are your thoughts? did we found another bug?

As a note i modded my VESC to include the C18 capacitor pair that should solve the loss of braking on FOC 

[poll public=true]
* Yes, 2.18 firmware on BLDC
* Yes, 2.18 firmware on FOC
* No, 2.18 firmware on BLDC
* No, 2.18 firmware on FOC
* Yes, Earlier than 2.18 firmware on BLDC
* Yes, Earlier than 2.18 firmware on FOC
* No, Earlier than 2.18 firmware on BLDC
* No, Earlier than 2.18 firmware on FOC
* Yes, Ackmaniac 2.53 firmware on BLDC
* Yes, Ackmaniac 2.53 firmware on FOC
* No, Ackmaniac 2.53 firmware on BLDC
* No, Ackmaniac 2.53 firmware on FOC
[/poll]
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-11T22:03:53.670Z Reads: 148

```
When you had version 2.10 before WHT is your hardware version. Because my firmware file is only for Hardware version 4.10 and higher.
```

---
## \#3 Posted by: Pedrodemio Posted at: 2017-02-11T22:15:01.987Z Reads: 141

```
4.10 unfortunately, do you have the original 2.18 in your computer? just to rule out that some of the improvements you made are causing this, but i bet that the original will show the same behavior
```

---
## \#4 Posted by: Eboosted Posted at: 2017-02-13T05:08:36.713Z Reads: 120

```
I have the VESC reset on one of my boards.

When your VESC reseted itself what were your faults?

Was it this one?

FAULT_CODE_OVER_VOLTAGE

My VESC showed 57.68V at the moment of the reset.

What motor and wheel pulleys are you runing?
```

---
## \#5 Posted by: Pedrodemio Posted at: 2017-02-13T13:02:02.789Z Reads: 108

```
Unfortunately VESC was hard resetting, completely shutting down, so no faults logged
 But I doubt is was overvoltage since the battery was at 37V

What's bugs me most is that I had problems using the same settings as I ever used on another firmware

230Kv 12/36 80mm
```

---
## \#6 Posted by: PXSS Posted at: 2017-02-13T13:37:39.684Z Reads: 103

```
Can you replicate it on a bench?? If so attach a usb, and record the screen, maybe you can get faults for a split second before it shuts down or see what is going on. Just log everything you can and check the last few frames before it turns off to see if anything seems out of place
```

---
## \#7 Posted by: Pedrodemio Posted at: 2017-02-13T14:17:31.527Z Reads: 97

```
Good idea, I will use a rope on the wheel to simulate a long braking

But will take a while since the can't afford to have my board down during the week
```

---
## \#8 Posted by: Eboosted Posted at: 2017-02-13T14:50:01.187Z Reads: 91

```
When my vesc resets after braking it does log the fault, I just need to keep read the fault before turning the board off
```

---
## \#9 Posted by: Pedrodemio Posted at: 2017-02-13T16:50:30.775Z Reads: 86

```
When it resets yes, when it crashes and does not reset no
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-02-13T23:10:49.131Z Reads: 76

```
@Pedrodemio  Maybe your VESC has the previous Resistor for the voltage devider.

This here es what Vedder mentions on his website. 
"Note: before running the make upload command, you should open conf_general.h and select which hardware version you are using. It is printed on the PCB. Also, 2015-01-22 I changed the voltage divider resistors to allow up to 60V to be measured by the ADC, so in that case you also have to override VIN_R1 to 39000.0 in conf_general.h"

How old is your VESC?
```

---
## \#11 Posted by: Pedrodemio Posted at: 2017-02-13T23:50:52.393Z Reads: 73

```
Nice catch, it's a possibility, i bought it late 2015 from Jason, as soon as possible i will re upload your firmware and see whats the reported voltage is on a fully charged battery
```

---
## \#12 Posted by: Ackmaniac Posted at: 2017-02-14T11:23:25.300Z Reads: 65

```
And please post a screenshot of your motor settings if you still have trouble.
```

---
## \#13 Posted by: WARMAN Posted at: 2017-02-18T23:35:39.124Z Reads: 52

```
Same issue! No brakes vesc just flashes pink cuts out then I have nothing for a couple of seconds then back.
Thought maybe it's the extra trigger movement on the moded gt2b enclosure as fixing this has seemed to work for someone else,iv yet to try it. 
@Pedrodemio if you've changed the firmware and the issue went away surely it's that right!
Can I use 2.10 with a 4.12 vesc if so I'll be changing to that tomorrow,will be nice to be able to brake for a change lol
```

---
## \#14 Posted by: Pedrodemio Posted at: 2017-02-19T01:14:42.355Z Reads: 50

```
Yes you can, just pay attention to the hardware version of the firmware

Please post the results
```

---

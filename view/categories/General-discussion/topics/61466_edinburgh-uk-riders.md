# Edinburgh UK riders

### Replies: 8 Views: 348

## \#1 Posted by: Silent_bob52637 Posted at: 2018-07-10T17:33:47.281Z Reads: 62

```
Just looking to find other riders in Edinburgh to meet up with and skill/knowledge-share
```

---
## \#2 Posted by: mrav Posted at: 2018-08-31T08:30:45.343Z Reads: 40

```
Hi Silent bob, I'm in Edinburgh, developing an ebike drive unit and looking at using a VESC for the prototype.  
Do you have experience with the VESC?
```

---
## \#3 Posted by: Silent_bob52637 Posted at: 2018-08-31T08:44:27.382Z Reads: 33

```
I do have some experience with the flipsky 4.12 HW 
What can I (try to) help with
```

---
## \#4 Posted by: mrav Posted at: 2018-08-31T10:18:09.165Z Reads: 29

```
Hi, thanks for getting in touch.
I founded a start-up and got some funding from Scottish Enterprise to help with prototype costs.  I'm developing a multi-speed gearbox with integrated motor. I've bought a VESC (Maytech) and plan to use it with the prototype ebike drive unit. I need to download the BLDC tool and have a play...  there is one specific (unusual) thing I want to do though.

Do you have much experience setting up the brakes?  
I'd like to momentarily apply the brakes (eg for 0.1s duration) at a high current, then release brakes and immediately re-apply power to the motor.  This is to help with changing gear.  I can use an external programmable controller (eg arduino or similar) to send the signal to the VESC to do this, but I don't know if the VESC will be capable of doing this.  Eg is there a significant time delays/lag when you apply the brakes?  Are they instantly powerful or do the ramp up to full power?

Thanks, Mark
```

---
## \#5 Posted by: Silent_bob52637 Posted at: 2018-08-31T10:47:37.536Z Reads: 27

```
You can apply brakes by ramping up or not I haven't experienced any real brake delay 
Max brake current is going to govern how hard a braking force applied
If you want to use Arduino to send these "braking" signals it can be programmed to input into the vesc ppm input while your throttle would be via ADC not sure if both can be active at same time, I will check when home in about 45-60 mins

Jimi
```

---
## \#6 Posted by: sk8l8r Posted at: 2018-08-31T11:07:41.271Z Reads: 24

```
[quote="mrav, post:4, topic:61466"]
Scottish Enterprise to help with prototype costs
[/quote]

very cool! how much effort did that take?
```

---
## \#7 Posted by: mrav Posted at: 2018-08-31T17:29:04.120Z Reads: 19

```
A lot!!!   I spent the best part of a year doing concept designs, writing the business plan and applying for funding.  The funding application was a lengthy process, and a lot of evidence needed - quotes from suppliers & sub-contractors, financial projections for next 3 years, etc.  
Thanks for the info! Good to know there's no noticable delay - sounds like it could work...
I thought I could run all control signals through an arduino, so the arduino would receive a throttle signal and a separate signal telling it to apply brakes momentarily.  So am I right in thinking there is basically just one input signal to the VESC, which is the PPM?   Ie moving the throttle from closed (brake) to open (full power) progressively changes the ppm signal which is fed into the VESC?  Or is the brake a separate input?  Many thanks!  Searching for info on all this stuff has kind of got me interested in a powered longboard...  they seem pretty cool!!
```

---
## \#8 Posted by: Silent_bob52637 Posted at: 2018-09-01T13:58:28.226Z Reads: 17

```
Throttle control is one input that includes throttle and brake.
Ppm is just an input protocol as is ADC which your throttle will likely output. 
I assume you need erpm data from the vesc for the duino to know when to do its thing which would be available over UART.
The vesc has all three and a few more but I know ppm and UART can run simultaneously
You could have your duino read data from UART and decide when to change gear but also have your duino read the adc signal from your throttle and pass it through to vesc
No idea how you would actually code this tho as only have basic experience with duinos so far
```

---

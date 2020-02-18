# Do My BLDC settings look OK?

### Replies: 14 Views: 1346

## \#1 Posted by: slerm Posted at: 2017-06-01T18:07:28.642Z Reads: 111

```
Can someone take a look at my BLDC settings and see if everything looks ok? Everything is working on the bench, but it seems like it's spinning insanely fast, so I want to make sure I'm not going to burn something out. Set-up is:

- Dual Carvon V2 motors
- 10s3p pack from @JLabs
- Dual VESC-Xs
- Mini RC Remote from ebay

http://imgur.com/4zvL90x
http://imgur.com/NOj1d9L
http://imgur.com/VA2ooVU
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-06-01T18:51:55.811Z Reads: 94

```
Mostly looks good but I found a couple things: 
1. On App/PPM, your ERPM limit start shouldn't be 0. That means it will limit power ALWAYS. Set it to more like 57000, so it starts limiting power there and stops applying power at 60k.
2. Not a big deal but I'd raise your battery cutoff end to like 32.00 volts. It's just a little better for your battery.
3. Where did you get the 15 amps battery max? Does that battery have a 30 amp bms or something? (probably fine but if the battery has a higher current rated bms, you can raise battery max)

Other than that, as long as you did motor detection and remote calibration, looks good!
```

---
## \#3 Posted by: slerm Posted at: 2017-06-01T19:14:46.657Z Reads: 88

```
Thanks!

Battery has a 77a BMS, so I guess I can raise to around 30. I was going off of someone who had a similar build and just mimicking their settings.

I made these settings, and now noticed that when I turn my remote off the motor starts up. Any idea what's happening there?
```

---
## \#4 Posted by: t0m_r1dd1e Posted at: 2017-06-01T19:23:32.675Z Reads: 88

```
Yeah so you can use battery max to basically control your max power output. So it 30 amps feels to strong or jerky, you can lower it to whatever feels good. Alternatively, you could switch to Ackmaniac's excellent alternative framework here: https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

Then you could use Watt control mode to set a max power output explicitly. (It also allows you to add a bluetooth module and view data/change settings from your phone).

Yeah you need to set your remote min and max on App/PPM. (Ack's firmware has a really sweet calibration wizard). But if you stick with this firmware, check the display box  at the bottom so you can see what values your remote is sending. Then turn off the remote and note the value. Turn the remote back on and trim the throttle so that center is the same as when it's off (if your remote has a trim knob), then adjust your min and max pulsewidth so that neutral throttle is right in the middle.
```

---
## \#5 Posted by: yaca Posted at: 2017-06-01T19:35:18.146Z Reads: 77

```
Did you connect Master and Slave via can bus? 
Master needs "Multible ESCs over CAN", Controller ID "0", "PPM" and don't click "Send Status over Can"
Slave vesc needs Controller ID "1", "No app", click on "Send status over CAN" and don't click on "Multible ESCs over CAN"
```

---
## \#6 Posted by: slerm Posted at: 2017-06-01T19:59:22.396Z Reads: 71

```
I have it connected over CAN, but do not have settings configured in that way. I'll have to update it.

I just shrink wrapped everything to the bottom and did a test run. Acceleration seems really slow in comparison to a single motor metroboard I have. It takes a while to get going, but definitely hauls once it gets going. ANything I can change to increase acceleration or is this just standard when using hubs vs belt drive?
```

---
## \#7 Posted by: Hummie Posted at: 2017-06-01T20:07:30.780Z Reads: 69

```
Motor max 120 is the programmed limit regardless of what you put in I believe.   If u want more low speed power that's where it's at and still won't effect the true batt amp limit as its set
```

---
## \#8 Posted by: slerm Posted at: 2017-06-01T20:20:37.608Z Reads: 68

```
What would be a safe number to bump that up to? Or are you saying I could theoretically put it as high as i want and the battery limit will ultimately restrict the amp output?
```

---
## \#9 Posted by: yaca Posted at: 2017-06-01T20:28:26.462Z Reads: 67

```
Did you set your pulsewith now and change your Master/Slave settings at first. I don't know about carvon hubs, but I don't think acceleration is so weak. I use Jacob's hubs and they are a beast.
```

---
## \#10 Posted by: Hummie Posted at: 2017-06-01T20:30:00.461Z Reads: 67

```
Battery limit will restrict true amps from battery but motor amps  it goes to 200 on the screen, but the amp sensor on the vec goes to 160, and beyond that it's got a programmed limit of 120 regardless of what it shows.  
Tell us what you think and bump it up to 120!!  U will then have a true 120
Amps circulating in the motor!  I sound excited cause I am. the motors will get hotter sooner because you're putting out more power but it's only slightly less efficient than would be if u put out that amperage at a higher speed.  It's just switching losses and I believe this is just an esc loss in our use and I've never had the vesc shutdown from over-temp anyway. 
The vec!
```

---
## \#11 Posted by: slerm Posted at: 2017-06-01T21:36:21.185Z Reads: 60

```
So I changed the Master/slave settings, and bumped motor max to 120. It definitely helped with acceleration, but doesn't pull super hard. I'm ~ 175 lb, so maybe I'm too heavy. I got it to 33 mph though, and had plenty left. Not sure I need to go any faster than that...

After riding around my parking lot for a minute the motors were quite warm to the touch, and then I started having remote issues where it seemed to be cutting in and out. Not sure if I have some bad solder joints to the motors or what. Also, sometimes, not always, when i turn the remote off the motor will turn on, ramping up to a high speed. I tried re-pairing it a few times, but is still happening. Not sure why
```

---
## \#12 Posted by: yaca Posted at: 2017-06-01T22:00:27.052Z Reads: 59

```
Did you adjust the pulsewith? Click on "Display". When you turn off your remote the bar has to be at 50%. Does your receiver have failsave? With ackmaniacs software you can also adjust the value for centre pulswith, so it's a bit easier.

You got 33mph and you still had plenty left? What KV do you have, must be very high, so I understand why you are not satisfied with your acceleration.
```

---
## \#13 Posted by: hexakopter Posted at: 2017-06-04T21:07:41.373Z Reads: 50

```
[quote="Hummie, post:10, topic:24347"]
Battery limit will restrict true amps from battery but motor amps  it goes to 200 on the screen, but the amp sensor on the vec goes to 160, and beyond that it's got a programmed limit of 120 regardless of what it shows.Tell us what you think and bump it up to 120!!  U will then have a true 120
[/quote]
Before I read this false information more often (you say that in a lot of threads) let me correct you that this is just true for the VESC Tool. That means it is just true for a software that isn't even available yet. The current BLDC Tool don't have that feature and you can destroy your hardware when using currents like 200A.
I know I have said that I don't answer to your posts any longer, but when you are risking hardware of others with your BS an exception is acceptable. :smiley:
```

---
## \#14 Posted by: Hummie Posted at: 2017-06-04T21:49:14.915Z Reads: 43

```
As you say and I didnt realize there would be new firm ware for the old 4.  With the new firmware for the 4 the limits are in place but if u have the old I guess there's no limit and then the sensor ability is at 160 so that seems the safe limit.
Keep that smile and you'll be ok. 

Myself after doing 200 motor amp limit for weeks and no disaster happened while also performing better than ever it still questionable to me.   It was said I didn't put enough load on it.
```

---

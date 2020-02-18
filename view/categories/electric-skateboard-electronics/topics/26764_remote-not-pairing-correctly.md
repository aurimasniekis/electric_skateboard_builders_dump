# Remote not pairing correctly

### Replies: 26 Views: 2450

## \#1 Posted by: ATLesk8 Posted at: 2017-07-04T20:09:34.123Z Reads: 221

```
I've got a single 6374 torqueboards motor with torqueboards vesc. I was able to configure the vesc correctly, and I am able to spin the wheel/motor with the arrow keys on my keyboard. I have gone through the steps to pair the mini remote to the receiver and it seems to work as intended, however it will not make the wheel spin, and I cannot seem to find the remote working under the PPM tab. I tried to use other remotes I have (another mini from ebay, benchwheel, and GT2B), none were successful. So I'm wondering if the vesc could possibly be the issue, or am I coincidentally setting up each remote wrong? Any suggestions are greatly appreciated. Thanks.
```

---
## \#2 Posted by: JLabs Posted at: 2017-07-04T20:45:52.570Z Reads: 216

```
In the PPM tab do you have PPM selected and not Disabled? Also make sure the receiver is plugged into channel 2 with the ground (black) wire on the outside. 

Screenshots and setup pictures of this dosnt work please
```

---
## \#3 Posted by: ATLesk8 Posted at: 2017-07-05T03:42:32.573Z Reads: 198

```
Should I pull the bind plug out prior to or after powering down the vesc/receiver? I've heard multiple ways to bind this mini remote which I got on ebay. I previously had no issue pairing with this remote and vesc combo on a previous build. I can confirm that the black wire is on the outside of both the vesc and receiver. I will check the vesc settings and post them here. I am using a 10s3p pack, vesc, and motor from DIY/torqueboards. Thank you for the help in advance.
```

---
## \#4 Posted by: ATLesk8 Posted at: 2017-07-05T03:48:54.411Z Reads: 175

```
<img src="/uploads/db1493/original/3X/c/c/ccb00e7ff9b7aa958e52462b6445810a39f85c38.png" width="690" height="383"><img src="/uploads/db1493/original/3X/e/6/e6cf1e56cddcacaef241afba1188db17d54078ae.png" width="690" height="386"><img src="/uploads/db1493/original/3X/3/d/3d4c4554722280557c025d326e5ba91fc6550344.png" width="690" height="382">
```

---
## \#5 Posted by: ATLesk8 Posted at: 2017-07-05T03:54:05.564Z Reads: 157

```
<img src="/uploads/db1493/original/3X/5/1/5102259d29ffb47f27f396ddadcdb9793a940a7a.jpg" width="500" height="500">
```

---
## \#6 Posted by: ATLesk8 Posted at: 2017-07-05T17:47:28.691Z Reads: 151

```
@JLabs Do you see anything wrong here? Thanks.
```

---
## \#7 Posted by: JLabs Posted at: 2017-07-05T18:34:05.441Z Reads: 145

```
You bind the mini remote by butting in the bind plug on ch4 (bottom) and connecting the servo connector. Then power on the VESC and receiver with the controller off. After that turn on the remote with the bind button pressed in (next to nobs). You will then see the led blink and you can release the bind button. After that power off the VESC and take out the bind plug. Then go to the PPM tab and configure the min and max pulse width. Check the display box and turn on the remote. If you pull the trigger the blue hat should move. The pull the remote all the way and put in the maximum value you see in the live count box. Do the same thing for the minimum value. 

Let me know if that dosnt work.
```

---
## \#8 Posted by: ATLesk8 Posted at: 2017-07-05T20:55:53.155Z Reads: 134

```
I followed each step carefully and it seems to work with the lights blinking and then becoming solid. Then when I go to the PPM tab it doesn't move with the remote on throttle/brake. Any other ideas? Could it be my remote. They were cheap on ebay. Thanks again @JLabs
```

---
## \#9 Posted by: wafflejock Posted at: 2017-07-05T21:02:46.244Z Reads: 122

```
If you don't see any number in the ms value box then there is no pulse being sent through the signal line connected to the VESC.  If the value is somehow out of range it could affect the percentage but if it doesn't see any pulse width coming in then it's something on the receiver side (either connection between receiver and VESC or the receiver is sending no data for whatever reason).
```

---
## \#10 Posted by: JLabs Posted at: 2017-07-05T21:02:59.078Z Reads: 114

```
Hmm not sure, it may be the remote not sure.
```

---
## \#11 Posted by: ATLesk8 Posted at: 2017-07-05T21:10:51.355Z Reads: 105

```
Well I tried both mini remotes and receivers I have in all combos possible and everything indicates that the binding is working but then nothing in the ms value. Any other ideas? I also tried a gt2b and it was the same story. Could it possibly be the vesc?
```

---
## \#12 Posted by: wafflejock Posted at: 2017-07-05T21:14:29.596Z Reads: 104

```
I guess it's possible anything can fail.  I have a little super cheap ($20-30 JBTek I think can check the brand but got it on amazon) DIY oscilloscope I use for checking out my homemade receiver since ya know it's homemade it needs checking.  There are also oscilloscope apps for Android though I haven't tried using one for looking at a pulse width I think they should work it's a 1-2ms pulse (my custom receiver sends the pulse 50 times a second) and the ADC in the phone for the mic can do 22KHz I think so could try that to see, let me know if you try and that works.

---

I have this one installed it seems decent: https://play.google.com/store/apps/details?id=com.xyz.scope

---

You'd basically have to sacrifice a mic (or maybe headphone with mic) cable and you touch one end to the ground pin and one to the signal (white) line and you should be able to set a voltage point where it will try to lock onto a repeating signal (the pulse width) if it doesn't show anything coming out of the receiver while the receiver is powered and connected then there's something wrong with the receiver (or controller or whatever but not a VESC problem)

---

Cautionary note I haven't done this, you may want a voltage divider between the PWM signal and the phone since I'm not sure what the max voltage is on the input there before you start cooking things (pwm on time should be pretty small like 8-10% duty I think so probably won't be a problem momentarily but probably not good for the phone long term).
```

---
## \#13 Posted by: ATLesk8 Posted at: 2017-07-05T21:32:53.717Z Reads: 96

```
To be quite honest I'm not sure I can pull that off. Any other ideas/solutions. I have a gt2b i could try again. I'm just concerned that all these remotes seem to be working correctly but won't coooerate with the vesc.
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-05T21:44:45.607Z Reads: 94

```
Yeah hard to say without any other components to feed the info into, to see if it's the VESC or the receivers that aren't doing their job.  If you have an arduino around or quick access to one from a friend or something there are tutorials to wire up and the code for reading a PWM signal https://www.element14.com/community/thread/54304/l/reading-pwm-signals-with-the-arduino?displayFullThread=true  But without some way to isolate and test the receiver separate from the VESC (or another VESC) it's hard to say where to point the blame.  The little crappy oscilloscope has been really great for stuff like this because I don't really care if it fries and gives you a good look at what's going on with higher speed signals than you can track with a regular old volt meter.  I also eventually got a bench power supply which is useful for getting the voltages you needs so for instance could power the receiver off the bench power supply through the black and red wires with 5-6V and then hook the el-cheapo oscilloscope to the signal line.  It's a lot of crap for a relatively small problem but good for other electronics diagnostics and building as well so might be worth the investment.
```

---
## \#15 Posted by: ATLesk8 Posted at: 2017-07-06T01:10:56.464Z Reads: 89

```
@torqueboards Have you guys seen or heard of any issues with the vescs recently not working with the remotes? Any other suggestions? I've had no problem in the past with 2 of your vescs on the same firmware.
```

---
## \#16 Posted by: torqueboards Posted at: 2017-07-06T01:41:50.854Z Reads: 93

```
Did you see our youtube tutorial on it? I haven't heard of any issues as of lately. You can send it in if you want.

https://www.youtube.com/watch?v=ywUfqtKF8Zg
```

---
## \#17 Posted by: tibal32 Posted at: 2017-07-06T03:37:55.274Z Reads: 90

```
hey guys i've been having trouble trying to pair my receiver with my remote. let me explain my situation. I bought the torqueboard nano remote whic comes with the receiver and did succesfully paired. But idk how, i lost the receiver and ordered another receiver which appears to be the one from the mini remote, and i cant get my nano remote to pair with it. i dont know if they are incompatible or not, but if they arent can some one help me? :frowning:  <img src="/uploads/db1493/original/3X/8/5/859dc1c48c756441e40ec0b2b075e4bc165ea5d4.jpeg" width="281" height="500"> this what i have right now and i want to make it work.
```

---
## \#18 Posted by: wafflejock Posted at: 2017-07-06T04:54:10.872Z Reads: 81

```
Sorry not familiar with either of those but if they aren't from the same company usually you can't bind them from what I've seen (unless it's a clone or something).  With my custom control I hard coded the channel and the "pipe" used to establish a connection but most of these boards those particulars are baked into the firmware and don't think there's an easy way to flash them (since there are small variations on hardware and software used by the remote vendors)
```

---
## \#19 Posted by: ATLesk8 Posted at: 2017-07-06T16:55:24.902Z Reads: 82

```
@torqueboards Well gents...this was driving me nuts so I swapped one of the vescs from my dual hub setup. Everything seems to be running fine upon initial setup. The board rides great. In other words I believe it is a defective vesc. Looks like I'll need to swap it out.
```

---
## \#20 Posted by: wafflejock Posted at: 2017-07-06T17:00:41.070Z Reads: 82

```
Thanks for letting us know, glad you got it working.   Saw in another thread about canbus vs splitting ppm Vedder apparently said the ADC for reading the signal in the arm mcu was fried and he thought it was due to splitting the ppm cable between two vescs.  Not sure how that could be an issue with a single motor setup but guess good to know it can be sort of easily toasted.
```

---
## \#21 Posted by: torqueboards Posted at: 2017-07-06T19:52:32.484Z Reads: 79

```
@Tibal32 - We haven't added it yet but we'll be adding a nano receiver. I don't believe the Nano is compatible with the Mini Receiver.

@ATLesk8 - PM me with your order details, email, etc. We'll get you fixed up.
```

---
## \#22 Posted by: Sapphirinia Posted at: 2017-09-26T23:44:37.160Z Reads: 67

```
My receiver keeps blinking and the remote goes solid when I do those steps...
```

---
## \#23 Posted by: torqueboards Posted at: 2017-10-02T13:58:30.421Z Reads: 61

```
@Sapphirinia Yeah, that's correct. It should go solid when it does that means it paired properly.
```

---
## \#24 Posted by: ELLIOTTMORIARTY Posted at: 2017-12-19T00:24:27.955Z Reads: 56

```
My DIY custom board was working fine one day after I range tested it until the 12s4p battery died. Then a few days later the remote was taking longer to pair; when it finally did, I noticed that the board would sometimes randomly speed up and slow down on its own (which is dangerous), now the remote won't even pair with my board anymore; it just keeps blinking the green light. Anyone ever have this problem, if so, what is wrong? Is it one of my VESC's on my dual setup, the remote, or receiver?
```

---
## \#25 Posted by: yanggatang Posted at: 2019-01-03T03:13:33.114Z Reads: 19

```
I also have a connection issue
When I tried pairing the remote to the master vesc, the light signals that it has connected, but the motor won’t turn. I had this same issue back when I was pairing my remote for a single motor, and I somehow fixed it(forgot how exactly maybe by adjusting motor settings?). I was wondering if yall could help me?

Here are the links to the videos for my vesc config and setup:
https://drive.google.com/open?id=1HzCoh9pN9zzI1l8hRwPSSNPrHrFXSyr3
```

---
## \#26 Posted by: yanggatang Posted at: 2019-01-03T03:15:26.426Z Reads: 19

```
I have a 10s2p setup btw
```

---

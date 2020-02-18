# SK3 245 + 6S + VESC problem

### Replies: 47 Views: 820

## \#1 Posted by: poznan_pl Posted at: 2018-06-17T17:24:15.777Z Reads: 119

```
Hi Builders,

my e-longboard died and I decided to build one by myself. So, went with the following spec:
- SK3 245KV 6364 motor + additional HAL sensors
- 6S battery (24 Sony VTC6 3000 mAh 30A)
- VESC 4.12 - seller said he upgraded components thus it's able to work under 240 A

rest of the set is not worth to mention.
However, I faced a problem with the engine (or VESC). When it runs without a load, looks that everything is fine, while when I'm standing on the board and try to start, the engine is breaking in a weird way. Here you can see an example:
[https://vimeo.com/275506146](https://vimeo.com/275506146)

Also, I've noticed the board's acceleration is far away from the previous spec.
Do you have any ideas what is wrong?

Best regards,
Arek
```

---
## \#2 Posted by: Colson003 Posted at: 2018-06-17T17:28:37.528Z Reads: 112

```
What’s your motor max and battery max?
```

---
## \#3 Posted by: poznan_pl Posted at: 2018-06-17T17:35:02.315Z Reads: 107

```
I have this motor [https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html?wrh_pdp=7](http://Turnigy Areodrive SK3) so specs is as follows:
- motor max 70 A
- max voltage 37 V

Batteries:
- 1 cell has max discharging rate @ 30 A, so as far as understand 4 cells in a row have 120 A

To setup my vesc, I tried with values equal or higher than above:
- current motor max is 100 A
- current battery max is 110 A
```

---
## \#4 Posted by: Colson003 Posted at: 2018-06-17T17:37:02.492Z Reads: 91

```
I’d suggest turning those down. Start with 60a motor max and 40a battery max. 

That’s some bad cogging that’s going on.

Let’s see some pictures of the VESC too
```

---
## \#5 Posted by: poznan_pl Posted at: 2018-06-17T17:56:12.160Z Reads: 82

```
Ok, thanks, will give you feedback asap
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-06-17T18:47:42.224Z Reads: 80

```
if you give the motor too much current it will demagnetize the motor thus needing more current to accelerate...a vicious cycle
Btw starting from standstill without sensors is kinda unhealthy for the motor
```

---
## \#7 Posted by: poznan_pl Posted at: 2018-06-18T17:18:19.107Z Reads: 68

```
@Colson003 @Benjamin899

So I changed settings according to your suggestions but before I go for a test ride, I would like to ask you to take a look at my VESC settings.

![28|690x429](upload://vSfs47y5shA9trjNnwbrXZdMUhU.png)
![09|690x431](upload://nawpXsu5FPsB3EDvMRVjzMORZe.png)
![58|689x431](upload://8T1KlrSg0ndm4rnILgWJW91o6bI.png)
![33|690x431](upload://ylKyNQPrGdVB5llOtAjkXuH35wD.png)
![01|690x431](upload://4CIggiBvondZIviNU7DdSCrB0Qy.png)
![38|690x432](upload://reJ3Hu5wDt3zRt9vZE1pHGKIFSx.png)
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-06-18T17:25:14.386Z Reads: 52

```
looks good to me
```

---
## \#9 Posted by: Colson003 Posted at: 2018-06-18T18:42:41.271Z Reads: 54

```
You could decrease the motor min to -50
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-06-18T18:50:14.879Z Reads: 53

```
i love that you said decrease^^
```

---
## \#11 Posted by: poznan_pl Posted at: 2018-06-18T18:58:28.926Z Reads: 52

```
@Colson003 @Benjamin899
Guys, thank you for help so far. I did a test ride and it's better now. However, after 2 km I stopped to check if engine temp isn't too high and after this break, I had a problem to start. Similar problem like in the movie I posted yesterday. Also, slow climbing on the gentle hill was a huge problem for the skateboard (batteries fully charged). However, on a flat route, I made 33 km/h so I'm more than satisfied. The only change I made before I ride was to increase startup boost to 0,04, could it be a problem? Do you have any ideas on how to diagnose a problem? Probably additional Bluetooth module and iPhone app is the only solution to getting know what is going on?
```

---
## \#12 Posted by: Benjamin899 Posted at: 2018-06-18T19:11:23.837Z Reads: 48

```
did you run a motor detection? if it coggs you need to increase the duty a bit, dunno how much, normally there should be a tooltip in what increment you should increase it. 33km/h is quite fast, remember you have a 6s battery. And top Speed is also determined by gear ratio. Also climbing hills with a single drive is also realy straining for a 245kv on 6s. How much do you weigh?
```

---
## \#13 Posted by: poznan_pl Posted at: 2018-06-18T19:23:14.329Z Reads: 48

```
yes, I did a motor detection. Currently realized that my custom HALL sensors are causing problems, so I've thrown them out. Will do a test ride and will let you know. I weigh 75 kg, on the previous motor (do not know spec) and controller I was able to make 25% uphill every day, with pain but it was possible, currently, 10% is impossible, so somewhere I made mistake setting up the skateboard :slight_smile:
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-06-18T19:29:31.529Z Reads: 46

```
i am guessing the old motor had lower kv so it was easier at 6s to climb. I would like to know your wheelsize and gear ratio.
```

---
## \#15 Posted by: Colson003 Posted at: 2018-06-18T19:32:00.156Z Reads: 44

```
What brand esc is it?
```

---
## \#16 Posted by: poznan_pl Posted at: 2018-06-18T20:09:39.052Z Reads: 42

```
@Benjamin899
My gear ratio is following:
- 82mm wheels
- motor pulley 15 teeth
- wheel pulley 53 teeth if I calculated correctly :)

@Colson003 
The first electric skateboard was 1st gen Majestic Boards product, a small Polish company. It had a single motor, 6s battery, it wasn't a beast but it worked fine. After two years the battery has degraded and shortly after a battery replacement, the motor died. Current spec is in the first post.

Did a ride without sensors, and it looks that if I push throttle rapidly, the engine blocks itself - made a nice flight before noticed this issue :) So when I speed up gently, it goes even uphill, but once I move throttle to max, skateboard slows down or motor blocks itself.
```

---
## \#17 Posted by: Benjamin899 Posted at: 2018-06-18T20:16:56.871Z Reads: 41

```
i doubt that your wheel pulley has 53 teeth, not on 82mm wheels or wait, what pitch do you have
```

---
## \#18 Posted by: poznan_pl Posted at: 2018-06-18T20:19:17.370Z Reads: 41

```
Sorry Benjamin, don't understand your question...
```

---
## \#19 Posted by: Benjamin899 Posted at: 2018-06-18T20:26:10.916Z Reads: 46

```
What is your Tooth pitch on the pulley, i doubt it is 5M.
```

---
## \#20 Posted by: poznan_pl Posted at: 2018-06-18T20:34:47.972Z Reads: 44

```
Sorry, I had to google what is tooth pitch :) I don't have a precise tool to measure it, but it looks that it's 5 mm. And counted twice, 53 teeths :) 
![IMG_0500|375x500](upload://e2iiMOvH0lJ7xDc6zelmID7LLCm.JPG)
```

---
## \#21 Posted by: Benjamin899 Posted at: 2018-06-18T20:49:21.318Z Reads: 42

```
http://www.pfeiferindustries.com/documents/5mm%20HTD%20Timing%20Belt%20Pulley%20PD%20and%20OD%20Chart.pdf
This is what i mean, i think its not 5M, probably 3M, but not so important anway. Your gear ratio is good. But somehting is not right. How can you make 33km/h with that ratio at 6s. Are you sure your wheels are 82mm. Dunno one or multiple values are wrong.
You know what fits the picture, when i calculated for 10s the values fit quite good.
DId you run a new motor detection after you deinstalled the sensors?
```

---
## \#22 Posted by: poznan_pl Posted at: 2018-06-18T21:04:44.498Z Reads: 40

```
I measured speed using Strava, so probably not the most accurate measurement. The road surface if perfect smooth... I was scared a little, to be honest :) 
Yeah, currently recalculated everything on a calculator and it says I can do 20 km/h max.
Yes, I deinstalled sensors and then did a motor detection. Tomorrow will try to reduce start boost to 0.01 and also will reduce motor current max to 50A. Also, do you maybe know what is absolute max? Maybe I hit some maximum and then engine blocks itself?
```

---
## \#23 Posted by: Benjamin899 Posted at: 2018-06-18T21:22:10.563Z Reads: 40

```
the motor does no thinking, it is all in the vesc as far as i know, when i did my detection, it was cogging at the end of the test and the recommended method is to increase the duty. Absolut max no, but everyone recommends not to touch it^^
```

---
## \#24 Posted by: poznan_pl Posted at: 2018-06-19T18:39:53.811Z Reads: 41

```
CC @Colson003

Ok, I solved a problem :slight_smile:
I replaced cells in the battery, but BMS was left the same. So, I calculated max current amps based on my batteries (120 amps) while BMS limits max current to... I don't know the exact value, but I assumed it was around 20 amps (based on similar batteries found on Aliexpress :slight_smile: ). The skateboard works smooth, it isn't scary fast, it doesn't accelerate as a beast, but it is enough to commute every day. Probably will be tested other configurations as well, also in the future, I will install better BMS (thus I should be able to achieve better acceleration and better ride uphill, but for now it is really good as it is). Thank you very much for your support!
```

---
## \#26 Posted by: pat.speed Posted at: 2018-06-19T22:08:54.712Z Reads: 38

```
The bms will actually cut off if to much power is drawn, it will then recover when current drops again. I’d say that’s why it was cutting out at max acceleration. There are two ways to fix this:

1. Set your vesc to bat max <20a

2. Use the bms as charge only, there are lots of threads on this.

Ps. I used to hit 35km/h on my 6s/190kv board lots, just used 83mm and 2:1 ratio
```

---
## \#27 Posted by: Benjamin899 Posted at: 2018-06-19T22:59:21.011Z Reads: 37

```
yes but it doesnt regulate and that cutoff can end badly. okay, was it in a sligh decline?
```

---
## \#28 Posted by: poznan_pl Posted at: 2018-06-24T11:49:30.338Z Reads: 32

```
Ok, I'm back because the problem is back :) I would like to ask you about telemetry I pasted below. The first picture presents telemetry when battery max is limited to 10 amps, while the second when battery max is limited to 20 amps. It looks, that BMS cuts off current around 15 amps. It is not enough to run Tuningy SK3 245 KV 6364 motor, isn't it? I would like to mention that problem is back after replacing cables from the motor to VESC.
![10amp|690x376](upload://996M4cgmMJudha8UqDNAV1b1V9F.png)
![20amp|690x380](upload://7mnWhcv7oLeDVZlzdR4hsPbjCDa.png)
```

---
## \#29 Posted by: Benjamin899 Posted at: 2018-06-24T19:36:11.822Z Reads: 30

```
15amps for a bms is not alot especially if you run at 6s and its not bypassed. So you can try to change the bms, take it out of your board or buy one that can handle 60amps so you have headroom. Also i don't rly now why you have a 6s4p configuration, having higher voltage also adds alot to the range, it is not just mAh that influences that.
But i mean you can run it, but it will hit the limits fast
```

---
## \#30 Posted by: poznan_pl Posted at: 2018-06-26T18:49:37.241Z Reads: 25

```
@Benjamin899 @pat.speed 
thanks for the response, I went with this config only because the original spec was 6s4p and I wanted to use old components etc. However, I'm trying to connect BMS in charge only mode, do you know how to wire this thing? Currently, I have C- connected with charger minus, P- wired with - going to VESC and B- connected to the battery -.
Do you know what should I do to archive charge only mode?
```

---
## \#31 Posted by: Benjamin899 Posted at: 2018-06-26T18:52:49.933Z Reads: 25

```
have never done that, just search here in the forum or youtube. You should find something.
```

---
## \#32 Posted by: poznan_pl Posted at: 2018-06-26T18:53:33.046Z Reads: 23

```
I will try, thank you :slight_smile:
```

---
## \#33 Posted by: pat.speed Posted at: 2018-06-26T21:19:20.889Z Reads: 22

```
Yep, connect it in charge only, there are a lot of threads on this
```

---
## \#34 Posted by: poznan_pl Posted at: 2018-06-28T20:40:51.238Z Reads: 21

```
@Benjamin899 @pat.speed
Hi, the battery is connected with BMS in charge only mode, but the problem is the same. Currently, I'm able to ride a little, but when I push full throttle the skateboard stops. The same during rading uphill - more throttle means slower ride ride or stops completely.  I'm so pissed off, probably there is something with a battery or a motor :confused:
```

---
## \#35 Posted by: Benjamin899 Posted at: 2018-06-28T20:43:11.415Z Reads: 21

```
what are your current settings now that you have changed the bms to charge only
```

---
## \#36 Posted by: poznan_pl Posted at: 2018-06-28T20:48:07.228Z Reads: 21

```
During test ride was as follows:
- current max/min 60A/-60A
- battery current max/min 60A/30A

Tomorrow will check with reduced values, however, according to any specification, I see that motor current max is 70A and battery current max is 60A (4 cells in parallel, each of them can handle max discharge 15A without thermal protection).
```

---
## \#37 Posted by: Benjamin899 Posted at: 2018-06-28T20:51:08.383Z Reads: 20

```
yeah but your vesc doesnt. when you ride uphill on a single drive you will draw alot of amps. Do you have a focbox with direct fet or just the regular 4.12 vesc. because if so, you should lower your battery max to maybe 40 and that is pushing it, if it is a regular one. and battery min should be negative.
```

---
## \#38 Posted by: poznan_pl Posted at: 2018-06-28T20:55:30.139Z Reads: 19

```
well, I have the regular 4.12 vesc and the truth is during the ride I noticed on a mobile app that battery current max was ~25A... I will reduce all values and will back to you tomorrow. Again Benjamin, thank you for your support!
```

---
## \#39 Posted by: Benjamin899 Posted at: 2018-06-28T21:03:07.398Z Reads: 16

```
also on your ride up the hill? i mean the battery max?
```

---
## \#40 Posted by: poznan_pl Posted at: 2018-06-28T21:14:55.626Z Reads: 17

```
yes, ~25A was the max during the ride. I will double check it tomorrow. Also, I really didn't know for VESC a max battery current is ~40A. If so, probably I will think about modifying my battery to 8s3p, to provide more voltage to the engine but first, the skateboard has to start working correctly :slight_smile:
```

---
## \#41 Posted by: Benjamin899 Posted at: 2018-06-28T21:18:36.623Z Reads: 18

```
well on paper it is 50a continuous. but the ones with heatsink can take it better than the ones without. there are some here who don't care and let the vesc throttle itself from overheating.
I dont know man, your board reacts rly weird.
```

---
## \#42 Posted by: poznan_pl Posted at: 2018-06-30T08:52:10.536Z Reads: 20

```

On the lower settings, it is the same - full throttle = fall off from the skateboard. But I would like you to show something that may be interesting. I used VESC DataLogAnalyzer to observe what is happening during motor coggling and it seems, that it does not receive enough current from the battery (I use BMS in charge only mode).
If you take a look at a picture, you will see that at moment 1 engine should start spinning faster and faster, but it didn't start spinning until moment two (was coggling between moment 1 and 2). Am I right that there is something wrong with the battery?
![36%202|690x217](upload://nqZtoiLafjji7WCPLLozwYPEoAk.jpg)
```

---
## \#43 Posted by: Benjamin899 Posted at: 2018-06-30T15:09:59.553Z Reads: 16

```
that is above my paygrade, but it is weird behavior compared to before. Motor current goes up like crazy but the battery is not delivering.
Did you inspect the battery for any damage? 
I am by no means an expert, but it seems to come down to the battery.
@pat.speed can you look at what he postet. i have no eduacted guess left but battery.
```

---
## \#44 Posted by: poznan_pl Posted at: 2018-06-30T16:57:30.999Z Reads: 16

```
Ok, here I registered the moment in which skateboard stopped/started coggling during acceleration (in result I fell off the skateboard):
![32%202|690x141](upload://hk1bVYCZfWzJreVt3tKbjTvVwQc.jpg)  

It looks that before the skateboard stopped there was the decrease in current both on the motor and battery.
Tested spec:
- current motor 40A/-30A
- current battery 30A/-30A

Specs that I was able to ride slow (AF) but safe were:
- current motor 20A/-20A
- current battery 20A/-20A
And
- current motor 30A/-30A
- current battery 30A/-30A
```

---
## \#45 Posted by: Benjamin899 Posted at: 2018-06-30T17:04:08.229Z Reads: 15

```
did you a full visual inspection of all parts. especialy the battery?
```

---
## \#46 Posted by: poznan_pl Posted at: 2018-06-30T17:10:16.603Z Reads: 15

```
All except battery looks good, I will check the battery tomorrow as I decided to change some cables around battery after switching BMS into charge only mode. However, because of the last chart that I posted, I will also call my VESC manufacturer on Monday.
```

---
## \#47 Posted by: poznan_pl Posted at: 2018-07-02T20:33:54.616Z Reads: 12

```
Hi, generally I probably solved the problem (I say probably because I have to test it more). I did several things and don’t know exactly which one solved the problem so I will describe all of them:

* wires from the battery to the VESC - I soldered them again changing phases just in case :slight_smile: Also, I double checked if any of the phases don’t interfere with another one (the result of bad work during soldering wires to the VESC).

* checked battery - I found out that one cell was disconnected (probably it was a result of disassembling the battery, so I don’t think it was the reason of the problem with a skateboard - but you can check it just in case)

* last one and I think the real reason for my problems with the skateboard - lack of capacitor between battery and VESC!

Yes, I know, you can call me ignorant etc, you can ask how did you omit this part? Well, I’ve naively thought that if I buy VESC then I have everything I need. But on Sunday I took a look on the VESC schema and I realized there is lacking part in my build. So, I installed 2200 uF capacitor and the skateboard works perfectly.

Best regards,
Arek
```

---
## \#48 Posted by: Benjamin899 Posted at: 2018-07-02T20:53:15.024Z Reads: 13

```
weird. but if it works it works.
```

---

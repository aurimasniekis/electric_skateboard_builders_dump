# Motor/ESC brakes under hard acceleration

### Replies: 48 Views: 1957

## \#1 Posted by: Clonkex Posted at: 2017-11-25T05:41:16.191Z Reads: 149

```
So my replacement pulleys from johnny arrived on Thursday and I installed them and the new 90mm wheels today, then took the board out for a test ride. First thing I noticed, 90mm is fantastic compared to ~60 :stuck_out_tongue: Second, I noticed that now that I'm using a 15mm belt and pulleys instead of the paltry 9mm, I get 0 belt slippage no matter how hard I accelerate or brake. Woo!

Unfortunately I'm facing a strange issue. When I accelerate hard the board instantly throws me off forwards. It's not just cutting the power, it's actively braking. Except it's not a normal brake. It doesn't squeal like it normally would while braking (it's a 150A X-Car esc) and it makes a different sort of noise. At first I thought it was the receiver cutting out due to power brownouts, so I put a 220uf cap on the BEC from the ESC. Tested again, still threw me off. It's very consistent and I can replicate every time.

So I'm not sure what it could be. It doesn't sound like the ESC is braking, but it feels like it is. Sort of. I wondered if maybe it could be motor timing, but I don't know anything about that so I don't know where to start.
```

---
## \#2 Posted by: TeslaAlex Posted at: 2017-11-25T07:59:14.507Z Reads: 135

```
I have the exact same issue with my X-Car Beast... :sob:

Been trying to solve it for months but without any success. 

Does it sound and look like this? YT link: [X - Car Braking during acceleration](https://youtu.be/iRhGuUsmYLc)
```

---
## \#3 Posted by: pennyboard Posted at: 2017-11-25T08:08:42.471Z Reads: 133

```
You could be hitting the ERPM limit of your ESC and it is braking to avoid damaging itself. What is the kv of your motor and how many cells is your battery? Although I have no idea what the ERPM limit of that ESC is though, you'll have to check to see if you're exceeding it
```

---
## \#4 Posted by: trigger4point7 Posted at: 2017-11-25T08:33:00.188Z Reads: 121

```
Check for faults (DRV), I had the same issue but I could kinda about it by accelerating very slowly.
```

---
## \#5 Posted by: Clonkex Posted at: 2017-11-25T09:52:51.078Z Reads: 111

```
@TeslaAlex Yes, that's exactly it! Dang, maybe I'll have to buy a vesc after all :confused: 

[quote="pennyboard, post:3, topic:39222"]
You could be hitting the ERPM limit of your ESC
[/quote]

Except that it does that only if I accelerate hard. If I accelerate more gently I can reach full speed with no issues.

[quote="pennyboard, post:3, topic:39222"]
and it is braking to avoid damaging itself.
[/quote]

It sounds nothing like braking normally.

[quote="trigger4point7, post:4, topic:39222"]
Check for faults (DRV)
[/quote]

These are X-Car ESCs, not vescs, so checking for faults isn't a thing.
```

---
## \#6 Posted by: TeslaAlex Posted at: 2017-11-25T10:02:04.028Z Reads: 95

```
Yea, I'll will definetly throw away that garbage rc ESC and pick up a FOCBOx on the upcoming sale. Im tired of things not working properly, should have gone the VESC route like everyone said, but I was too greedy... :grin:
```

---
## \#7 Posted by: pat.speed Posted at: 2017-11-25T11:11:52.883Z Reads: 88

```
@Clonkex and @TeslaAlex I have this same esc and I might know what's wrong. This is just a theory but could you be drawing to much current and voltage sag is making you hit the low voltage? Although from the sound it doesn't sound like it
```

---
## \#8 Posted by: TeslaAlex Posted at: 2017-11-25T11:24:23.965Z Reads: 82

```
I have done several tests with a multimeter and neither Amp draw or voltage sag seems to be a problem. 

My specs:
2x 5000mah 3s 20c zippy in series
X - car beast 120a
5060 NTM Propdrive 270kv
12/36 gearing
```

---
## \#9 Posted by: pat.speed Posted at: 2017-11-25T11:25:25.719Z Reads: 79

```
Hmm maybe temp shut off? Do you need to restart the board after?
```

---
## \#10 Posted by: TeslaAlex Posted at: 2017-11-25T11:27:02.003Z Reads: 79

```
Nope, no need to restart after it shuts off. 

The ESC has a specific light (blue led blinking) for temp shutoff and it doesnt light up that way.
```

---
## \#11 Posted by: pat.speed Posted at: 2017-11-25T11:28:43.407Z Reads: 73

```
Jeez I don't know what it could be then. Did you set the motor timing to high and set all the settings? What remote are you using?
```

---
## \#12 Posted by: Clonkex Posted at: 2017-11-25T11:29:33.852Z Reads: 69

```
I haven't tried changing the motor timing yet but it's my next troubleshooting step.
```

---
## \#13 Posted by: pat.speed Posted at: 2017-11-25T11:30:39.516Z Reads: 70

```
Are you able to reach your top speed with it on the normal setting? When I go mine I could only go half throttle until I changed it
```

---
## \#14 Posted by: TeslaAlex Posted at: 2017-11-25T11:31:39.806Z Reads: 67

```
Yea I reach the top speed when accelerating slowly.

Im using this remote: [Link](https://www.ebay.com/itm/262779892776)

I have the programming card and have tried all possible settings for motor timing, low voltage shutoff etc...
This is such a wierd problem... :confused:
```

---
## \#15 Posted by: Clonkex Posted at: 2017-11-25T11:34:18.286Z Reads: 67

```
Same as Tesla, I can reach top speed easily, I just can't accelerate too hard.
```

---
## \#16 Posted by: TeslaAlex Posted at: 2017-11-25T11:35:15.600Z Reads: 72

```
What remote are you using? The only thing I have not tested yet is to change remote
```

---
## \#17 Posted by: pat.speed Posted at: 2017-11-25T11:36:32.423Z Reads: 70

```
@Clonkex @TeslaAlex I have know idea why it doesn't work mine has worked perfectly since I got it although I don't really do hard acceleration because I will fall off since my deck is so small
```

---
## \#18 Posted by: Clonkex Posted at: 2017-11-25T13:03:42.318Z Reads: 69

```
It's kind of unpleasant to test this problem too since it involves accelerating hard with the intention of having the board throw you off violently :P
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-11-25T13:07:55.186Z Reads: 68

```
just scrap it and get a focbox!
```

---
## \#20 Posted by: Rinzler Posted at: 2017-11-25T13:55:44.624Z Reads: 71

```
Have a FVT car esc on my board and when i accelerate hard it cuts off, breaks a little and just coasts for like one sec, after that i have full control again. Powering up a hill and pulling the trigger to accelerate has a similar effect, it just cuts off the power and sometimes puts me in its slow mode to protect itself. I ran a 260 kv motor, i have a 190 kv coming in the mail. It felt to me like the esc couldnt keep up with detecting the rotor position, and just freaked out and decided to cut power to slow down. Maybe i was using too much power, when accelerating and keeping my hand close to the esc it started blowing warm/hot air out of its heatsink. But the esc has always put me in limp mode after spirited riding up a hill, so i guess the issue isnt related to the power draw. Will let you know how a 190 kv works out, also will play with the setting and the software.
```

---
## \#21 Posted by: Namasaki Posted at: 2017-11-30T03:02:01.455Z Reads: 54

```
Maybe @lowGuido can shed some light here. He is an expert on the XCar Beast ESC.
```

---
## \#22 Posted by: Clonkex Posted at: 2017-11-30T03:04:55.139Z Reads: 50

```
Interesting, I didn't know anyone here was.
```

---
## \#23 Posted by: Namasaki Posted at: 2017-11-30T03:10:40.347Z Reads: 51

```
He has been using them for years although I think he uses the 150a model.
One thing for certain, if you use a Car ESC you need the programming card to adjust settings.
I would not recommend using any Car ESC as it comes with default settings.
```

---
## \#24 Posted by: Clonkex Posted at: 2017-11-30T03:13:00.050Z Reads: 55

```
I have the 150A model as well, and I don't have a programming card, I have the programming LCD thing which I plug in to my computer via USB.
```

---
## \#25 Posted by: Namasaki Posted at: 2017-11-30T03:19:34.346Z Reads: 53

```
The LCD box is a programer. I used one like that on my Torqueboards 12s ESC's
You should be plugging the ESC into the LCD box

Check out this video from Torqueboards.
https://youtu.be/hvljCjOZLUc
```

---
## \#26 Posted by: lowGuido Posted at: 2017-11-30T03:24:10.771Z Reads: 53

```
i have used X-car beast 150A ESCs on a lot of boards and I have never seen this before.
I have only ever used the 150A version though so I imagine that it could be an initial current draw too large for the ESC and some sort of protection. you could try setting your punch to low.
but as I said I have only ever used the 150A not the 120A so it could be a limitation of the 120A version.
```

---
## \#27 Posted by: lowGuido Posted at: 2017-11-30T03:26:52.871Z Reads: 53

```
I use 3.0v cutoff
Forward brake no reverse.
Motor timing very high
Initial acceleration low
0% drag brake
Brake force 70%
Neutral 4%
```

---
## \#28 Posted by: Clonkex Posted at: 2017-11-30T03:35:42.841Z Reads: 52

```
@Namasaki I know, I've successfully programmed the ESC several times. :)

@lowGuido I have the 150A version. What makes everyone assume it's the 120A version? :thinking: (I'm not annoyed btw, just curious; is the 120A more common?)

[quote="lowGuido, post:27, topic:39222, full:true"]
I use 3.0v cutoff  --- I forget what mine's set to
Forward brake no reverse. --- I currently have reverse enabled, though I'll disable it because it doesn't help anything
Motor timing very high --- haven't changed this on mine so it's probably still medium
Initial acceleration low --- same
0% drag brake --- same
Brake force 70% ---I think mine's still 50%
Neutral 4% --- I think I set mine to 10% because my controller has a slightly dodgy pot :P
[/quote]
```

---
## \#29 Posted by: Namasaki Posted at: 2017-11-30T03:39:48.664Z Reads: 50

```
@TeslaAlex has a 120a
```

---
## \#30 Posted by: lowGuido Posted at: 2017-11-30T03:40:18.712Z Reads: 51

```
sorry I thought I saw a reference to a 120A ESC above.
in all the ESC's I have used I have never seen this problem..
its replicatable always??? or only straight after boot up?????
I have seen one time where the battery detection on boot up takes a little while and the 6th beep will throw you if you try to ride it immediately.
I watched the youtube and it doesnt look like that case in the video.
```

---
## \#31 Posted by: Namasaki Posted at: 2017-11-30T03:45:09.142Z Reads: 50

```
Maybe try disabling the low voltage cutoff.
When I was running my TB 12s ESC's, I disabled the low voltage cutoff because I heard that it was not reliable and accurate anyway.
I think it's possible that your low voltage cutoff might be triggering even though your voltage is not too low.
```

---
## \#32 Posted by: lowGuido Posted at: 2017-11-30T03:47:40.770Z Reads: 52

```
yes, could well be the low voltage cutoff.. I have never found the LVC to be that useful in the HK ESC's
```

---
## \#33 Posted by: Clonkex Posted at: 2017-11-30T04:17:34.201Z Reads: 50

```
Wait, the beeps are the number of cells?? I assumed it was just an annoying arming warning. I definitely don't try to ride it until it's finished beeping, and it's 100% replicatable as many times as I want.

I'll try changing the settings when I get home. I may well have low voltage cutoff too high. I wonder if @TeslaAlex may be thinking he's changing settings on the ESC but not succeeding? Entirely possible. I'm just trying to work out if it's possible that changing settings might work, when Tesla says he's tried all the settings and it never fixed anything.

It's worth mentioning also that when I first tested my board in town I didn't accelerate very hard because of the slipping belt so I didn't see this problem while testing it, _except_ when I tried to ride up a not-super-steep hill and a little way up it threw me off.  I don't remember what the throttle was at but I think it was at full throttle and had been for about 20 seconds. It would have been just at the start of the steepest bit of the hill when it just stopped suddenly.
```

---
## \#34 Posted by: lowGuido Posted at: 2017-11-30T04:46:10.189Z Reads: 45

```
I want to say that its a low voltage cutoff related thing.
I cant be 100% sure, but I can say that any time I changed the voltage cutoff to anything other than default it didn't work for me.
so I just leave it default.
```

---
## \#35 Posted by: TeslaAlex Posted at: 2017-11-30T10:28:10.066Z Reads: 46

```
[quote="Clonkex, post:33, topic:39222"]
I wonder if @TeslaAlex may be thinking he's changing settings on the ESC but not succeeding?
[/quote]

I was afraid of this as well. To eliminate this risk, I changed the throttle limit to 50%, just to see if I really was getting any new settings, which I was. :slight_smile:

I´ll try to turn off the voltage cutoff when I get home and see if I get any different results.
```

---
## \#36 Posted by: TeslaAlex Posted at: 2017-11-30T10:31:20.855Z Reads: 44

```
[quote="lowGuido, post:26, topic:39222"]
I have only ever used the 150A version though so I imagine that it could be an initial current draw too large for the ESC and some sort of protection. you could try setting your punch to low.
[/quote]

I plugged in a Multimeter to my setup to check both amp-draw and lowest voltage. Neither of those values were a problem. I think I reached about 50A at most.
```

---
## \#37 Posted by: TeslaAlex Posted at: 2017-11-30T10:32:33.565Z Reads: 43

```
https://www.electric-skateboard.builders/t/too-many-amps-or-voltage-cutoff/36463/24?u=teslaalex
```

---
## \#38 Posted by: TeslaAlex Posted at: 2017-12-02T11:54:50.281Z Reads: 39

```
**IT WORKS!!!!!!**

I removed the voltage cutoff and it works! I dont get thrown off the board, no matter how hard I accellerate! 

Im so frickin happy, been trying to solve this for months! 

I feel kinda stupid though that I did not try it before :joy:

Thanks for your help guys! 

@Clonkex you gotta try it!
```

---
## \#39 Posted by: Clonkex Posted at: 2017-12-02T12:49:07.337Z Reads: 39

```
I'll do it first thing tomorrow morning!! :D Definitely have to get a voltmeter though haha, don't want to overdischarge my batteries!
```

---
## \#40 Posted by: Strassa Posted at: 2018-07-10T16:25:53.056Z Reads: 29

```
Sorry to revive this old post but my problem is excatly the same as mentioned in the thread. 

My HK X-Car Beast 120A ESC also shuts off when accelerating hard/climbing a hill. It also makes a wierd noise and I also can continue my ride on the fly (no restart or anything). I disabled Low Voltage Cutoff, but without success.

@Clonkex have you fixed your problem in any way? It cannot be the motor pulley that slips, right? 

Thanks for helping, was reading this forum for a long time now and just decided to make an account to ask you guys this question :)
```

---
## \#41 Posted by: Clonkex Posted at: 2018-07-10T22:40:18.023Z Reads: 28

```
In my case I ended up buying a Focbox and never actually tried disabling low voltage cutoff. If you're absolutely sure voltage cutoff is disabled (check it twice! if I remember correctly you can set the settings through the computer with a USB cable and that was easier and much more reliable than using the LCD programmer), definitely check your motor pulley. If you don't loctite your grub screws they can come loose. One time I had to remove my belt and push my board back to the car because the pulley came loose and started slipping. But it just felt like I was losing power, not a sudden cutoff.

And yeah, when I had the cutoff issue it stopped for just a fraction of a second then started again, no restart needed.

Something you could do is put a voltmeter on the board in a place you can see it while riding, then try accelerating hard and see if it drops significantly (the voltage, not the meter :stuck_out_tongue:).
```

---
## \#42 Posted by: TeslaAlex Posted at: 2018-07-11T05:10:15.605Z Reads: 23

```
DO NOT DISABLE VOLTAGE CUTOFF - my lipos went puffy after a couple of rides. Get yourself a focbox or any other 120A+ car esc. It seems as if the x-car beast has an manufacture error...
```

---
## \#43 Posted by: Clonkex Posted at: 2018-07-11T05:35:24.655Z Reads: 24

```
Well if you draw too much or take the voltage too low, of course they'll go puffy. That's not the fault of the ESC. Disabling the voltage cutoff is fine as long as you have some other way to monitor the voltage.
```

---
## \#44 Posted by: TeslaAlex Posted at: 2018-07-11T05:42:01.833Z Reads: 26

```
Yea I know, I was too desperate for a solution so I messed up. My new board has a focbox and bms, should have gone that route from the beginning...
```

---
## \#45 Posted by: Strassa Posted at: 2018-07-11T05:54:26.201Z Reads: 25

```
I disabled it, and I have a Voltmeter on the board. But since I got 4 x 5000mAh 3s LiPo's 20C (forming a 6s 10000mAh battery 40C) the Voltage doenst drop very much, 

@TeslaAlex disabling it seemed to have helped in your case, right? Maybe I have to check the setting again, but I was 100% sure I disabled it. @lowGuido stated above the he left it at the default setting, maybe that helps? :slight_smile:
```

---
## \#46 Posted by: TeslaAlex Posted at: 2018-07-11T06:31:39.791Z Reads: 24

```
I might have over exaggerated a bit... I tried the board inside my house at relatively low speed, and it did seem as if the problem was solved. But when accelerating faster outside the problem occurred again. Since then I bought a Hobbywing 120A car esc, which works great. That’s what I would recommend you to do, throw that x-car beast in the garbage or make it a $50 paperweight :smile:
```

---
## \#47 Posted by: lowGuido Posted at: 2018-07-11T10:23:41.832Z Reads: 22

```
I found with that ESC that the voltage cut off when in the "disabled" state didnt work at all. like cut off any time I tried to accelerate.  So I left it at the default cut off and never had a problem.
```

---
## \#48 Posted by: Strassa Posted at: 2018-07-11T21:20:49.538Z Reads: 16

```
@lowGuido guess I will try that tomorrow, busy at work at the moment :) will give you updates ^^

thank you guys!
```

---

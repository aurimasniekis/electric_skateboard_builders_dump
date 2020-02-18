# Wiring up the supower 12S BMS

### Replies: 60 Views: 3871

## \#1 Posted by: capfirepants Posted at: 2017-08-23T14:28:18.471Z Reads: 324

```
So I've ordered a Supower 12S 60A. I have 3x 4s LiPos in this config. 
My idea here is to somehow bypass the bms while riding, so I want to just use it for charging. I appologise for the horrible diagram, I hope it is understandable.
I was not sure which pin is 1 and which is 5 etc. for the JST connector. Is it variant A or B on the right side? My JST cables look like the one in the picture with the red cable on one side.
Thanks for having a quick look over this and letting me know if it's right. 
<img src="/uploads/db1493/original/3X/1/d/1d39952ebea31bc0842598e402dd56e235e96a6f.jpg" width="500" height="500">
```

---
## \#2 Posted by: SilentException Posted at: 2017-08-23T14:32:31.837Z Reads: 292

```
This doesn't look right, if you want to bypass it, then minus (-) from the battery should be connected directly to VESC as well. Unless B- and P- are in direct contact which I don't think they are because then charging through BMS would not make sense...
```

---
## \#3 Posted by: capfirepants Posted at: 2017-08-23T14:49:11.308Z Reads: 284

```
 Yeah, this diagram is without the BMS bypass discharge. I just wasn't sure how to wire exactly, so I left it out. How about the Balance cable?
```

---
## \#4 Posted by: SilentException Posted at: 2017-08-23T14:56:50.697Z Reads: 274

```
<img src="/uploads/db1493/original/3X/a/1/a1d3d8628fd7a6e516198b65cc62f437aae77e9c.png" width="690" height="385">

So variant B.

If you turn the BMS like in this image, from the left to right start with first + balance lead and proceed up to second to last one.
```

---
## \#5 Posted by: jmasta Posted at: 2017-08-23T16:24:59.808Z Reads: 264

```
Don't bypass a 60A BMS.  You lose one of the most important features:  individual cell voltage over-discharge protection.  This is especially critical with lipos.  Often a few of the cells will have significantly more voltage sag, and it only gets worse over time. You will be unknowingly wrecking havoc on your batteries

So for example, if you drop to 46.2V under load, you might think all your cells are at 3.85V.  But this is the ideal case, and generally is not true at all, especially with lipos.  Some cells might be at 3.95V, while one cell might actually have drifted down to 3.2V or lower. Release the load and they all go back to the same voltage. So you think your pack is "balanced". But its not balanced under load
```

---
## \#6 Posted by: capfirepants Posted at: 2017-08-23T17:55:07.127Z Reads: 238

```
Thanks for those insights, I did not know that.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-08-23T18:36:16.320Z Reads: 234

```
Right On! @jmasta

Also if you bypass, you would not have short circuit protection which can save your entire system if a short occurs. 

This happened to me on one of my builds when a had a short at the charge port. The bms instantly shut the whole system down and nothing was damaged.

Besides you don't need to bypass anyway with a 60a bms.
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-08-25T05:56:00.604Z Reads: 212

```
I plan on upgrading to dual motors within the coming weeks, and I have hit 50A with my single motor on startup, do you think when I upgrade it will cause the BMS to become overloaded?

I have this same exact bms wired with discharge enabled :slight_smile:
```

---
## \#9 Posted by: Namasaki Posted at: 2017-08-25T06:38:14.508Z Reads: 204

```
How do you know your hitting 50a and do you mean 50a motor current?
```

---
## \#10 Posted by: ShutterShock Posted at: 2017-08-25T14:40:01.450Z Reads: 199

```
Yes I mean 50a motor current, from a slow start with a tiny uphill.  I have the hm-10 bluetooth module installed with the VESC monitor app :slight_smile:
```

---
## \#11 Posted by: Namasaki Posted at: 2017-08-25T15:41:57.726Z Reads: 197

```
Battery current and motor current are not the same. 
Battery current is normally less and they are both controlled by the Vesc anyway.
```

---
## \#12 Posted by: ShutterShock Posted at: 2017-08-25T17:04:55.464Z Reads: 186

```
Ohhh okay so the current monitored by the app is the current drawn from the battery?
```

---
## \#13 Posted by: Namasaki Posted at: 2017-08-25T17:56:12.397Z Reads: 184

```
I'm not familiar with the app you're using
I wouldn't fully trust those Bluetooth apps anyway. 
I have the Metr module and app and it doesn't even display voltage correctly. 
I have tested battery current with an inline watt meter. 
Running dual motors going up a fairly steep hill the total current draw on the battery was only 18 amps
With 12s voltage
```

---
## \#14 Posted by: ShutterShock Posted at: 2017-08-25T17:58:05.693Z Reads: 171

```
ah apologies, the app I am using is the one from Ackmaniac's thread.  The VESC Monitor
```

---
## \#15 Posted by: ShutterShock Posted at: 2017-08-25T19:10:44.572Z Reads: 175

```
Oh alright that is good to hear, thanks for your input :smiley:
```

---
## \#16 Posted by: Namasaki Posted at: 2017-08-25T19:33:36.460Z Reads: 180

```
I'm currently running an 80a Bestech bms. 
Dual motors with Vescs set at 80a motor max and 50-60a battery max for each Vesc. 
Even when riding hard up hills I'm having no issues.
```

---
## \#17 Posted by: ShutterShock Posted at: 2017-08-25T19:35:29.959Z Reads: 180

```
Sweet.  Can't wait to upgrade mine for that extra punch at the beginning and better brakes
```

---
## \#18 Posted by: capfirepants Posted at: 2017-09-05T10:03:46.592Z Reads: 187

```
So I've figured out the balance wires wiring and created the connector. Now I just have 2 more questions:
Is the vedder switch wired correctly according to this diagram?
<img src="/uploads/db1493/original/3X/a/8/a8fe4ea175e8f44e5518be6f402b53062572a709.jpg" width="500" height="500">
How do I solder this switch: https://www.aliexpress.com/item/High-Quality-1-PC-New-Waterproof-16mm-12V-Latching-Push-Button-Power-Switch-Black-Metal-Blue/32767204345.html to the Vedder antispark to make the LED light up? Am I right in assuming I need a voltage converter or can it be done otherwise somehow? If possible, that would be great, as I could save some space....
```

---
## \#19 Posted by: capfirepants Posted at: 2017-09-06T10:35:21.538Z Reads: 174

```
@goldenHusky @Namasaki  @jmasta can you guys help me out?
```

---
## \#20 Posted by: goldenHusky Posted at: 2017-09-06T11:10:20.101Z Reads: 175

```
@capfirepants 
I have never wired a BMS but I guess the the schematic is correct, otherwise you'd have to switch your board on for charging.

To make the LED light up while your board is switched on you need to use an additional resistor, it says 1,9k on the picture but this will most likely be too bright, use a value between around 4k and 6k instead.

https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/a/a/aab2430d32f88afeb65b8ce99772eda64ef05c32_1_665x500.png
```

---
## \#21 Posted by: capfirepants Posted at: 2017-09-06T11:46:02.226Z Reads: 166

```
@goldenHusky great, thanks! What about the fuse? What do I need there?
```

---
## \#22 Posted by: goldenHusky Posted at: 2017-09-06T12:16:56.985Z Reads: 163

```
@capfirepants ATO size 40A fuse or you can bridge the pads with a wire.
```

---
## \#23 Posted by: capfirepants Posted at: 2017-09-06T13:03:57.326Z Reads: 154

```
@goldenHusky Does 40A make sense if my BMS is 60A? Or is it to protect the switch?
```

---
## \#24 Posted by: goldenHusky Posted at: 2017-09-06T13:27:01.769Z Reads: 153

```
The switch could handle more, there is just no ATO sized fuse with more than 40 amp. 40A is like the standard value for a fuse in an electric board, I don't think you will pull more, especially at 12s.
```

---
## \#25 Posted by: jmasta Posted at: 2017-09-06T15:48:53.607Z Reads: 158

```
My LED switch is powered directly by a 12V BEC.  Using resistors to drop the voltage is an option, but it burns more power than you'd expect...  

The LED in those switches are usually 15 mA

R = V/I = (50.4-12)V / 0.015A = **2.56 kΩ**

However, this burns over half a watt of power:

P = I^2*R = (.015A)^2*(2560) = **.576W**

Those little resistors you see everywhere are only 1/4W resistors. So you would need to use two 5.2kΩ 1/4W resistors wired in parallel, or two 1.3kΩ 1/4W in series. Or use a 1W resistor like the image above


If you want to use only a single 1/4W resistor, you'd have to limit your LED to current to 6mA by using a resistance value around **6.4kΩ**.  The power dissipation in this case would be **.23W**
```

---
## \#26 Posted by: jmasta Posted at: 2017-09-06T15:51:27.125Z Reads: 156

```
[quote="capfirepants, post:21, topic:31314, full:true"]
@goldenHusky great, thanks! What about the fuse? What do I need there?
[/quote]

You don't need a fuse if you are discharging through a 60A BMS.  The BMS is essentially a self-resetting fuse.  If you happen to go over 60A for some reason, it just cuts the load and automatically recovers a few seconds later.  Much better than blowing a fuse and completely shutting down your board
```

---
## \#27 Posted by: jmasta Posted at: 2017-09-06T16:00:47.202Z Reads: 156

```
[quote="goldenHusky, post:22, topic:31314, full:true"]
@capfirepants ATO size 40A fuse or you can bridge the pads with a wire.
[/quote]

The switch only cuts the negative line, so you don't need to bridge the pads.    You can use the anti-spark without a fuse by just connecting one of the two positive output solder pads (upper right in image above) to your positive line.  You don't even need to use heavy gauge wire.  A small 22AWG wire is more than sufficient
```

---
## \#28 Posted by: capfirepants Posted at: 2017-09-06T18:08:10.965Z Reads: 157

```
Do you mean these 2 up here? (Blue Circle)
<img src="/uploads/db1493/original/3X/c/b/cbc814e814aee66fb034c754370c5aedc3e72024.png" width="665" height="500">
```

---
## \#29 Posted by: jmasta Posted at: 2017-09-06T18:31:09.845Z Reads: 144

```
Yeah those ones. They are connected to each other via large traces on the PCB. So they are effectively the same
```

---
## \#30 Posted by: capfirepants Posted at: 2017-09-21T17:43:21.545Z Reads: 140

```
So ive tried wirong up my bms but it will only output 2 volts - input voltage is 46 volts. Am I doing something wrong?
I plugged it in in the order:
B-
Balance cable
P-
```

---
## \#31 Posted by: jmasta Posted at: 2017-09-21T17:47:17.448Z Reads: 134

```
Whoa don't give it 46V input!  You might have fried that thing already

The SuPower BMS only acts on the negative main line. The positive main is completely untouched.  

B- goes to Battery negative
P- goes to anti-spark switch negative (or VESC negative)
```

---
## \#32 Posted by: capfirepants Posted at: 2017-09-21T17:56:09.888Z Reads: 127

```
@jmasta Im sorry, that was a but unclearly worded - the voltage across B- and Battery + is 46v.
The voltage right before the anti spark switch (and at P-) abd the plus line is 2v.
```

---
## \#33 Posted by: jmasta Posted at: 2017-09-21T18:01:04.588Z Reads: 137

```
That's weird...

Use your voltmeter to check the following voltages, and maybe I can help you troubleshoot

* B+ to B- = 46V
* B+ to P- = ?
* B- to P- = ?
```

---
## \#34 Posted by: capfirepants Posted at: 2017-09-21T18:06:08.865Z Reads: 131

```
@jmasta 
Without "load" (no vescs plugged in) 
B+ to P- = 43.58v
B- to P- = 1.926v
With load:
B+ to P-: 0.0v
B- to P-:46v
Thinking about it, this is very wierd.
```

---
## \#35 Posted by: longhairedboy Posted at: 2017-09-21T18:43:27.342Z Reads: 130

```
check your balance lead order. its easy to get them crossed. weird shit happens when the streams cross. hellfire and damnation, dogs and cats living together, total protonic reversal.
```

---
## \#36 Posted by: capfirepants Posted at: 2017-09-21T19:06:08.042Z Reads: 131

```
@longhairedboy
Ok, so from B- as - i tested the voltages for all Balance wires. From Left to right, they have the following voltages:
3.7
7.5
11.3
15.17
19.1
23.4
26.9
30.8
34.6
38.4
42.2
46.1
As I understand it, the voltages without load from my last post would be somewhat correct?
Edit: i tested without the bms - the vescs lit up. Looks like the problem really is there.
```

---
## \#37 Posted by: longhairedboy Posted at: 2017-09-21T19:27:40.171Z Reads: 131

```
[quote="capfirepants, post:36, topic:31314"]
3.7
7.5
11.3
15.17
19.1
23.4
26.9
30.8
34.6
38.4
42.2
46.1
[/quote]

hmmmm.... the distance between those numbers should be more similar than they are. The pgroup cell voltages should be more even, but yours appear to be as follows:

3.7, 3.8, 3.8, 3.87, 3.93, 4.3 (not so good!), 3.5, 3.9, 3.8, 3.8, 3.9

They should all be within a tenth of a volt of each other. I think you may have overcharged one of your p groups some how. If you have a single cell charger, try charging each p group individually and see if it will go all the way up to 4.2 without issue, then assemble the pack and se if the BMS complains, then fully discharge the whole pack and re-charge and see if the BMS is able to balance it again properly.
```

---
## \#38 Posted by: capfirepants Posted at: 2017-09-21T19:29:30.996Z Reads: 123

```
@longhairedboy Ok - I have a single cell charger! Ill hook the batteries up now to test.
Also just tested - when I plug the vesc in, it lights up for a second before turning off. Maybe the BMS limiting the output?
Checking the batteries - some cells are at 3.9, while some are at 3.8. Is this a problem?
```

---
## \#39 Posted by: capfirepants Posted at: 2017-09-22T08:28:33.303Z Reads: 126

```
@longhairedboy @jmasta
I've also noticed that the BMS makes a sound when it gets olugged in (circuit is closed). Its high pitched and goes even higher until it is bearly audible to me. Sounds like something charging up?
```

---
## \#40 Posted by: longhairedboy Posted at: 2017-09-22T11:53:42.648Z Reads: 138

```
They should be as close to each other as possible. If you can get them all to 3.9 (if that's the highest besides the overcharged 4.3v outlier) it would be ideal. And ideally if you could discharge that overcharged pgroup down to 3.9 slowly using a small drain like from a flashlight or tiny motor or something then that would be good too. Otherwise you may have to rely on the BMS to trim it down which may not happen if the issue is with your BMS. 

The point of all of this is to see if the cells stay balanced, that way you can see if your BMS is doing its job or fucking off instead. 

I'm in the middle of a pgroup transplant on an evolve mod pack that got sent back. The cells they ordered weren't from a reputable source, so some of them just weren't up to snuff and made the whole pgroup suffer. So now i'm digging through the spare cells they sent trying to line up a few good ones and charging them individually on my Sunkko. The charger on the Sunkko 788H is legit. IT takes a while but you get a full and properly trickled in charge. But at 3-4 hours per cell its taking me a couple days. 

TL;DR i feel your pain.
```

---
## \#41 Posted by: rich Posted at: 2017-09-25T13:56:13.205Z Reads: 130

```
I am thinking of ordering this BMS, too because of its size but I don't understand the specifications. It says "max. continuing discharge current: 60A" but also "over-current Protecton: 60 A". This makes no sense to me. So it supports 60A continious and shut off at 61A???

I have 3x 10S BMS so far with max. continuing discharge current: 60A and over-current Protecton: 120 A. This is how it makes sense. It seems like the supower BMS is rated for 30A cont. with 60A over-current to me. 

Please someone help me to understand. I need this for MTB and am afraid it's too weak.
```

---
## \#42 Posted by: jmasta Posted at: 2017-09-25T14:28:55.534Z Reads: 129

```
The 60A SuPower BMS can handle up to 60A.  If you draw more than 60A, it temporarily cuts the load to prevent damage

There are different versions if you need more current

<img src="/uploads/db1493/original/3X/d/f/dfab17d31cc1d9b8c3e2e27a9ab38005b01c3602.png" width="690" height="398">
```

---
## \#43 Posted by: rich Posted at: 2017-09-25T17:26:33.745Z Reads: 122

```
Thanks for explanation @jmasta! I’m not new to BMS topic (but no expert) but my point is that supower seems to be the same 30A BMS no matter if they say 30A, 45A or 60A. All BMS in this world I know have over-current protection about the double amount of cont. discharge. Imagine a Lipo would have the same discharge and burst rate, that’s not legitimate. 

I need a BMS with 60A cont. and 120A over-current protection so it doesn’t shut off when I exceed the 60A for a couple of seconds. 

Unfortunately I killed my 10s 10Ah Graphene Lipo a couple of days ago, where I had the BMS for charging only. After the ride the voltage was 35V but I forgot to switch off the board, 28 hours later the voltage was 9V and the Lipos puffed and dead.

I can’t use nice and big 80A BMS like @Namasaki because I have no space for it. I want to uprade to 12s but I can’t find a proper BMS which is not big as a book. I have 10S BMS 60A/120A (9cm x 9cm) which are nice but I need 12S now. 

I can’t believe that I can’t find any nice 12s BMS with not more width than 9cm (except supower).
```

---
## \#44 Posted by: Namasaki Posted at: 2017-09-25T17:37:56.841Z Reads: 111

```
The Bestech bms that I use might have saved your battery by automatically turning off when min voltage was reached.
```

---
## \#45 Posted by: longhairedboy Posted at: 2017-09-25T17:42:08.325Z Reads: 113

```
I've been using those 60 Amp BMSs in my boards all year and zero issues. 

With the proper VESC settings you'll get up to ludicrous speed and still go full plaid without tripping the BMS.
```

---
## \#46 Posted by: jmasta Posted at: 2017-09-25T17:54:19.714Z Reads: 109

```
The top three BMS's I showed do look identical and are basically the same price.  My guess is that they designed one board to withstand 60A and then down-regulated the 45A and 30A models.  By simply changing the over-current setting you can meet a wider range of needs for your customer.  This allows them to manufacture a single PCB with the same hardware, which drastically cuts costs.  If you look closely at the 12S version, you'll notice a whole row of resistors is missing.  That's because they use the same PCB for 13S. Similarly on the 11S variant, two rows are "missing"
```

---
## \#47 Posted by: Namasaki Posted at: 2017-09-25T17:55:38.182Z Reads: 103

```
He would have been fine with the Supower bms except he forgot to turn his board off before storing it.
```

---
## \#48 Posted by: rich Posted at: 2017-09-25T17:58:24.545Z Reads: 106

```
True @Namasaki  :cry:, We had a conversation in your thread some time ago and you suggested me to use my "proper" BMS for discharge instead of my small one for charging only. I did enjoy riding more than change the BMS, now it's too late, f***!

@longhairedboy I need this BMS for my E-MTB with dual VESC 6 so I think I'll exceed 60A from time to time. I already almost died because of a remote drop out on full speed approaching a road with traffic :joy:, next killer is the BMS why I can't break. But I think I give it a try and if it shuts off I'll use it for charging only (and hopefully don't forget to switch off my board). Maybe it works.

@jmasta you're right, that makes sense.
```

---
## \#49 Posted by: longhairedboy Posted at: 2017-09-25T18:19:55.735Z Reads: 106

```
yeah.. you might need more than 60 amps there. lol

as soon as those open source JTAG ones i'm buying into with the rest of the group prove themselves i'm switching over wholesale. They're 100 amps and have a fuse holder and a number of other features i need within a smaller footprint.
```

---
## \#50 Posted by: ShutterShock Posted at: 2017-09-26T07:26:15.036Z Reads: 105

```
I use this exact BMS for my street board, 2x 6355 190kv at 12S and I have pulled all the way up to 60A battery current no problem, granted it hasn't been a sustained load, just when really accelerating hard :stuck_out_tongue:
```

---
## \#51 Posted by: b-rad Posted at: 2019-01-24T23:56:21.411Z Reads: 45

```
Does anyone know if this wiring diagram is correct for the 12s battery supports BMS?? 

I have this exact setup and batterys i just need to know if this is correct for regular charging/discharge

Thanks ahead of time!

![image|537x500](upload://dEqw0NbiKtUWnHrNRXb94FGC1HE.jpeg)

![image|681x500](upload://e4uqyBp2UXhmQ8j6dklEogp2yDQ.jpeg)
```

---
## \#52 Posted by: TowerCrisis Posted at: 2019-01-25T00:02:01.023Z Reads: 44

```
Have you got a loop key? You'll need one (or an e-switch) between the vesc and the BMS.

Also, make sure it is between the vesc and where the charging port wires tap into the main line. Otherwise you'll need your board to be on to charge, which you don't want.
```

---
## \#53 Posted by: b-rad Posted at: 2019-01-25T00:22:19.991Z Reads: 43

```
Yes, I have a loop key exactly where you mentioned between the vesc and where the charging port wires tap into. 

So with the loop key in the correct place will this diagram work for this BMS? For the balance wires should i just leave out the ground wires? 

![ves|606x500](upload://cZYeDEPQ3QxcXIbjU2ZIdlgSXar.png)
```

---
## \#54 Posted by: Jumpman Posted at: 2019-01-25T01:07:57.487Z Reads: 39

```
Make sure you double check the balance port wiring.  The numbers 1-12 on the picture above are a bit confusing, I think it should read 12-1, like in the other picture you posted.
```

---
## \#55 Posted by: Dwain Posted at: 2019-02-09T15:07:52.545Z Reads: 34

```
Hey can anyone please help me I am having the same problem with my supower 12s BMS.  High pitched noise when connecting and powering on esc and voltage is low and fluctuating up and down and esc won't work..

Anyone please help it is brand new and I am pretty sure I connected it correctly.
```

---
## \#56 Posted by: Daniloquacquarelli Posted at: 2019-04-09T14:36:01.339Z Reads: 29

```
Hi @b-rad 
hello I have the same bms but I don't know exactly how to connect everything since I always have the current passing ... where should I put the loop key? who can help me?
in substance bon I manage to cut the current, with or without a loop key it remains all lit ... the loop key is on the B-bel bms
```

---
## \#57 Posted by: b-rad Posted at: 2019-05-08T20:17:05.384Z Reads: 28

```
So I recently got a chance to test this new BMS hooked up to my lipos and i noticed when i was doing a range test that i would only get about 10 miles per charge... before i hooked up the BMS to my lipos (12s1p) or (3x 4s 10,000mah LIPOS) i was gettting a range of about 16 miles. can someone help me understand what can be causing this and how to fix it? i have a feeling it has to do with the charger. the charger says 12S 12x 3.6V on it but my lipos full charge per cell is 4.20v, im not sure what the 12S 12x 3.6V is suppose to mean if it says that the charger goes up to 50.4v which is what i need for 100%.  

this is the BMS used: http://www.batterysupports.com/44v-48v-504v-12s-150a-12x36v-lithium-ion-lipolymer-battery-bms-p-394.html

this is the charger used: http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html
```

---
## \#58 Posted by: linsus Posted at: 2019-05-08T21:03:30.010Z Reads: 24

```
Meassure output on charger with DMM to see voltage. My guess is that the cutout on the bms hits sooner than without. Guessing u set stepoff voltage in vesc previously?

Discharge battery to what the BMS exhibits as "empty" check individual cell lvls. 

Do the same after charging it with the charger to full
```

---
## \#59 Posted by: b-rad Posted at: 2019-05-09T01:42:37.678Z Reads: 22

```
Okay sounds like a good plan, but should i use these terminals to check the voltages? or should i check the voltage on the end of the loop key? just to see if it adds up to 50.4v? check the attached image

![terminals|690x430](upload://a5431FZwR2HqJe4BwUnLWz4TaLU.png)
```

---
## \#60 Posted by: linsus Posted at: 2019-05-09T06:25:58.079Z Reads: 20

```
There or somehwere else u can see it. W/e works
```

---

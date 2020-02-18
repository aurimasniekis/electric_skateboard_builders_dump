# 10s BMS for 9 cell LiPo battery setup - wiring diagram

### Replies: 46 Views: 2083

## \#1 Posted by: MrDGOrman Posted at: 2018-09-27T17:13:48.379Z Reads: 129

```
Hello everyone,

I purchased myself the BMS below from eskating.eu. Just wondering how I go about wiring everything up!
https://eskating.eu/product/10s-bestech-bms-80a-10s4p/

I'm using this BMS with a 9 cell LiPo battery setup (see diagram below). Which wire should go where?

If someone could be kind enough to alter my image so that I know where the switch (Sw?), fuse, and balance leads should go then I'd be really grateful. There's also B-, P- and C-. What are these for? @b264 can you help?

![BMS%20wiring%20diagram|574x499](upload://9ppmVTTYbcnbNJ9pnnJUNYOKvIP.png) 

Also, on a side note - considering my image the balance lead port goes up to 24. Does that mean I could solder additional ports on in the future and connect a larger battery to it? Not that I would because my enclosure will only fit a 10s4p pack (future upgrade), but interesting to know!

Thanks,
Daniel
```

---
## \#2 Posted by: b264 Posted at: 2018-09-27T17:29:22.147Z Reads: 101

```
@fottaz you have a customer in need
```

---
## \#3 Posted by: fottaz Posted at: 2018-09-27T18:09:04.408Z Reads: 100

```
Hi Daniel! Thanks for your purchase. 

The 10s bms should be used with a 10s battery to be safe with all kind of automatic detections.
Anyway it's usable with a 9s too.

The balance leads are for a 10s and programmed for 10s max. I would suggest to avoid any modification.

The B- is the negative of your battery, the C- is for negative charge port and the P- goes to the negative LCD and XT60/90 or any connector you will use.

About the two white wires coming out, those are for the on off switch 

Alberto
```

---
## \#4 Posted by: MrDGOrman Posted at: 2018-09-27T19:04:26.775Z Reads: 91

```
@b264 @fottaz

Is it safe to say that the below is a suitable wiring diagram? For each cell in the battery pack I understand it needs to go in sync. That means finding out which cell comes first and which comes last, right? I presume I can do that with a voltage meter and the voltage will differ for each one. The smallest number is cell 1, the largest number is cell 3, and the remaining is cell 2. I would test this by placing a wire on the black balance lead and then going between each wire. Correct? Also, does it matter which way round the Sw/Fuse wire attaches to the on/off switch? And why is one called Sw and the other Fuse?

![BMS%20wiring%20diagram|520x500](upload://3b8GBhu1CTTbAGGZlfI2EVMDM8z.png) 

Thanks,
Daniel
```

---
## \#5 Posted by: MrDGOrman Posted at: 2018-09-28T00:05:45.102Z Reads: 78

```
@mmaner @Namasaki - could one of you potentially help me please? I saw you both commenting on other threads so hopefully you can help.

With a 9s setup is it correct I need to use a 37.8v charger?

I'm really nervous about getting this wrong :frowning_face::
```

---
## \#6 Posted by: mmaner Posted at: 2018-09-28T00:18:37.675Z Reads: 72

```
The max voltage for a li-ion cell is 4.2v, multiplied by 9 you have a max voltage of 37.8v.
```

---
## \#7 Posted by: Namasaki Posted at: 2018-09-28T00:36:12.680Z Reads: 72

```
[quote="MrDGOrman, post:5, topic:69376"]
With a 9s setup is it correct I need to use a 37.8v charger?
[/quote]


Yes you are correct
```

---
## \#8 Posted by: MrDGOrman Posted at: 2018-09-28T06:01:58.893Z Reads: 63

```
@mmaner @Namasaki - okay perfect. Is my wiring diagram that I posted above (not original post) correct?

Cheers,
Daniel
```

---
## \#9 Posted by: Namasaki Posted at: 2018-09-28T11:28:16.743Z Reads: 57

```
That bms will not work with a 9s battery. 
It will not turn on because of zero voltage at B10
Pin.
```

---
## \#10 Posted by: MrDGOrman Posted at: 2018-09-28T11:44:56.994Z Reads: 56

```
You're kidding? There's so many conflicting answers around here. Honestly I'm so frustrated if that's the case.

Some people say it'll work fine, others not. Is there a way to bypass it? People say to leave the last balance lead unplugged?
```

---
## \#11 Posted by: Namasaki Posted at: 2018-09-28T12:00:48.322Z Reads: 56

```
Some bms are designed for multiple configurations. 
This bms is designed specifically for 10s. 
It will detect a fault with only 9 cells. 
And it’s total values will be wrong as well.
```

---
## \#12 Posted by: MrDGOrman Posted at: 2018-09-28T12:04:58.089Z Reads: 57

```
Fantastic..

Any ideas what BMS I could use which will allow me to use 9s, 10s, 12s, etc. Multi configurations as you say?

All I want is to charge my batteries easily and have an on/off switch. I can't afford to pay out for Li-ion batteries at the moment so need to stick with my LiPos.

What about this one?
https://eskating.eu/product/12s-bestech-bms-80a-12s4p-5p/
```

---
## \#13 Posted by: pat.speed Posted at: 2018-09-28T12:11:39.227Z Reads: 54

```
Apparently all ‘Dumb’ bms modules will work with cells missing as long as it is the last one on the line. Well that’s what I’ve heard from @Deckoz and can confirm this myself with running a 12s battery on 13s bms. 

Although maybe this is a ‘smart’ bms? I don’t know, although the seller did say it will work so I would probably go with what he has said
```

---
## \#14 Posted by: MrDGOrman Posted at: 2018-09-28T12:22:13.809Z Reads: 55

```
This is one thing that I'm on the fence about. The seller (@fottaz) says it will work fine with 9s and in another thread @b264 agreed, however now there's conflicting opinions.

The last thing I want to do is plug it all together and something dangerous happens or the BMS explodes or something.
```

---
## \#15 Posted by: Namasaki Posted at: 2018-09-28T15:15:17.898Z Reads: 51

```
Theoretically it should not work but you can try it and the worst that will happen is the bms will shut down as soon as you turn it on. 
It is supposed to read 10 individual voltages and shut down if any of them fall below the low voltage detection value.
```

---
## \#16 Posted by: MrDGOrman Posted at: 2018-09-28T15:29:05.015Z Reads: 45

```
I'll give it a shot then I think. It won't cause the BMS to fail and be useless though, right? If it doesn't work I'll just upgrade my battery pack sooner rather than later. I wouldn't want to buy another BMS by running the risk of plugging my current setup in!
```

---
## \#17 Posted by: Namasaki Posted at: 2018-09-28T17:24:05.986Z Reads: 41

```
Not connecting the 10th cell will not damage the bms. It just won’t turn on theoretically.
```

---
## \#18 Posted by: MrDGOrman Posted at: 2018-09-28T17:37:18.173Z Reads: 40

```
Okay. I'll test it and see what happens!
```

---
## \#19 Posted by: b264 Posted at: 2018-09-28T18:19:46.125Z Reads: 40

```
[quote="Namasaki, post:17, topic:69376, full:true"]
Not connecting the 10th cell will not damage the bms. It just won’t turn on theoretically.
[/quote]

Just make sure the cell (or cells) that's disconnected is on the positive end
```

---
## \#20 Posted by: MrDGOrman Posted at: 2018-09-28T18:31:10.572Z Reads: 41

```
They're labelled B-, B1, B2 all the way to B10. I'll leave B10 alone?
```

---
## \#21 Posted by: Namasaki Posted at: 2018-09-28T20:31:40.048Z Reads: 43

```
Nice diagram btw.
```

---
## \#22 Posted by: pat.speed Posted at: 2018-09-28T21:00:57.976Z Reads: 43

```
Yep, leave off the last lead. I’m thinking it will work but you never know. 


Diagram looks good. If your adding a fuse though you might as well have the charge port fused as well. That way if anything is connected wrong or something gets in the plug the fuse will blow and not your battery. It’s not essential just my opinion
```

---
## \#23 Posted by: MrDGOrman Posted at: 2018-09-28T21:22:16.785Z Reads: 44

```
Makes sense. Based on my diagram I'll put the charging positive wire into the xt-90. Not literally, but you know what I mean.

I'll report back with my findings tomorrow 😁
```

---
## \#24 Posted by: MrDGOrman Posted at: 2018-10-03T20:09:20.610Z Reads: 44

```
Hi everyone,

Sorry about the delay in posting but I've only just been able to finish doing some of the wiring.

Okay so far I've wired everything up apart from the charging socket. Using my diagram above, the skateboard starts up when I turn on the switch. The FOCBOX works and everything happens as normal. I've only done a bench test so I'll be unable to tell what the cell voltages are like until I use it. The cells are currently full with power. I'll ride it for a little and then see what the cells are again.

However I feel the real testing will happen when I connect the charging port and attempt to charge it. I can't seem to find a charger suitable for 9 cells (37v?) that charges higher than the standard 2 amps. I want to get a quick charger of sorts that had an automatic cutting of when it reaches max voltage. If anyone has any suggestions on this then I'll be happy to hear them!

Question:
How do I wire the charging plug? There's 3 pins, I presume they're positive, negative and earth. How do I know which wire goes where? If I need to test it with a voltage meter, how would I do that? Please excuse the nooby question but I'm not great with a voltage meter!

Thanks,
Daniel

@Namasaki @pat.speed @fottaz @b264 @mmaner
```

---
## \#25 Posted by: mmaner Posted at: 2018-10-03T20:10:23.674Z Reads: 42

```
when you get a charger, plug it into the charge port and use a multimeter to define the pins.  You only need POS & NEG.
```

---
## \#26 Posted by: MrDGOrman Posted at: 2018-10-03T20:12:30.410Z Reads: 37

```
Perfect idea! I didn't think of that. Another noob question - what setting would I have it on and what method should I use to test it?

Also, any recommendations on a 37v charger which does fast charging? :thinking:
```

---
## \#27 Posted by: mmaner Posted at: 2018-10-03T20:18:52.485Z Reads: 44

```
Set the multimeter to DC 60a.  Be careful using a high amp charger, I would suggest getting a 2a to test with and then after the battery is proven (2 complete discharges and charges) get a 4a.  I never charge over 4a and mostly at 2a or 3a.

**37.8V 3A Li-ion Battery Charger Aluminum Case Charger For 9S 33.3V Li-ion Battery Smart Charger Auto-Stop Smart Tools**  
by WAOUKS 
**Link:**  http://a.co/d/iyHqJjD

**37.8V 4A Charger 33.3V Li-ion Battery Smart Charger 9S Red Aluminum shell With fan Battery pack charger Input 100VAC-240VAC**  
by WAOUKS 
**Link:**  http://a.co/d/iSykSVD
```

---
## \#28 Posted by: b264 Posted at: 2018-10-03T20:19:50.394Z Reads: 44

```
[quote="MrDGOrman, post:24, topic:69376"]
Question:
How do I wire the charging plug? There’s 3 pins, I presume they’re positive, negative and earth. How do I know which wire goes where? If I need to test it with a voltage meter, how would I do that? Please excuse the nooby question but I’m not great with a voltage meter!
[/quote]

Typically the 3 pins are

Ground (negative)
Charging (connected to negative when NOT charging, disconnected while charging)
Positive (positive)

Use a multimeter NO MATTER WHAT to verify though.
```

---
## \#29 Posted by: MrDGOrman Posted at: 2018-10-03T20:32:57.986Z Reads: 39

```
@mmaner I'll do as you suggest. A 3a charger should be okay for testing though, right? If I monitor it closely? Or should I not run the risk and get a 2a charger aswell? Thank you for a mini lesson on voltage meters :smile: 

 @b264 negative and positive are easy enough to wire up but how would I wire up the charging pin? Mmaner says the 3rd pin isn't required?
```

---
## \#30 Posted by: mmaner Posted at: 2018-10-03T20:50:37.652Z Reads: 41

```
I mean, your the one buying it so get what you want.  If it's not an affordability thing I would get a 2a and a 4a.  Use the 2a when your just sitting around and not in a hurry, use the 4a when you wanna charge fast.  By charging to 4.1v per cell and discharging to 3.5v per cell you more than double the possible charge cycles.

To be completely honest, I never do that.  I use a lab power supply to charge most of the time, at 3a and a brick charger when I'm not home and I only carry the 4a bricks with me.  That being said, I try to give my packs a decent burn in by charging with 2a the first few charge cycles.
```

---
## \#31 Posted by: mmaner Posted at: 2018-10-03T20:53:09.530Z Reads: 41

```
[quote="MrDGOrman, post:29, topic:69376"]
how would I wire up the charging pin
[/quote]

I don't...

![tmp_2018100315521285346|504x500](upload://wf9p96OjhbUf7VTAqrnNjn0AwRa.jpeg)
```

---
## \#32 Posted by: MrDGOrman Posted at: 2018-10-03T21:59:03.406Z Reads: 39

```
@mmaner cost isn't a huge concern of mine at the moment. I'll get a 2a and 4a charger. I work from home so I can have it plugged in while I'm working.

Thanks for the picture. Which one is positive and which is negative? My guessing is the 90° point is positive because the other two match, which would make sense for a negative and earth connection (or charging as @b264 said). Also, what awg cable is that? I've only got 12awg at the moment which seems a little overkill?
```

---
## \#33 Posted by: MrDGOrman Posted at: 2018-10-03T22:44:45.042Z Reads: 36

```
Oh, I just realised. 4a charging so atleast 4 amps!
```

---
## \#34 Posted by: mmaner Posted at: 2018-10-03T22:52:30.796Z Reads: 34

```
yep, the big lug/pin is the positive, but check with a multimeter just to be sure.
```

---
## \#35 Posted by: b264 Posted at: 2018-10-03T23:48:51.509Z Reads: 32

```
[quote="MrDGOrman, post:32, topic:69376"]
Which one is positive and which is negative?
[/quote]

You absolutely have to use a multimeter to check this, EVEN IF YOU KNOW.  It's not exactly negotiable or optional.  Lithium cells are essentially fire-in-a-bottle.
```

---
## \#36 Posted by: MrDGOrman Posted at: 2018-10-04T13:30:07.508Z Reads: 31

```
I tried to order that 3a charger but they can't send it to my address. I'm in the UK so I'm guessing that's why :frowning_face:
```

---
## \#37 Posted by: mmaner Posted at: 2018-10-04T16:43:10.479Z Reads: 32

```
That was just an example, check gear best or something.
```

---
## \#38 Posted by: pjotr47 Posted at: 2018-10-04T21:11:00.895Z Reads: 36

```
It will turn on and works, because the circuit of cell 10 is not closed
BUT the bms will cut the whole pack if it is lower then 3v*10=30v (Over discharge detection voltage)

A 9cell pack is empty when it is at 27v -> you can't use the whole capacity of the pack

So buy a 9s bms ;)
```

---
## \#39 Posted by: Namasaki Posted at: 2018-10-04T21:43:07.555Z Reads: 36

```
The only test that I did with this bms was that I connected the battery mains and not the balance wires and tried to turn the bms on. It would not turn on with the balance wires disconnected.
It was my understanding that this bms monitors individual cell voltages by the balance leads and shuts down if even one cell falls to 3v or what ever the detection voltage is set at.
```

---
## \#40 Posted by: pjotr47 Posted at: 2018-10-04T21:47:00.473Z Reads: 35

```
Yeah, I was thinking just the same but a friend from me use a 10s bestechpower bms with 8s battery and it works until it reach the over discharge detection voltage and then the bms cut the load.
```

---
## \#41 Posted by: Namasaki Posted at: 2018-10-04T23:32:09.568Z Reads: 30

```
I just tested the theory by disconnecting the balance wires from cells 9 and 10 on my 10s system and the bms still turned on.
This is very disappointing.
```

---
## \#42 Posted by: TowerCrisis Posted at: 2018-10-04T23:37:20.716Z Reads: 30

```
Can't say I'm surprised. Most BMS's don't have any electrical connection between the balance portion and the protection portion with mosfets, aside from maybe a common ground.

EDIT: what BMS are you using?
```

---
## \#43 Posted by: Namasaki Posted at: 2018-10-04T23:41:13.236Z Reads: 31

```
Bestech HCX-D223 10s
```

---
## \#44 Posted by: MrDGOrman Posted at: 2018-10-07T19:12:41.105Z Reads: 27

```
Small update to all:

I decided to contact Lucy and Henry at Bestech and they've confirmed that using this particular BMS with a 9s setup will be fine. All I had to do was join the B9 and B10 leads together, which I thought would be the case anyway.

I've not added the charging port just yet, but that's to come.

I've taken the board out for a quick spin and everything appears to work as expected however @b264, you're right - using a BMS for the charge and discharge can prevent the brakes from working due to over voltage features. I'm a little bit pissed off with this but then I guess you can't have one without the other. Does anyone have any recommendations on how to resolve this? I'd like to fully charge the board but not run the risk of having no brakes!

Cheers all,
Daniel
```

---
## \#45 Posted by: b264 Posted at: 2018-10-07T21:50:07.354Z Reads: 23

```
Try only charging to 4.15V per cell (37.35V) then.  The problem is to balance the cells you might need to charge to the full 4.20V per cell (37.8V) sometimes.
```

---
## \#46 Posted by: MrDGOrman Posted at: 2018-10-07T22:23:15.709Z Reads: 23

```
I thought that would be the case. Just wanted some confirmation on it that's all.

Thanks!
```

---

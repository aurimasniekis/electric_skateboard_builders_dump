# Pros &amp; Cons list to BMS

### Replies: 35 Views: 462

## \#1 Posted by: Schtekarsten Posted at: 2019-01-16T11:38:18.004Z Reads: 139

```
Would love to get some pointers regarding the best BMS for my application. I am set on discharging through the bms.
Space available 150mm x 80mm x 23mm
12s3p and Vesc 6's so 12s3p and dual 6374. so the 12s3p will be the weak link and I want to push it to its limits.
Im thinking of the following:

Fat Bestech 80A ish: http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D596.html
Pros:
High balancing current 126 mA something something
Integrated Anti-spark switch (just need a 12v latching button)
Can certainly handle the loads
Cons:
Super fat, nogo if it is 25mm tall (is 20mm or 25mm?)
Expensive
Board has to be turned on to charge? (which means I have to turn it off after it's fully charged every time? kinda want to just plug it in and leave until the next time I want to use the board and not have to think about it)
No breaks when fully charged? (is there a way to get around this?)

Bestech 50A: http://www.bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D452V1.html
Pros:
Oh that size and price
Comes with and integrated anti spark switch? (hopefully, maybe, idk, meh)
Cons:
Might see the magic smoke sooner or later cus of 50A...
Board has to be turned on to charge?
No breaks when fully charged?

Supower 60A: http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html
Pros:
Cheap ish
Can handle the loads with no problem
Comfortably fits my enclosure
Cons:
No brakes when fully charged
No integrated anti-spark switch (will need a ugly XT90S)

Uhm yeah. us new builders are, erm do have a tiny bit to learn! any pointers and feedback would be lovely!:smiley:
```

---
## \#2 Posted by: Andy87 Posted at: 2019-01-16T11:57:36.848Z Reads: 117

```
you will have no breaks with all 3 bms when fully charged.

[quote="Schtekarsten, post:1, topic:81046"]
is there a way to get around this?)
[/quote]
yes. don´t fully charge or bypass for discharge.
but bypassed the e-switch will not work.
```

---
## \#3 Posted by: Winfly Posted at: 2019-01-16T11:59:03.484Z Reads: 114

```
12s3p definitely on the small side if you are using VESC6's and dual 6374. If you are set on 3p only, you technically only need a 60A discharge bms (20A per cell unless you are gona beat the hell out of your 30Qs). I am a charge only guy, and from what I've seen, the D596 is the go to for a discharge bms. unless you can wait and pay for a DieBieMS.

Can I ask why only 3p? Personally I would just go with focboxes if you only have 3p. 3p doesnt have the power to utilize VESC6.

Also, yes if you use a discharge bms, it will cutoff when you brake at full battery.
```

---
## \#4 Posted by: totalgeek9224 Posted at: 2019-01-16T11:59:13.461Z Reads: 104

```
Maybe youd have room for the DieBieMS? Great bms if size+ price isn't an issue plus supports 80 a discharge
```

---
## \#5 Posted by: Schtekarsten Posted at: 2019-01-16T12:08:36.044Z Reads: 99

```
Uhm it's a space thing mostly and I am way to classy to have dubble stacked battery. and it's one of those Chinese ones that are cheaper then the focboxes. so :smiley:
But what you are saying is the power bill be lacking compared to a beefier battery? not just range? can't I just use the bull whip on the batteries I mean acceleration, short period you know. Continuous draw is it really that high?
```

---
## \#6 Posted by: Schtekarsten Posted at: 2019-01-16T12:09:32.729Z Reads: 94

```
Ohhh I'm cheap :smile:
```

---
## \#7 Posted by: Winfly Posted at: 2019-01-16T12:11:01.438Z Reads: 96

```
I wouldn't say power will be lacking but it will definitely wear out your cells quicker and more sag, which means shorter range.

Since you said you are new, I will list you the pros and cons of charge only:

Pros:
* Small form factor
* Cheaper
* No cutoff at full battery (hurt your battery better than hurt yourself)
* No current limit from your battery
* No extra heat lose from Mosfets on discharge
* still balance your pack at the end of charge cycle

Cons:
* Need to wire it up correctly for bypass
* no under voltage cutoff (can be handled by VESC)
* no immediate power cutoff when a group of cells dies. (you can also just keep an eye on sudden drop in battery capacity and catch it when your battery doesnt charge fully)
* No E-switch
```

---
## \#8 Posted by: Andy87 Posted at: 2019-01-16T12:11:56.419Z Reads: 85

```
maybe something like this would be an option too
https://bmsbattery.com/bmspcm/833-smart-bms-10s13s-60a-with-blue-tooth-android-or-ios-app.html
```

---
## \#9 Posted by: Schtekarsten Posted at: 2019-01-16T12:12:44.010Z Reads: 82

```
I wont bypass. friends might get hold of it down the road and y leaving it on for the weekend = angry friend..
Is it enough to just lower end of charge from the factory and still use a 4.2 volt per cell charger or do I need a special charger aswell or just the charger? hum...
```

---
## \#10 Posted by: Andy87 Posted at: 2019-01-16T12:13:24.049Z Reads: 78

```
i would add, no e-switch
```

---
## \#11 Posted by: Winfly Posted at: 2019-01-16T12:15:38.660Z Reads: 76

```
what deck and enclosure are you thinking? it won't fit a 4p?
```

---
## \#12 Posted by: Andy87 Posted at: 2019-01-16T12:15:48.579Z Reads: 75

```
if you set down the over voltage limit to let´s just say 4.1V for example, the bms will only let you charge till 4.1V and again you have the same problem.
if you drive with a cell voltage of 4.1V and break your bms think you charge and want to overcharge the cell and switch of because of it.
```

---
## \#13 Posted by: Winfly Posted at: 2019-01-16T12:17:20.863Z Reads: 70

```
one way to get around it is to use a buck converter in between your charger and charge port to trim the charger voltage down to 4.1V per cell.
```

---
## \#14 Posted by: Andy87 Posted at: 2019-01-16T12:17:58.307Z Reads: 66

```
yes, but than it may be that your bms will never ever start to balance.
```

---
## \#15 Posted by: Winfly Posted at: 2019-01-16T12:19:38.800Z Reads: 68

```
that's not necessarily true.
```

---
## \#16 Posted by: Schtekarsten Posted at: 2019-01-16T12:19:40.159Z Reads: 68

```
ah it's a home brew carbon fiber resin infusion deal with 6 compartments. single layer 4 compartments a 9 batteries each. one for bms and one for the vescs. I go diagonal aswell on the motors so it's tight
```

---
## \#17 Posted by: Andy87 Posted at: 2019-01-16T12:20:35.789Z Reads: 67

```
depending on how your bms works.
if your bms first overcharge one cell and than drain it is.
```

---
## \#18 Posted by: Schtekarsten Posted at: 2019-01-16T12:22:57.876Z Reads: 70

```
Is that the how the big boys does it or. seems complimecated
```

---
## \#19 Posted by: Winfly Posted at: 2019-01-16T12:23:41.369Z Reads: 70

```
or you can get a variable voltage charger.
```

---
## \#20 Posted by: Schtekarsten Posted at: 2019-01-16T12:26:00.317Z Reads: 65

```
that thing looks dope, sadly im in Europe though. uhm. but can't you get the same stuff in a preprogramed bms though just have the factory set it and forget it?
```

---
## \#21 Posted by: Schtekarsten Posted at: 2019-01-16T12:27:16.863Z Reads: 56

```
y but isn't balancing a problemo then and expensive, remember im dumb and cheap.
```

---
## \#22 Posted by: Andy87 Posted at: 2019-01-16T12:28:50.993Z Reads: 56

```
you can get it from AliExpress or other sources too.
The link was just an example.
If you don´t change any settings the factory settings will work all time.
but than you can also just get a usual bms from bestech.

just linked as i think it´s a cheap way inbetween a usual bms and the DieBieMS.
```

---
## \#23 Posted by: Schtekarsten Posted at: 2019-01-16T12:36:49.570Z Reads: 56

```
Okay okay. i have a few fears (feers ferries?) when it comes to bmses. 
1 Shipping government, fine, jail when selling bypassed stuff down the road. 
2 killing the pack if left powered on for a few days
3 blowing up in my face

discharge through bms
1 stupid brakes
2 having to remember to keep the board on to charge and turn off after fully charged every single time
```

---
## \#24 Posted by: Winfly Posted at: 2019-01-16T12:38:42.615Z Reads: 53

```
Voltage step down with buck is actually pretty easy. just use a pair of plugs so you can take off the buck once in a while for balance.
```

---
## \#25 Posted by: Andy87 Posted at: 2019-01-16T12:40:30.504Z Reads: 58

```
[quote="Schtekarsten, post:23, topic:81046"]
1 Shipping government, fine, jail when selling bypassed stuff down the road.
[/quote]

? 😂
It’s not like you chip crack your PlayStation in the late 90s.

You buy a normal bms just wire it up to your needs.
```

---
## \#26 Posted by: Schtekarsten Posted at: 2019-01-16T12:42:41.408Z Reads: 52

```
y maybe just maybe could learn how to do stuff like that but I want an idiot. no baby proof board
```

---
## \#27 Posted by: Winfly Posted at: 2019-01-16T12:45:00.727Z Reads: 53

```
ok. I guess a Bestech bms would be the easiest for you. you just need to be careful about going down a hill when it's full charged. learn how to foot brake just in case.
```

---
## \#28 Posted by: Schtekarsten Posted at: 2019-01-16T12:54:14.728Z Reads: 51

```
Sorry but living on a hill my friend I'm currently consuming twice as many shoes as I used to do with that setup... even flipflops can't really take it.
as well as the on/off charge thing is annoying with a switch. (using xt90s atm)

would love to bypass but leaving the board on for the weekend thing just doesn't cut it.
as well as shipping issues and government jazz keeps me from doing it.
how do the big boy brands and the posh ladies in pink high-heels do it? :dancer:
```

---
## \#29 Posted by: Andy87 Posted at: 2019-01-16T14:02:00.945Z Reads: 48

```
[quote="Schtekarsten, post:28, topic:81046"]
as well as shipping issues and government jazz keeps me from doing it.
[/quote]

What you mean with it?
```

---
## \#30 Posted by: Schtekarsten Posted at: 2019-01-16T14:04:55.017Z Reads: 45

```
im mean isn't there rules and stuff that you need to have a short circuit protection for batteris and that kind of stuff and you can't just throw it in a box and ship it with DHL like it was a box of flowers.
```

---
## \#31 Posted by: Andy87 Posted at: 2019-01-16T14:08:43.463Z Reads: 43

```
You can ship every battery as long as it’s local and ground service.
Doesn’t matter what protection you have.
How you think single cells are shipped?

What you can’t, ship them via plane.
But that you can’t with any battery as long as it’s not integrated in a full product (like laptop) or you have a special certification.
You can take batteries till a specific size into your hand luggage, but again this doesn’t depends if there is a bms inside or not.
```

---
## \#32 Posted by: Schtekarsten Posted at: 2019-01-16T14:12:31.486Z Reads: 41

```
Cheers for that!
Awesome thanks!
But aren't there standards aswell when selling electronics that basically tells you to have a fully functional BMS connected to your pack
```

---
## \#33 Posted by: Andy87 Posted at: 2019-01-16T14:14:00.317Z Reads: 45

```
I don’t know if any.
Theoretically nobody makes you to use a bms at all.

Most of the rc cars and planes don’t use a bms.
They use a balance charger for the lipo packs, but the pack by it’s own doesn’t have a protection usually.
```

---
## \#34 Posted by: Schtekarsten Posted at: 2019-01-16T14:18:06.589Z Reads: 45

```
Smart man!
did not think of that! interesting :smiley:
```

---
## \#35 Posted by: mynamesmatt Posted at: 2019-01-17T02:09:23.628Z Reads: 30

```
Just saying, it's really easy with the whole switching on the system to charge. you plug in the board and turn it on. then when full, you turn it off and unplug it.? really isn't that hard. also, if you live on a hill like me, just gun it up the hill when you ride it. so gun it up the hill, then coast down, brake quick turn around and gun it again. Discharges the pack just enough to have brakes lol
```

---

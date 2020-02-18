# First longboard build parts list - will it work for what I want?

### Replies: 18 Views: 581

## \#1 Posted by: cjpanici Posted at: 2018-05-04T14:57:25.060Z Reads: 81

```
This is my first esk8 build. Please have a look at my parts list to see if there's anything I am missing:
What I want: I want something that has decent acceleration for my weight (200lb). I want something that can go about 20mph and has good range (10 mi). Don't really have a lot of steep hills around so I am not worried about losing speed when going uphill. Here's what I've got for a parts list so far - haven't bought anything but the deck.

1. 9-ply maple 39x10 longboard deck
2. caliber II 50 degree trucks - are these wide enough for a dual rear drive setup?
3. 90mm flywheels
4. Dual turnigy aerodrive sk3 6354 motors 260kV - will these fit on my rear truck without modification?
5. riser pads - maybe get the 1" and file them down to get desired clearance?
6. DIYE electric skateboard motor mount caliber II truck compatible
7. Michobby dual vesc 150a w/ canBUS cable - Any experience with this particular setup?
8. Two 6S 5000mAh 50C battery wired in series for 12S
9. 12mm motor pully and 3 or 4 to 1 gear ratio. Any good retail ones that would work for my setup?
10. Misc. parts & connectors.
11. 12AWG wire for electric drive system
12. Kill switch

I appreciate any feedback you can give me!

cj
```

---
## \#2 Posted by: cjpanici Posted at: 2018-05-04T15:01:01.851Z Reads: 72

```
I will also get a remote and receiver for the vesc, just don't know which one yet. That is minor though.
```

---
## \#3 Posted by: moon Posted at: 2018-05-04T15:04:10.827Z Reads: 67

```
Those trucks are fine

Pretty sure that diyeboard don't have motor mounts for caliber trucks
```

---
## \#4 Posted by: linsus Posted at: 2018-05-04T15:16:21.089Z Reads: 64

```
[quote="cjpanici, post:1, topic:54382"]
260kV
[/quote]
I'd say lower kV.

[quote="cjpanici, post:1, topic:54382"]
Michobby
[/quote]
The what, who now?
[quote="cjpanici, post:1, topic:54382"]
5000mAh
[/quote]
For 15km range? It's doable if riding on flat. You wont have alot more then that tho.

Wheres the charger?
Get a proper helmet atleast.
enclosure?
Also, personally I'd take a single SK3 6374 over dual 6354 setup.
```

---
## \#5 Posted by: cjpanici Posted at: 2018-05-04T15:35:19.820Z Reads: 57

```
Thanks for the feedback. Can you suggest one that will fit?
```

---
## \#6 Posted by: cjpanici Posted at: 2018-05-04T15:44:24.985Z Reads: 59

```
Hey Linsus thanks for the feedback.

Sorry, the VESC is made by Vedder, Michobby sells it here:
http://www.michobby.com/product/vedder-vesc-speed-controller/

I thought having the dual motor setup would give me some more acceleration and still get higher speeds, am I wrong? Can I go with a bigger dual motor setup with wider trucks?

If I can fit another 6s battery or two on there I will for longer range.

I have a proper helmet already. For the enclosure I will look for one that will fit my needs and if I can't find one I will vacuum form it out of kydex or make one out of carbon fiber.
```

---
## \#7 Posted by: cjpanici Posted at: 2018-05-04T15:46:22.066Z Reads: 53

```
Dual setup is on sale right now:
http://www.michobby.com/product/dual-vesc-with-2-vescs-and-1-canbus-connector/
```

---
## \#8 Posted by: moon Posted at: 2018-05-04T15:49:33.438Z Reads: 53

```
Where are you located
```

---
## \#9 Posted by: cjpanici Posted at: 2018-05-04T15:51:44.849Z Reads: 46

```
I am in Wisconsin. So I ride in the burbs and am sick of pushing :-)
```

---
## \#10 Posted by: pennyboard Posted at: 2018-05-04T15:53:10.893Z Reads: 46

```
You’d be better off paying the extra $17 and getting 2 VESC from diyelectric skateboard. I know those aren’t the most robust VESC, but I’m willing to be bet that they’re a lot better than Mic Hobby, given I’ve never heard of them, and I’m skeptical as to whether they can handle 12s voltage
```

---
## \#11 Posted by: pennyboard Posted at: 2018-05-04T15:55:24.731Z Reads: 42

```
Also, I’d recommend getting the TB 218mm trucks and @marcmt88 motor mounts. The turnigy 6354’s a little larger than conventional 6354s and with those larger 218mm trucks, you won’t be pressed for space.
```

---
## \#12 Posted by: TehAtheist Posted at: 2018-05-04T16:02:37.221Z Reads: 38

```
  Lower the KV of your motor, you're above the 60000 ERPM (limit for the VESC you'll use) and although possible, it's not recommended. With 1:3 gear ratio you could achieve 65km/h which in al honesty, is simply mindbogglingly fast. 

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:12,%22motor-kv%22:260,%22system-efficiency%22:85,%22motor-pulley-teeth%22:10,%22wheel-pulley-teeth%22:30,%22wheel-size%22:96}|

That's your current setup, I recommend not to go higher than this:

http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:12,%22motor-kv%22:190,%22system-efficiency%22:85,%22motor-pulley-teeth%22:14,%22wheel-pulley-teeth%22:36,%22wheel-size%22:96}|

Play around with the gear ratio along with what kits you find or how you'll make it yourself.
```

---
## \#13 Posted by: briman05 Posted at: 2018-05-04T16:13:16.839Z Reads: 34

```
I dont think you would need 1 inch risers that is fucking high.  On all my custom boards I do 1/4 or 1/8
```

---
## \#14 Posted by: linsus Posted at: 2018-05-04T16:25:31.904Z Reads: 34

```
[quote="cjpanici, post:6, topic:54382"]
Sorry, the VESC is made by Vedder, Michobby sells it here:
[/quote]

First off all, yes the hardware design is vedders, the software is vedders. That esc on the Picture is not made by vedder but by "mic hobby", quality of which i know 0 about. 

[quote="cjpanici, post:6, topic:54382"]
am I wrong?
[/quote]

Speed depends on more factors then the amount of motors. F.e voltage*kv=rpm of motor(roughly) - > gearing to Wheel-> top rpm of  90mm Wheel -> translate to km/h. Its a pretty accurate way of calculating the speed. 

My first board was a single motor build with one 6374 on 10s. I shat my pants several times learning to ride Electric with that setup, berly ever pushing it to the speedlimit nor having any problems whatsoever with hills. Later tried dual 6374. The term "action stance" comes to mind when trying to cope with the torque that board gave. no way you'd pull moderate throttle and still be on it if you werent fully ready for it.
```

---
## \#15 Posted by: cjpanici Posted at: 2018-05-04T17:42:32.784Z Reads: 28

```
Guys, I appreciate your input - you're truly awesome. You've convinced me to do the following:

Start with a single motor 6374 190kV setup
I am still going to go with the 12S battery
Do a 3:1 gear ratio
Spend the extra money on the diyelectric skateboard VESC
Get the wider 218mm trucks
Hit up that dude for the motor mounts

This gets me a good start and plenty of things to play with to get more speed if I even need it. I don't think I need to be going 30MPH right out of the gate.

Thanks again,
cj
```

---
## \#16 Posted by: linsus Posted at: 2018-05-04T17:48:20.677Z Reads: 28

```
If i remember correctly i had 34:14 theeths. roughly 2.4 ratio.
Sudgestion would be to buy one or two of the motor pulley with different amounts of teeths to find just right ratio for you.

Bought the pulleys and belts off http://esk8.de/.  Used keggels for Wheels.
```

---
## \#17 Posted by: FredrikHems Posted at: 2018-05-04T18:16:38.407Z Reads: 30

```
[quote="linsus, post:4, topic:54382"]
5000mAh

For 15km range? It’s doable if riding on flat. You wont have alot more then that tho.
[/quote]

Uhm.. Thats 220Wh. Which equals to around 20-25km of range. 15km shouldnt be a problem at all...
```

---
## \#18 Posted by: linsus Posted at: 2018-05-04T18:46:17.877Z Reads: 30

```
[quote="FredrikHems, post:17, topic:54382"]
Uhm… Thats 220Wh. Which equals to around 20-25km of range. 15km shouldnt be a problem at all…
[/quote]

Yes. Like i said, its doable. The flat remark was due to him mentioning he had no hills.
```

---

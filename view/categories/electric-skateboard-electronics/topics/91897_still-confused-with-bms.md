# Still confused with bms:(

### Replies: 36 Views: 231

## \#1 Posted by: konstantinos Posted at: 2019-04-27T02:19:02.368Z Reads: 59

```
Hi this is my second post about bms and i am still as confused as i was...I am planing to build my board in the future but i am stuck with choosing my bms.I will be running my board on 2 6s lipo 20000mah 12c 24cmax batteries in series.2 6384 170 kv 80a motors and for the vesc the focbox unity.What i don't understand is how many amps my bms must be...I am happy to read all your answers:)
```

---
## \#2 Posted by: Jcullinan09 Posted at: 2019-04-27T02:23:38.150Z Reads: 57

```
I'm assuming you're using Li-Po's but could you post a link to the specific batteries you'll be getting?
```

---
## \#3 Posted by: konstantinos Posted at: 2019-04-27T02:25:07.528Z Reads: 57

```
Yes sure

https://hobbyking.com/en_us/turnigy-high-capacity-battery-20000mah-6s-12c-drone-lipo-pack-xt90.html?wrh_pdp=7
```

---
## \#4 Posted by: AdamE3399 Posted at: 2019-04-27T02:26:05.987Z Reads: 53

```
If you discharging through the bms its best to have something that can handle the current youll be sending through it so something like 80 amps or higher should be fine
```

---
## \#5 Posted by: konstantinos Posted at: 2019-04-27T02:29:00.414Z Reads: 45

```
I was planning on getting this but seems like i need a bigger one:(
https://miamielectricboards.com/shop-1/12s-bms
```

---
## \#6 Posted by: Aleks1 Posted at: 2019-04-27T02:31:35.147Z Reads: 36

```
Well, ur battery's max amp discharging is Ah x c (20 x 12) = 240
But this is max discharge, usually it's better to use half what you have to make it last longer.
So basically u have 120 "safe" amps.
What I would do is buy 200 amp bms, because you have 2 x 80 amp motors, which is total is 160amp.
```

---
## \#7 Posted by: Aleks1 Posted at: 2019-04-27T02:33:24.543Z Reads: 35

```
Also I think it would be safe to use 160 amp from battery, because you only will be using it in very peak situations, which will happen very rarely.
But see what other people say, bc I'm not a big geek in it.👍
```

---
## \#8 Posted by: konstantinos Posted at: 2019-04-27T02:35:50.005Z Reads: 35

```
Sounds good.can u suggest me a good bms?
```

---
## \#9 Posted by: AdamE3399 Posted at: 2019-04-27T02:36:07.858Z Reads: 32

```
I agree with @Aleks1
```

---
## \#10 Posted by: Aleks1 Posted at: 2019-04-27T02:37:02.825Z Reads: 31

```
the problem is that 200amp bms is gonna be big, if it's not a mountain board
```

---
## \#11 Posted by: konstantinos Posted at: 2019-04-27T02:37:43.229Z Reads: 32

```
It is a mountain board;)
```

---
## \#12 Posted by: Aleks1 Posted at: 2019-04-27T02:37:44.446Z Reads: 39

```
people say Bestech BMS are good, and also I use Bestech but mine is 12s 80amp
```

---
## \#13 Posted by: JLabs Posted at: 2019-04-27T02:37:46.143Z Reads: 38

```
https://buildkitboards.com/products/bestech-bms
https://buildkitboards.com/products/bestech-d140-charge-only-bms
```

---
## \#14 Posted by: Aleks1 Posted at: 2019-04-27T02:39:59.544Z Reads: 36

```
he needs 200amp
```

---
## \#15 Posted by: konstantinos Posted at: 2019-04-27T02:41:14.953Z Reads: 36

```
Thats what i was gona say:D
I cant find any bms with more than 100amps:(((
```

---
## \#16 Posted by: JLabs Posted at: 2019-04-27T02:43:14.071Z Reads: 37

```
You can’t run 100-200 amps through 12awg wire constantly. Your likely barely ever to pull 80A on an eSk8. Constant will be much less, less than 20a. 

You can bypass with the D140 I linked, or get the 80A with eSwitch
```

---
## \#17 Posted by: Aleks1 Posted at: 2019-04-27T02:45:38.815Z Reads: 37

```
but the idea of 2 80amp motors was strange in the beginning)
```

---
## \#18 Posted by: JLabs Posted at: 2019-04-27T02:47:52.240Z Reads: 39

```
They dont draw 80A constantly, thats just their peak power. 

Same with the batteries... if you discharged them at their max rate you would barely be able to ride. You can limit the battery amps in the VESC tool, just do that and get an 80A BMS or D140 and dont worry about the discharging.
```

---
## \#19 Posted by: konstantinos Posted at: 2019-04-27T02:49:59.286Z Reads: 37

```
Ok lets say i go with the 80a bms with the switch how do i conect it if there is no dischsrge?
```

---
## \#20 Posted by: Aleks1 Posted at: 2019-04-27T02:50:07.855Z Reads: 36

```
his bat max is 240 amp, pretty sure he can use 160amp sometimes with no harm for bat
```

---
## \#21 Posted by: AdamE3399 Posted at: 2019-04-27T02:50:33.137Z Reads: 34

```
I know that the battery can give out 200 amps but relisticly it will be like 20 amps constant, even though the bms is an 80 amp bms it also has a higher burst rating so it will be fine
```

---
## \#22 Posted by: konstantinos Posted at: 2019-04-27T02:52:07.533Z Reads: 34

```
So we end up with the 80a bms?also can a get any bms with 80a or just charge 80a?
```

---
## \#23 Posted by: JLabs Posted at: 2019-04-27T02:56:13.576Z Reads: 34

```
What VESC lets you pull 160A?

@Kostkolama you just wire it like in the wiring diagram (80A D223 version)

If you want to bypass the discharge and not have a switch you buy the D140 version. You wire it like in the photo, but add another wire from B- to your XT60 connector (like the B+ wire).
```

---
## \#24 Posted by: konstantinos Posted at: 2019-04-27T02:58:08.821Z Reads: 34

```
Sounds great:)
```

---
## \#25 Posted by: konstantinos Posted at: 2019-04-27T02:59:57.180Z Reads: 32

```
I want to thank everyone that helped me understand what's going on with bms it really helped!!
```

---
## \#26 Posted by: J0ker3366 Posted at: 2019-04-27T03:01:30.067Z Reads: 31

```
Why not just bypass discharge and run a charge only bms?

Edit: now i see jlabs suggests it lol
```

---
## \#27 Posted by: konstantinos Posted at: 2019-04-27T03:05:48.419Z Reads: 30

```
Thats what i am going to do.Or at least try:D
```

---
## \#28 Posted by: deucesdown Posted at: 2019-04-27T03:09:10.810Z Reads: 31

```
Please pay attention to get a BMS for lipo not lithium ion. cutoffs are different.

Are you ready for huge power? lol. Guys on endless sphere seem to like these. The plus size cousin of the smart bms that's starting to get popular here. Different software, so it's completely different sutff.

https://www.aliexpress.com/store/product/Smart-Display-300A-8-24S-Cells-Lithium-Battery-Protection-Board-Balance-BMS-Coulomb-Meter-Lithium-iron/2856009_32827394534.html
```

---
## \#29 Posted by: konstantinos Posted at: 2019-04-27T03:14:16.925Z Reads: 30

```
I will never be able to setup something like this
```

---
## \#30 Posted by: J0ker3366 Posted at: 2019-04-27T03:14:55.914Z Reads: 30

```
[quote="deucesdown, post:28, topic:91897"]
cutoffs are different
[/quote]

Correct. But if youre using vesc cutoffs, it doesnt matter what you use. Vesc can cut it before the bms.
```

---
## \#31 Posted by: konstantinos Posted at: 2019-04-27T03:18:56.826Z Reads: 30

```
Is this bms going to work?
https://alienpowersystem.com/shop/bms/battery-bms-with-switch-for-12s-lipo-battery-l16s50/
I am aksing because there are not ehough info there
```

---
## \#32 Posted by: J0ker3366 Posted at: 2019-04-27T03:19:01.199Z Reads: 29

```
[quote="konstantinos, post:29, topic:91897, full:true"]
I will never be able to setup something like this
[/quote]

Im saying not saying i know as most of the pros on here, but ive put in my work to know the stuff i know. Starting out, i was the same way you feel. Once i had all the components in hand and could physically see where these connected, it became easy and the "fear" went away. Now, do i still get erky when doing the simplest things (plugging up my battery which is about 9 connections)? Fuck yes lol. But paying attention to what youre doing and taking your time is key
```

---
## \#33 Posted by: konstantinos Posted at: 2019-04-27T03:21:47.353Z Reads: 26

```
One of the best answers so far...i really dont know what to answer here xd.
```

---
## \#34 Posted by: konstantinos Posted at: 2019-04-27T03:23:32.040Z Reads: 26

```
Lol just found the info XDXD
```

---
## \#35 Posted by: deucesdown Posted at: 2019-04-27T03:36:29.290Z Reads: 27

```
The thing with the power system on diy high power electric skateboards is, you've got to understand everything. It's a huge mountain to climb, but you've got to climb if you want to play. At least so you can not cause fire, and repair things when (not if) they break.

Take it step by step and be prepared to have a box full of fried components as you learn. :slight_smile:
```

---
## \#36 Posted by: konstantinos Posted at: 2019-04-27T03:38:39.468Z Reads: 26

```
Fried conponents sound good but when we talk about electric skateboards its bad so i will be carefull not to burn anything
```

---

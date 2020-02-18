# Need your advice on upgrading to vesc

### Replies: 24 Views: 363

## \#1 Posted by: sanderfu Posted at: 2018-12-14T13:29:39.522Z Reads: 120

```
I am currently on a Diyeboard ESC and Battery combo, strongly considering upgrading the esc to vesc to use the firefly remote im building and get a better ride.

What I am wondeirng is if the battery or the esc is the ture bottleneck of the diyeboard kit, can someone make that clear for me?

Also, I am going to buy cheap flipskys if my esc is the bottleneck, because on a student budget, focboxes are just to damn expensive! ;) If anyone advice strongly against buying them from aliexpress instead of flipsky.net (will save me 50usd in total at least for two) then please say something to stop me from beeing stupid!
[Link to the flipsky I'm considering](https://www.aliexpress.com/item/FLIPSKY-FSESC-50A-V4-12-Multi-purpose-ESC-Electronic-Speed-Control-for-Electric-Skateboard-RC-Car/32916597684.html?spm=2114.search0104.3.9.75591db8jBfb9D&ws_ab_test=searchweb0_0,searchweb201602_5_10065_10068_319_10059_10884_317_10887_10696_100031_321_322_10084_453_10083_454_10103_10618_10307_538_537_536,searchweb201603_51,ppcSwitch_0&algo_expid=31cd60b7-2c44-4c7e-96e9-2a5f9feda5ac-1&algo_pvid=31cd60b7-2c44-4c7e-96e9-2a5f9feda5ac)

Thank you for your input!
```

---
## \#2 Posted by: DeathCookies Posted at: 2018-12-14T13:41:21.833Z Reads: 110

```
I dont answer your question about the bottleneck. But i will give you an Argument for a vesc.

If you have the same setup except different Escs it does Not matter where the bottleneck is. The only thing you are changing is the control behaviour of the Motor. You could easily destroy your battery with hardcore settings but if you Start gently you will be fine. So i would recommend a vesc because you can configure more
```

---
## \#3 Posted by: sanderfu Posted at: 2018-12-14T13:54:44.356Z Reads: 100

```
Thank you and I agree, but I actually like the raw untamed-ness of the china-direct esc, but I would like to maximize performance (to what my battery can take of course) and maybe get some less deathly breaking as I live in hilly Norway.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-14T13:54:53.722Z Reads: 92

```
[quote="sanderfu, post:1, topic:78003"]
am wondeirng is if the battery or the esc is the ture bottleneck of the diyeboard kit
[/quote]

That depends on your battery.
We don’t know which battery you have so nobody can say what’s the bottle neck.

But you can think about that by your own.
If the battery max output current is higher than what the vesc can max handle continues than the esc is the weak part.
If it’s other way round it’s other way round 😅
```

---
## \#5 Posted by: sanderfu Posted at: 2018-12-14T13:55:40.997Z Reads: 86

```
Hmm, its the 10s5p pack from Diyeboard (should have mentioned that at least). I am not sure about the cells, but I am sure someone else on the forum knows, will check.
```

---
## \#6 Posted by: Tinp123 Posted at: 2018-12-14T13:55:54.152Z Reads: 86

```
diyeboard uses bad cells in their batteries, and there is where you could get bottleneck. Do you have 10s5p or 10s2p? 
You could use those batteries with conservative settings, max 10 amp per parallel group. that means, for 5p battery, 50 amp max (25 amp per vesc if you have dual), for 2p battery, 20 amp max (10 amp per vesc) - those are really low settings. 
another big problem with those batteries is voltage sag, and lower maximum capacity under higher loads. 
10s3p of samsung 30Q cells will beat diyeboard 10s5p any day, both in power and in range. 
you can order from aliexpress, they have cheap or free shipping and you will get exactly same vesc like from flipsky. I did it too.
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-14T13:56:43.175Z Reads: 84

```
Maybe you can link your battery and your esc?
```

---
## \#8 Posted by: sanderfu Posted at: 2018-12-14T14:03:13.268Z Reads: 83

```
@Andy87 

Sure, know that Diyeboard is a bit controversial here on the forum after all that has happened so these links are merely for research and I would not recommend anyone reading this thread now or ever buy from Diyeboard as they are not to be trusted!

Battery: http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-with-charger-p-655.html

ESC: http://www.diyeboard.com/upgraded-v21-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-599.html

@Tinp123
I know, but I fell for the cheap option when buying last spring and I want to make the best of what I have for this build (and do better on the next one).

Do any of you know if I could be better off using 1 motor with a vesc with this battery and get almost as good performance as with dual? I have two 6355 motors from @JLabs so I guess that one might would be strong enough for me really (Weight~68 kg but quite hilly though).
```

---
## \#9 Posted by: DeathCookies Posted at: 2018-12-14T14:11:02.558Z Reads: 76

```
Rather go dual if you can afford it. I remember when i braked with a Single too hard and my Board just went to the side as one wheel blocked ... That throw me off the Board.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-12-14T14:11:22.512Z Reads: 77

```
Ok so i still can’t really help because I can’t see in the description which cells they use and if the esc is ready for 50a for both motors or for one.

With the vesc you want to order you can get about 35a continues out of.
If you have the opportunity I would always go with dual drive. That’s just less load on the esc the motors and the drive train
```

---
## \#11 Posted by: Deodand Posted at: 2018-12-14T16:31:39.655Z Reads: 65

```
[quote="sanderfu, post:1, topic:78003"]
Also, I am going to buy cheap flipskys
[/quote]

[quote="sanderfu, post:8, topic:78003"]
I know, but I fell for the cheap option when buying last spring
[/quote]

How much are you planning on spending for the flipsky ESCs? Keep in mind you will also have to buy\make some sort of power switch I think. I've heard a few people on this forum having troubles with the cheaper flipsky offerings. 

I'd wait a couple days and take a look at the focbox unity price :slight_smile:
```

---
## \#12 Posted by: nuttyjeff Posted at: 2018-12-14T17:39:14.191Z Reads: 57

```
Ohhhh is this a hint, is there going to be another sale?

[quote="Deodand, post:11, topic:78003"]
I’d wait a couple days and take a look at the focbox unity price :slight_smile:
[/quote]
```

---
## \#13 Posted by: briman05 Posted at: 2018-12-14T17:41:29.435Z Reads: 52

```
Maybe they didnt sell as many as they had hoped they would black friday with there deal on the raptor hubs? Now they have an over abundance
```

---
## \#14 Posted by: dareno Posted at: 2018-12-14T18:45:30.555Z Reads: 48

```
Upgrade the battery as well as the esc.  If you pop a unity in there and try to up the current the bms will die.  Trust me on this lol.  Those esc's are only rated to max of 18amps per motor.  The bms will pop if you try to run at anything over 20.  Been there done that.  The battery is the main issue with the diye stuff.
Get a decent 30q or equivalent pack and slap a unity in there and the motors will be completely transformed.  I have a focbox powered 10s 4p diye hub board that is a little demon.  Lots of fun.
```

---
## \#15 Posted by: Deodand Posted at: 2018-12-14T19:22:21.978Z Reads: 44

```
You could also bypass the bms and set it up charge only l.
```

---
## \#16 Posted by: dareno Posted at: 2018-12-14T19:24:07.547Z Reads: 43

```
Honestly jeff its really not worth the effort.  Terrible cells.  Truly terrible.
```

---
## \#17 Posted by: Deodand Posted at: 2018-12-14T19:25:21.796Z Reads: 42

```
Yeah no experience with this product :slight_smile:
```

---
## \#18 Posted by: dareno Posted at: 2018-12-14T19:30:59.144Z Reads: 41

```
You can get some juice out of the hubs though.  Had mine up to 80 motor amps for a bit and they had a fair bit of grunt but got a bit warm so dropped them back down.  Waiting for the silly season to be over then grab me a unity.
```

---
## \#19 Posted by: sanderfu Posted at: 2018-12-14T21:46:42.610Z Reads: 40

```
That is some serioua great feedback in this thread!

@dareno I know the pack sucks but it honestly works OK for me with the setup I have now, but thanks for the info on the bms, I was unaware of that limitation.  

I have seen so many different estimates on how much the escs draw and how much the pack can take, it would be awesome if someone has tested this or has a source for the info! I still think flipskys are ok for my budget, but will of course be on the lookout for good deals!
```

---
## \#20 Posted by: sanderfu Posted at: 2018-12-24T12:28:53.070Z Reads: 35

```
Another question on christmas eve itself, does anyone have mounting/heatsink advice for the flipsky 4.12?

I was considering using the flipsky massive heatsink, but it wont fit in my diyeboard 10s5p-enclosure

Any experience or ideas regafding this will be greatly appreciated!

Merry christmas to you all! :santa:
```

---
## \#21 Posted by: sanderfu Posted at: 2019-01-23T19:55:51.108Z Reads: 27

```
Okay so Im back and I have bought some stuff and need some more input:

Does anyone know how high current I can draw from the diyeboard 10s5p battery without killing the BMS and also how high charge current I can put into the battery. Just wondering since I am setting up my new vescs and I dont want to immediately ruin the battery. @dareno what settings did you have when you messed up the BMS? 

Thanks for any and all input on this!
```

---
## \#22 Posted by: epss4 Posted at: 2019-01-23T21:19:37.762Z Reads: 22

```
They told me 50A continious
```

---
## \#23 Posted by: sanderfu Posted at: 2019-01-23T21:26:38.943Z Reads: 21

```
Do we trust them with the history they have though..

Thanks for the input anyway ;)
```

---
## \#24 Posted by: epss4 Posted at: 2019-01-23T22:13:29.255Z Reads: 17

```
Not at all:P
```

---

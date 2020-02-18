# Motor Help Needed!

### Replies: 9 Views: 232

## \#1 Posted by: bmolnar Posted at: 2019-03-20T06:04:50.872Z Reads: 78

```
Hey all,

Been making my longboard, but when I put everything together today I noticed my motor kept stalling (skateboard won't move) when I'm standing on it at rest w/ the motor at full power. It works ok-ish if I have a bit of speed then turn on the motor.

I think my problem is I don't have enough torque to get myself moving. I weight about 150 lbs and the board is ~15 lbs. 

Is there a way to increase torque other than change my gear ratio? I noticed 650 KV is a lot of rpm for a skateboard. Would adding a second of the same motor help or should I just get a different motor altogether?

Thanks,
Benjamin

[Motor](https://hobbyking.com/en_us/propdrive-v2-series-4248-650kv-brushless-outrunner-motor.html) (650 KV 1295W) 

[ESC](https://hobbyking.com/en_us/hobby-king-80a-esc-4a-sbec.html) 80 A

[Battery](https://hobbyking.com/en_us/zippy-flightmax-4000mah-5s1p-40c.html) 5S

[Wheels](https://www.amazon.com/gp/product/B073WL8SCV/ref=ppx_yo_dt_b_asin_title_o00_s00?ie=UTF8&psc=1) 70 mm

[Belt/Mount](https://usa.banggood.com/DIY-Parts-Kit-Pulleys-And-Motor-Mount-For-7270MM-Wheels-Electric-Scooter-p-1180088.html?rmmds=detail-left-hotproducts__6&HotRecToken=CgExEAIaAklWIgJQRCgB&cur_warehouse=CN)
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-03-20T07:24:46.933Z Reads: 73

```
Yeaaaah, you bought just about the worst possible motor. That, and that ESC is not designed for ground vehicle use, which makes your problem worse. And you're using a very low battery voltage (The usual bare minimum is 6s, and 10s is recommended). All this together means you're not  going to have a good setup until you replace the motor at the bare minimum, and preferably the motor, battery and ESC.

The lesson of this is, buy right or buy twice. Don't cheap out on batteries or  ESCs, and do some research before you open your wallet.
```

---
## \#3 Posted by: meesie Posted at: 2019-03-20T10:13:26.476Z Reads: 65

```
assuming you're running 10s (2 zippies) you'd want to get one of these:

https://hobbyking.com/nl_nl/turnigy-sk8-6374-192kv-sensored-brushless-motor-14p.html

if you're not yet running at least 10S in voltage, you definetely should :slight_smile:
```

---
## \#4 Posted by: bmolnar Posted at: 2019-03-20T12:34:33.416Z Reads: 57

```
Thanks the the advice!

The motor you recommended has a max current of 100 A, do you think I'd need a 100 A esc or would my 80 A esc be fine?
```

---
## \#5 Posted by: Superflim Posted at: 2019-03-20T12:38:28.582Z Reads: 56

```
burst current Is 100 amps so yes
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-03-21T06:48:30.762Z Reads: 37

```
Buy a flipaky vesc. The performance difference between a car esc and a vesc is beyond words. Ive tried a car esc for kicks, felt like trash. (Xcar beast series 120a) dont buy cheap to save $30. Buy the right part and really enjoy your build
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-03-21T06:54:49.785Z Reads: 36

```
I should also say, you really need a real belt setup that works well. With a decent motor, that belt ans mount is pointless. Get some 90mm flywheel clones, boardnamics mounts, and a cheap pulley kit. Of you can afford it, get some better caliber II trucks as well. Ive seen so many people make boards like yours, and ive heard nothing but complaints. Spending a little extra will make it 10x better



https://m.banggood.com/15mm-Wide-Belts-DIY-ABEC-Flywheel-Pulley-Kit-265mm-255mm-p-1222305.html?rmmds=search

https://www.amazon.com/Owlsome-Longboard-Flywheels-Precision-Bearings/dp/B01IBJ5YDY/ref=asc_df_B01IBJ5YDY/?tag=hyprod-20&linkCode=df0&hvadid=312035433248&hvpos=1o1&hvnetw=g&hvrand=15115132181283644993&hvpone=&hvptwo=&hvqmt=&hvdev=t&hvdvcmdl=&hvlocint=&hvlocphy=9024158&hvtargid=pla-623518552686&psc=1


https://boardnamics.com
```

---
## \#8 Posted by: Superflim Posted at: 2019-03-21T08:03:53.259Z Reads: 35

```
Go dickyho route! Awesome budget stuff
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-03-21T09:20:39.504Z Reads: 30

```
A vesc clone rated for 80A (Or even 60) will give you far better performance than a car or airplane ESC that can deliver 120. You can run a 100A motor on a lower- rated vesc, but not on a lower-rated car or plane ESC.  
If at all possible, go for a 6.x version vesc-alike.
```

---

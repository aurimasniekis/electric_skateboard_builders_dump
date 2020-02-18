# Which battery should I choose?

### Replies: 15 Views: 321

## \#1 Posted by: Dutchman Posted at: 2019-04-15T20:01:30.270Z Reads: 134

```
Hey everyone,

I'm currently building my first board running a single 6374 motor.
Looking for a top speed of around 30km/h and a reach of 15-20km.

I'm planning on building  a 10s2p 18650 battery pack with the following items:

**20x Samsung 3000 mAh battery**

https://eu.nkon.nl/rechargeable/18650-size/samsung-inr-18650-30q-3000mah.html

**Vruzzend battery kit** (Cause I don't have a sport welder)

https://eu.nkon.nl/vruzend-diy-battery-kit-v2-0.html

**10S BMS**

https://www.aliexpress.com/item/10S-36V-Li-ion-Lithium-Cell-40A-18650-Battery-Protection-BMS-PCB-Board-

**Charging Cable**

**Battery indicator**

**180A Anti-Spark**

https://electricboardsolutions.com/collections/switches/products/180-antispark-switch

What are your thought on this setup? I just want to make sure I don't forget anything.

Improvements or tips are welcome!

Thanks!
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-15T20:03:18.962Z Reads: 125

```
3 people have created this same kind of threads....
```

---
## \#3 Posted by: brenternet Posted at: 2019-04-15T20:03:24.732Z Reads: 125

```
I would suggest buying a well made, welded battery from a professional.
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-04-15T20:15:11.588Z Reads: 121

```
Yeah but wheres the fun in that
```

---
## \#5 Posted by: Dirt_Bag Posted at: 2019-04-16T05:00:23.493Z Reads: 100

```
Fire is fun, but not when indoors. Some of the batteries i have seen built by new people are terrifying. They are one hard bump or abrasion away from being an inferno.
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-04-16T05:02:10.390Z Reads: 92

```
You are going to want the standard 10s4p or 10s3p battery for that sort of range. With a 30q cell in 2p, you will have longevity issues and voltage sag. I can build you a 10s battery if you like. I use sony vtc5 cells (2600mah 25-30a)
```

---
## \#7 Posted by: Dutchman Posted at: 2019-04-16T18:06:13.587Z Reads: 78

```
I looked into that as well, but building one is way more fun :smile:
```

---
## \#8 Posted by: Dutchman Posted at: 2019-04-16T18:09:48.133Z Reads: 72

```
I'm trying to build my board on a slim budget so I might have to reduce the range I was aiming for. How much are you asking for your 10s3p batteries?
```

---
## \#9 Posted by: Dirt_Bag Posted at: 2019-04-16T20:59:44.080Z Reads: 61

```
I will pm you about it
```

---
## \#10 Posted by: Dwain Posted at: 2019-04-16T21:44:24.722Z Reads: 61

```
Hey man i see u building a board and u want to use a 10s BMS. I have 2 for sale , i used them for a short time and they work great ! 

€25 each let me know if u are interested in purchasing 1 they are good quality.
```

---
## \#11 Posted by: captclearleft Posted at: 2019-04-17T10:59:32.129Z Reads: 43

```
I don't know much about the 18650's - But I am curious why a 10s 2p wont give you that range???  I run a cheap 10s1p 5ah lipos (2x5ah batteries) and have consistent 32km range at 24-30kph. Same exact motor. 

https://hobbyking.com/en_us/turnigy-5000mah-5s-30c-lipo-pack-xt-90.html
```

---
## \#12 Posted by: Friskies Posted at: 2019-04-17T15:58:27.130Z Reads: 27

```
@Dutchman I would probably consider a 3p 30Q battery for the range that you require. 10s will get you the speed (geared to around 30-40kmh should be easy). At this time I would probably go for the [NESE packs](http://18650.lt/index.php/product/n-e-s-e-module/) of you prefer to build your own pack. These are proven to be durable and reliable for Esk8 inside an enclosure. For the BMS you can run a **charge only** [Bestech D140](https://buildkitboards.com/collections/batteries/products/bestech-d140-charge-only-bms). You can run a discharge unit too but they are a lot larger.

It actually really depends on the capacity of the cells as well as the vesc setting/rider style/weight for range. Keeping in mind that your absolute max battery will be 40a which I would not reccomend for a 2p battery and voltage sag would suck.I would say that your range would possibly be achieved (15km) with a single drive on conservative settings and a small (low weight) but would be unlikely with a dual drive.  

@captclearleft I'd be interested to see what you are running to get that range as 32km would mean you either weigh nothing and run a single drive setup going down hill for 32 km or your stats may be a bit exaggerated. For reference I run a dual hummie hub 12s5p 30Q (15000 mAh for your lipo world) Unity 74kg rider at 50a motor and 65a battery and will consistently get about 30km with 33% left in the board. Please see today's ride for detailed stats.

https://metr.at/r/hjD5K
```

---
## \#13 Posted by: Dutchman Posted at: 2019-04-17T16:28:13.266Z Reads: 26

```
I'm thinking of doing the same, using 2 5ah lipo batteries instead of the 18650's.
Do you have them build into your board with a charge port or take them out each time you charge them?
```

---
## \#14 Posted by: Dutchman Posted at: 2019-04-17T16:34:34.596Z Reads: 27

```
Thanks for the advice! I might change my setup to 2x 5000 mAh Lipo batteries. This will probably help me stay within in my budget aswell. The BMS you advised would work with the lipo batteries aswell right?
```

---
## \#15 Posted by: captclearleft Posted at: 2019-04-17T16:47:37.552Z Reads: 24

```
@Friskies, You are correct. I am running a single TB 6374, Vesc 4.12, 110mm SuperFlys, two 5.0 5S LiPos (as 10s1p), 14t to 36t gears (I think... I'm not home) I weigh 155lbs (70kg)  I easily get 20 miles (32km) mostly flat in Denver CO USA. I cruise around 16mph (26kmh)... 
We need to start a spreadsheet with this kind of data...
I just finished a new board (2x6355s, 12s1p, 6x2 pneumatics... 10mi(16km) range is all I am getting... 😕... Now I am rethinking dual motors, my gear ratio, and my lipo selection.
```

---

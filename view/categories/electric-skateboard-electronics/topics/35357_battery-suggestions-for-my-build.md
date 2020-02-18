# Battery Suggestions for my Build

### Replies: 22 Views: 1136

## \#1 Posted by: apicker1 Posted at: 2017-10-12T05:46:08.685Z Reads: 156

```
I am starting to put together ideas for my Electric Longboard! I originally was going to get a deck and put this kit on it. http://www.diyeboard.com/10s5p-11ah-batteryescpower-truck-kit-dual-9052mm-hub-motors-p-598.html

I realized that it was a bit thick and I am going for a more streamlined look. I saw this battery and ESC housing but unfortunately it won't hold enough to power the motors I want efficiently.
http://www.diyeboard.com/dual-bldc-motor-sine-wave-foc-esc-speed-controller-for-diyeboard-p-522.html

The two pieces that I have chosen so far:
90mm Dual Hub Motors - http://www.diyeboard.com/dual-hub-motor-9052mm-1000w75kv-power-truck-front-truck-kit-p-558.html
ESC - http://www.diyeboard.com/dual-bldc-motor-sine-wave-foc-esc-speed-controller-for-diyeboard-p-522.html

I am new to figuring out what battery configuration I need to run this efficiently. I would appreciate any help to figure out the best way to power the board as well as a good case for the batteries and ESC.
Thanks!
```

---
## \#2 Posted by: willpark16 Posted at: 2017-10-12T05:51:05.614Z Reads: 151

```
What type of range and speed are you looking for?
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-10-12T05:53:44.369Z Reads: 142

```
I'd go 10s, you'll get about 25mph out of it. With hubs, you can't change the gearing (it's always 1:1) so you're kinda stuck with whatever battery gives you the speed you want.

For range, a good general rule of thumb is 10 watt-hours will get you 1km of range. So  a 10s pack with 5000mah (a common size lipo pack) will give you 10*3.7*5=185 watt-hours, or ~18km.


 I've used Kydex sheet to make an enclosure for my board, and you don't need a sophisticated vacuum setup. I used the house's oven and some foam and wood molds, and that worked just fine.
```

---
## \#4 Posted by: apicker1 Posted at: 2017-10-12T05:58:40.715Z Reads: 127

```
25mph and an average of 12 miles. I won't be going very far each day but want to have some juice if I forget to charge it during the night.
```

---
## \#5 Posted by: apicker1 Posted at: 2017-10-12T06:01:55.766Z Reads: 123

```
Thanks! I am still trying to grasp what the different amps, watts, etc. all mean for a battery and motor. I am working out of a dorm so the closest thing to an over I have is a hair dryer, a panini maker, and a box. :slight_smile:
```

---
## \#6 Posted by: willpark16 Posted at: 2017-10-12T06:03:37.662Z Reads: 113

```
10s3p should satisfy those needs
```

---
## \#7 Posted by: apicker1 Posted at: 2017-10-12T06:13:31.666Z Reads: 103

```
Based on MysticalDork's math, how many km would that get me? I am trying to figure out what the slimmest thing I could go for is. If they offered it, a 10s1p 3 in a row to make it flat would be great.
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-10-12T06:17:19.604Z Reads: 104

```
Either a 10s3p 18650 pack, or a 10s 5000mah li-poly pack will be just about right for those numbers. li-poly is cheaper but less durable. 18650s are more expensive but you'll get more charges out of them before they start to lose their capacity.

Depending if you go with 25R or 30Q (or other) cells, a 10s3p will generally have between 270 and 350 watt-hours in it, so between 27 and 35km.
```

---
## \#10 Posted by: apicker1 Posted at: 2017-10-12T06:24:24.989Z Reads: 97

```
How thick would a 10s3p be? The 10s5p made that casing extremely bulky. I was not sure if I could just daisy chain enough flat that I could power it. Are there any cells that you could link me that you like?
```

---
## \#11 Posted by: willpark16 Posted at: 2017-10-12T06:27:58.718Z Reads: 101

```
180mm wide 20mm tall
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-10-12T06:30:33.264Z Reads: 100

```
The standard cells are 18mm in diameter and 65 long. So the pack will generally be about 20mm thick, unless the cells are double stacked. https://ru.nkon.nl/samsung-18650-inr18650-25r.html Those used to be the golden standard, and they're still very good. https://ru.nkon.nl/samsung-inr-18650-30q-3000mah.html These are newer, have a little more capacity, and even though they're rated for 15 amps where the others are rated for 20, they actually outperform the 25Rs at 20 amps.


A realistic 10s3p pack size would be 140mm wide, 20mm thick and 270mm long.

For 18650 packs you'll also need a BMS, which will add to the pack size on top of the bare cell dimensions.

I have a 10s4p pack in my current build, and it's about the largest that would fit unless I got creative with routed-out slots in the board or double-stacked cells. 10s3p should be a pretty comfortable size for a longboard deck. If you're trying to fit all this on a board under 28" or so, you should consider lipo batteries just because they're more compact and power-dense, so you can use a smaller pack.
```

---
## \#13 Posted by: apicker1 Posted at: 2017-10-12T06:43:37.925Z Reads: 90

```
I thought that the ESC that I had selected would act also as the BMS. It had talked about protective measures and such. Would you mind linking me a 18650 10s3p pack? I'm searching for them but quickly realizing that I still don't know what I'm looking at haha.
```

---
## \#14 Posted by: willpark16 Posted at: 2017-10-12T06:48:37.025Z Reads: 84

```
I can make a custom one
```

---
## \#15 Posted by: apicker1 Posted at: 2017-10-12T07:00:25.940Z Reads: 77

```
I am trying to figure out how to string them together to get the thinnest look.
```

---
## \#16 Posted by: raven Posted at: 2017-10-12T07:55:38.786Z Reads: 80

```
Anyone knows why the motor works on a 5s and not on the 6s. Am really confused as it’s 120a car opto Esc. It should handle that current from what the spec says. Can’t trust the specs nowadays. Some guys even post how to blow up the house with dumb charging method
```

---
## \#17 Posted by: MysticalDork Posted at: 2017-10-12T14:44:43.317Z Reads: 67

```
Here's one that includes all the parts you'll need, including charger, battery monitor and BMS. https://eskating.eu/product/10s3p-eskating-electric-skateboard-battery/
```

---
## \#18 Posted by: JdogAwesome Posted at: 2017-10-12T15:13:44.822Z Reads: 70

```
No a BMS or Battery Management System helps balance and charge the pack. Yes the VESC or some other ESC's have a low voltage cutoff but the BMS protects the individual cells. Also if you live in the states IMRBatteries might be a better place for you to get your 18650's. The LG HE4 or HE2 cells are pretty cheap and are comparable to the 25R cells. Also a 10S3P will be almost half the size of a 10S5P.
```

---
## \#19 Posted by: apicker1 Posted at: 2017-10-12T18:34:19.376Z Reads: 63

```
It looks like they will be my cheapest option. I am guessing that I will have to do some soldering to get it into a 10s3p configuration. Is there a way to have them set up in a single row so that I can run them down the center of the board?
```

---
## \#20 Posted by: MysticalDork Posted at: 2017-10-12T18:42:08.699Z Reads: 62

```
You can arrange them any way you want. I wouldn't recommend soldering an 18650 pack as a first project though, unless you've got a decent amount of soldering experience already. If you're trying to get the slimmest possible build, I'd recommend getting 5 5000mah 2s lipo batteries and wiring them into a 10s pack. They're thinner, and they won't require you to solder directly to the cells.
```

---
## \#21 Posted by: JdogAwesome Posted at: 2017-10-12T19:31:50.733Z Reads: 62

```
Yeah just take a look at some different 18650 configurations, you can do them any way you want. You could solder all your cells though it's recommend to spot weld everything. A spot welder will add about $100 to your budget though you can use it for future builds or projects as well. And like @MysticalDork said using LiPo foil pouch cells will be easier and cheaper though you won't have as much range for the same size battery be cause there energy density is lower.
```

---
## \#22 Posted by: pennyboard Posted at: 2017-10-12T19:53:02.707Z Reads: 60

```
I'd go with 12s 5000 mAh Lipo pack. I've been running one without a BMS for over 9 months and it works great. I even bought a 12s charger off eBay so I can have laptop style charging without having to disassemble my board. All for about $130.
```

---
## \#23 Posted by: apicker1 Posted at: 2017-10-15T22:04:20.344Z Reads: 40

```
Yeah I have no soldering experience so I would rather stay away from that haha. I might go the with your idea and wiring them together.
```

---

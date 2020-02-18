# So many red and black wires!

### Replies: 18 Views: 2799

## \#1 Posted by: zmoney Posted at: 2016-05-25T03:40:53.709Z Reads: 189

```
**Before I start asking any questions im going to put down my (desired) first build below. Maybe you guys can find something wrong with it. (Might be missing stuff)**


 **MOTOR:** 1x [OllinBoardCo OM5065-200kv Sensored Motor](http://www.ollinboardcompany.com/product/om5065-200kv)

**MOTOR MOUNT:** I'm broke so this im [diying](http://www.homedepot.com/p/Simpson-Strong-Tie-12-Gauge-Angle-A24/100375162)

**BELT, PULLIES, AND DRIVE HUB:** [ Enertion's 12mm kit](https://www.enertionboards.com/cart.php)

**TRUCKS:** [Caliber II Trucks](http://www.amazon.com/Caliber-Degrees-Blackout-Skateboard-Longboard/dp/B00O05W0VI?ie=UTF8&psc=1&redirect=true&ref_=ox_sc_act_title_8&smid=A1KIGC2OOP10VK)

**WHEELS & BEARINGS:** Some cheap fly wheel knockoff's I found on [Amazon](http://www.amazon.com/Longboard-Flywheels-Wheels-Bearings-Spacers/dp/B00IO5D604?ie=UTF8&psc=1&redirect=true&ref_=ox_sc_act_title_7&smid=ALGPO5ABKXA1Z)

**CONTROLLER:** This [Wii Nunchuck](http://www.amazon.com/Wii-Kama-Wireless-Controller-Colours-Nintendo/dp/B0012R58LG?ie=UTF8&psc=1&redirect=true&ref_=ox_sc_act_title_6&smid=A8AS2V7147WAV).

**BOARD:**[ Loaded Bamboo Vanguard](http://www.amazon.com/Loaded-Bamboo-Vanguard-Longboard-Skateboard/dp/B00H7KB1BI?ie=UTF8&psc=1&redirect=true&ref_=ox_sc_act_title_10&smid=A1KIGC2OOP10VK) (Yes i know its pricey, but i bought a NEW one at a garage sale for 20 bucks)

**BATTARIES:** 2x in series [Turnigy nano-tech 5000mah 3S 25~50C Lipo](http://www.hobbyking.com/hobbyking/store/__20553__Turnigy_nano_tech_5000mah_3S_25_50C_Lipo_Pack_US_Warehouse_.html)

**VESC:**  [Ben Vedder's one on DIY's](product/vesc-the-best-electric-skateboard-esc/)

**CHARGER + THIS CHARGE LEAD:** [Turnigy Accucel-6 50W 6A Balancer/Charger](http://www.hobbyking.com/hobbyking/store/__18066__Turnigy_Accucel_6_50W_6A_Balancer_Charger_w_Accessories_US_Warehouse_.html) / [Twin pack charge lead (2 x 3S)6S w/ XT60](http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=10993)

Alright. Done with that. Soooo now some questions.

So my wiring set up is going to look something like this (if it works):

<img src="/uploads/db1493/original/2X/f/f1438c0980677d3cabb43365a796ff8dc91f8c24.png" width="479" height="452">
(the batteries are 3s not 6s, same for the charger)
## Where the yellow (and pink box that was supposed to be yellow on the top left corner) are, aren't they supposed to be XT-60's?

## Do I have so solder those into a XT-60 where the the red circles are?

## Also, can i leave the charger connected to the board so when i have to charge the board, so i can just plug in the laptop power supply cable?

**Thank you so much!**
```

---
## \#2 Posted by: jrpwit Posted at: 2016-05-25T03:55:10.350Z Reads: 157

```
Yeah those can be XT-60s cause they are only having the load of a single 3s battery going through them. But I would suggest using a BMS instead of having a balancing charger attached to the board. Firstly a BMS ill do all the things that the 12s changer you have but make this job alot simpler. I have a bms on my board and once did too consider attaching a charger like you to the board. Anyways looks good but a BMS would be better.
```

---
## \#3 Posted by: jrpwit Posted at: 2016-05-25T03:58:13.127Z Reads: 151

```
OH also one more advantage to using a BMS is that the BMS protects your batteries from over discharging when they go dead.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-05-25T04:06:21.374Z Reads: 146

```
You may want to re-think your motor choice or up the voltage 

Hit some calculations here

http://toddy616.blogspot.ca/2013/07/electric-skateboard-calculator.html?m=1

Then window shop on this thread 

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas


And lets see if you make some changes
```

---
## \#5 Posted by: jakobnator Posted at: 2016-05-25T04:56:33.248Z Reads: 119

```
If your looking for a relatively cheap build I wouldn't even bother with a BMS, instead just be smart with your batteries, and don't drop below their correct voltage. As for putting a charger on the board, the balancing chargers are relatively big and you have to press a few buttons to charge, on top of that they aren't exactly meant to handle the banging and vibrations that an e-board makes. All I can say with your wiring is make sure that your 2 3S to 6s converter is connected right. One of the 3s ports is the negative battery side and the other positive. Make sure this correlates with the wires that are going to the VESC
```

---
## \#6 Posted by: Iceni Posted at: 2016-05-25T05:20:35.509Z Reads: 110

```
The enertion drivehubs require you to modify your truck hanger, they need a longer axle than standard.
Can be done with some elbow grease or you can buy enertions truck which should come pre-modified.
```

---
## \#7 Posted by: zmoney Posted at: 2016-05-25T11:48:56.307Z Reads: 99

```
Thanks for all the help guys!. 

@Michaelinvegas whats wrong with the motor i chose (not being snarky im just curious as of why :D)? Honestly the only reason i chose those is because the sk3 245kv's are never in stock. Also, how do i output higher voltages? Do i put them in parallel?

@Iceni yeah i saw a video of a guy doing that to their trucks on Enertion's page. I was like wtf! Thank though, ill switch them up today.
```

---
## \#8 Posted by: lowGuido Posted at: 2016-05-25T12:01:24.867Z Reads: 90

```
[quote="zmoney, post:1, topic:3798"]
Where the yellow (and pink box that was supposed to be yellow on the top left corner) are, aren't they supposed to be XT-60's?
[/quote]
they don't have to be anything. they can just be soldered directly, no need for connectors really.
```

---
## \#9 Posted by: OskarCastrone Posted at: 2016-05-25T14:50:48.304Z Reads: 80

```
I think that motor is going to work out great! But yeah, you probably will not use the motors to their full potential...
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-05-25T15:11:25.302Z Reads: 82

```
The kv is too low... Ur gonna go like 12 mph...unless that's what u want ...and yes Honby King is always back ordered ...welcome to the club...
```

---
## \#11 Posted by: zmoney Posted at: 2016-05-25T18:51:38.257Z Reads: 81

```
:frowning: Damit Hobby king. I did some calculations with the blog post you posted and CalcRC and I got different results. 

<img src="/uploads/db1493/original/2X/4/40384503e92499bf051aaae9575d34e6fd1b9c8d.JPG" width="690" height="376">

When i was making my list I was going off CalcRc without keeping mind of the efficiency. I think I'm going to go with two 6s's instead of two 3's to make have a total of 12s. That way I can get this:

<img src="/uploads/db1493/original/2X/2/251417e78a2585159ce9e2bfa84037a9af818089.JPG" width="322" height="446">
```

---
## \#12 Posted by: zmoney Posted at: 2016-05-25T18:59:00.674Z Reads: 78

```
Do boosted boards have bms's instead of your typical charger? Or am confusing it with something else?
```

---
## \#13 Posted by: Michaelinvegas Posted at: 2016-05-25T19:00:16.625Z Reads: 76

```
Right now VESC and @torqueboards and @LEVer have ESCs that can handle 12s...

I'm waiting on an alternative 12s Esc and will test that out
```

---
## \#14 Posted by: jrpwit Posted at: 2016-05-26T00:05:40.542Z Reads: 73

```
Come on at least do a little research first. And to answer your question yes it does but seriously dont waste people's time asking questions you could just simply google. If you cant find what your looking for then ask your question. Btw I dont mean to come off rude but you could have just looked it up yourself.
```

---
## \#15 Posted by: jrpwit Posted at: 2016-05-26T00:17:29.384Z Reads: 72

```
Here is a link to the bms I use with my lipos http://www.batterysupports.com/44v-48v-504v-12s-30a-12x-36v-lithium-ion-lipolymer-battery-bms-p-268.html It works good but it is expensive. Also he is the link to the charger I use for it 
http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html

Also here is a diagram someone made to help me hook up the balance connectors of the battery to the bms. (btw i didnt make this pic i just dont recall who made it). This pick is helpful to me when I was hooking up my lipos cause I was using premade lipos for hobbyking that were in a series.
<img src="/uploads/db1493/original/2X/c/c3440a1c26fd938d955190679f9d7990f12026f8.jpg" width="640" height="480">

It make seem intimidating but it is surprisingly simple if you find some tutorials on how to hook up a bms.

Overall, a bms is great for charging on the go cause all you need is your charger. It is also really light and protects your batteries for over charging and over discharging. It is not entirely necessary though if you just monitor you batteries and use a balance charger. The only down side to the balance charger is that you have to open up your board and it is not ideal or practical for charging on the go. Also a bms plus the charger is expensive compared to just the balance charger. Anyways hope this helps you make your decision on how you will put together our board.
```

---
## \#16 Posted by: g4tv4life Posted at: 2016-05-26T03:59:39.275Z Reads: 61

```
FYI, ebay has the wheels for 5 dollars less.

http://www.ebay.com/itm/FREE-SHIPPING-Blue-Longboard-Flywheels-83mm-x-52mm-ABEC-7-Bearing-Spacer-/281745440544?hash=item4199563f20:g:IJAAAOSwu4BVnxaW

They have every color i believe.
```

---
## \#17 Posted by: jrpwit Posted at: 2016-05-26T22:39:40.811Z Reads: 50

```
Yeah those are some really good wheels! It stick to the ground really well when turning.
```

---
## \#18 Posted by: zmoney Posted at: 2016-05-27T02:31:32.214Z Reads: 46

```
I'll make sure to get those instead! Thanks!
```

---

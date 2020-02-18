# Budget &#124; Slow &#124; Short-range Longboard for complete Noobs

### Replies: 25 Views: 1030

## \#1 Posted by: kephart Posted at: 2018-12-04T22:17:51.561Z Reads: 239

```
I've never skated before, but when my youngest son (8 years old) said he wanted an electrical engine to build something that moves I started to investigate electrical skateboards and got hooked on the idea. I have some experience with Raspberry Pi , Arduino and Servos and DC-motors, soldering and other DIY-projects so I think I will be able to construct one, but I'm hesitant about the parts to use.

Our goals are a bit different than regular e-skaters I guess:
1. To have fun building it
2. To learn stuff about electronics, mechanics and batteries on the go
3. To build something reasonably safe
4. To build something stable and easy to ride
5. To find good budget alternatives, I’m thinking of a total budget around 300-400€. Buying used components is totally OK.
 
Things that are not important to us now are:
1. Speed - I guess around 15km/h will be enough
2. Range - If we can ride for half an hour that is OK to start with
3. Power to go uphill - We will try to stay level since we can't skate at all!

I'm thinking of following this tutorial:
[BigKids HOW TO BUILD A DIY ELECTRIC ⚡ SKATEBOARD](https://www.youtube.com/watch?v=LJqyWRSqOy4)

I'm interested in skimping on some parts however. Maybe we can use a weaker engine and/or also settle for a less powerful battery?
So far I've been thinking of these using these main parts:

1. [HGLRC-Flipsky FSESC 4.12 50A SK8 ESC](http://www.banggood.com/sv/FLIPSKY-FSESC-50A-SK8-ESC-Electronic-Speed-Control-5V-BEC-for-Electric-Longboard-RC-Car-E-bike-p-1293459.html?rmmds=cart_middle_products) - Maybe we can get a cheaper, less powerful ESC and hook it up to my Arduino?
2. [BangGood DIY Electric Skateboard Kit](https://www.banggood.com/sv/DIY-Electric-Skateboard-Kit-Parts-Pulleys-And-Motor-Mount-For-80MM-Wheels-p-1146629.html?cur_warehouse=CN)
3. 6374 190KV Outrunner motor - Maybe we can get a cheaper, less powerful alternative? Maybe a combined RC car ESC/motor-kit could save money?
4. A regular flexing longboard
5. Large wheels 70-90mm
6. Caliber trucks
7. Homemade enclosures.
8. Batteries - Not decided yet, could one Turnigy 5S 21V be enough for our purposes?
```

---
## \#2 Posted by: Jmding Posted at: 2018-12-04T23:16:40.285Z Reads: 209

```
That ESC is available for around $55 on aliexpress. You're not going to find a much cheaper ESC than that at almost any power level.

At your power levels, consider hub motors. They are inexpensive and mechanically simple. The kit you linked to is going to be a struggle to get working with likely lots of machining involved.

It sounds like you generally are are concerned about much power you need, and whether your components will be able to supply it. This is an AWESOME opportunity to teach some physics concepts. Use a free-body diagram to calculate how much thrust you need to maintain speed on a 20% gradient hill. Use the concept of torque and gear ratios to translate that to torque at the motor. Motor torque = Kt * current, where Kt = 1/Kv (after some unit conversions), so you can calculate the required current and compare it to what your electrical system can deliver.
```

---
## \#3 Posted by: Grozniy Posted at: 2018-12-04T23:31:57.916Z Reads: 193

```
Don't get banggood kit!!!!
Search for used TB vesc in the forum.
Check @dickyho for mounts, wheels, belts, trucks even, etc.
 190kv motor is ok. Want slow? Get only 6s battery. Lipo. Preferably above 40c.
This should be a good start for you to search and have fun with your family.
IMPORTANT: safety!!! Get safety equipment
```

---
## \#4 Posted by: b264 Posted at: 2018-12-04T23:34:04.694Z Reads: 177

```
[quote="Grozniy, post:3, topic:77072"]
IMPORTANT: safety!!! Get safety equipment
[/quote]

Yes, make sure you have a helmet in the house before any kind of powered skate equipment is made.  Because the second it's made, it will be ridden...
```

---
## \#5 Posted by: Grozniy Posted at: 2018-12-04T23:40:35.522Z Reads: 168

```
https://www.electric-skateboard.builders/t/15-20-boardnamics-caliber-motor-mounts/73643?u=grozniy
```

---
## \#6 Posted by: kephart Posted at: 2018-12-05T20:46:21.369Z Reads: 147

```
Thanks for the hints!

I found this kit that seem like a bargain:
[ebay kit 400kv mount and motor](https://www.ebay.de/itm/N5065-400KV-Brushless-Motor-Riemenscheibe-Halterung-Set-Fur-Scooter-70-72mm-Rad/322645856298?_trkparms=aid%3D555018%26algo%3DPL.SIM%26ao%3D1%26asc%3D20140117130753%26meid%3D3ea1b0da37c34504b6c0d71904c83365%26pid%3D100005%26rk%3D3%26rkt%3D3%26mehot%3Dpp%26sd%3D283263133404%26itm%3D322645856298&_trksid=p2047675.c100005.m1851)

I checked with the calculator:
[Electric Skateboard Calculator](http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1), and it seems the top speed will be more than enough, but it seems I and the calculator must be missing something here. According to your formula:
[quote="Jmding, post:2, topic:77072"]
Motor torque = Kt * current, where Kt = 1/Kv
[/quote] more KV leads to less torque right?

Hub motors indeed seem a lot simpler, but I have been discouraged to get them in Sweden since we have so much stone in our asphalt (to cope with spiked winter tires) which makes for a bumpy ride, thus a preference for thicker tires. I figure that if I want to upgrade later an outrunner will also be more modular and will not place any constrains on the trucks.

Speaking of trucks, the above mentioned mount featured a round hole, is that a big disadvantage? I see a lot of reference to the calibre trucks, maybe because they are square and thus will avoid slippage.
```

---
## \#7 Posted by: kephart Posted at: 2018-12-05T20:47:18.089Z Reads: 122

```
Thanks! Will check out @dickyho, hope he ships to Sweden.
```

---
## \#8 Posted by: kephart Posted at: 2018-12-05T21:13:22.853Z Reads: 120

```
Thanks @Grozniy! That mount sure looked pro, and a good price too!
```

---
## \#9 Posted by: Grozniy Posted at: 2018-12-05T21:17:30.780Z Reads: 120

```
Don't get that kit. At least buy KEDA 6364
```

---
## \#10 Posted by: pat.speed Posted at: 2018-12-05T21:18:06.097Z Reads: 124

```
I would advise against a 400kv motor, it will lack in torque unless geared very unusually.

Your plan started well with the flipsky vesc and 190kv motor. I would use the Keda 190kv motor from hobbyking to save some money. A 6s battery will be perfect to start with and you should get a speed around 25km/h but this can be lowered in the settings of the vesc. 

You will also need some wheels 97mm would be best if there are lots of rocks. Truck will be needed and either turnigy trucks and their mount will be a cheap easy fit, or caliber 2 with a mount from the forum.

You also need pulleys which can be bought on the forum or from @dickyho or if you have a 3D printer you can print the large one.

You also may want to use a bms for charging instead of a balance charger and the switch for the board can be made from an XT90s connector.

Good luck and have fun with you kid 🙂
```

---
## \#11 Posted by: kephart Posted at: 2018-12-05T22:30:05.212Z Reads: 111

```
I looked at the Hobbyking site and I was happy to see they also ship from Europe which is good considering you get around 15$ of extra charges per shipment plus 25% VAT otherwise. The price for a good motor isn't to bad either.

I have put these parts in the cart now:

1. [KEDA 63-64 190KV Brushless Outrunner 10S 2000W](https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html)
2. [TURNIGY HEAVY DUTY 4000MAH 6S 60C LIPOLY BATTERY PACK](https://hobbyking.com/en_us/turnigy-heavy-duty-4000mah-6s-60c-lipoly-battery-pack.html)
3. [TURNIGY P606 LIPOLY/LIFE AC/DC CHARGER (EU PLUG)](https://hobbyking.com/en_us/pd606-charger-eu-plug.html)

Does Hobbyking have any ESC worth considering?
I'm also wondering whether I could get away with a cheaper battery maybe. Is 4S enough for my modest requirements? 40C? Maybe a 1200mAh will be OK to start with as well?
```

---
## \#12 Posted by: Grozniy Posted at: 2018-12-05T22:45:24.586Z Reads: 107

```
https://hobbyking.com/pt_pt/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html
The rest items are good
```

---
## \#13 Posted by: kephart Posted at: 2018-12-08T21:47:41.224Z Reads: 89

```
Does Hobbyking have the pulleys to match the their KEDA motor?
I don't see the specs on them.
```

---
## \#14 Posted by: pat.speed Posted at: 2018-12-08T22:36:17.461Z Reads: 89

```
I think so? The Keda motors all have 8mm shafts and I would assume the hobbyking pulleys are the same as they work with there other 8mm shaft motors
```

---
## \#15 Posted by: Grozniy Posted at: 2018-12-08T22:51:28.948Z Reads: 84

```
KEDA shaft is round. You'll need to file flat spots for grub screws. Use knurled tip grub screws, loctite 243 and Wera Hex Plus to torque them down
```

---
## \#16 Posted by: pjotr47 Posted at: 2018-12-09T01:22:55.243Z Reads: 81

```
Where do you live? I have some cheap parts laying around... those parts are perfect for a cheap first build
```

---
## \#17 Posted by: Schulerbible Posted at: 2018-12-09T01:32:25.803Z Reads: 84

```
Get the pulleys and belt(s) from eBay
```

---
## \#18 Posted by: kephart Posted at: 2018-12-11T20:26:42.851Z Reads: 74

```
Thanks @pjotr47! 

That's very interesting. What kind of teething do you have?

We live in Stockholm, Sweden.
```

---
## \#19 Posted by: pjotr47 Posted at: 2018-12-11T21:05:31.863Z Reads: 68

```
https://www.electric-skateboard.builders/t/eu-garage-sale/76947
```

---
## \#20 Posted by: kephart Posted at: 2019-09-16T22:20:46.509Z Reads: 41

```
Long time, no work on the board, but now I have all the parts. 
Got a 12t motor pulley with set screws from Italy. Is there anything in particular I need to think of when filing down the shaft? I need to get down about 1,5mm in so that the set screws don't protrude and disturb the belt. Could drilling be an option? Thinking of using me Dremel-clone.
```

---
## \#21 Posted by: venom121212 Posted at: 2019-09-16T23:42:10.779Z Reads: 39

```
Cover the motor can with a bag and tape it closed when filing! Those metal shards will get all over the magnetic motor and could mess things up otherwise
```

---
## \#22 Posted by: kephart Posted at: 2019-09-18T19:17:10.118Z Reads: 37

```
Hello guys,

Just wanted to say thanks for the help and share some experiences after the maiden voyage of the board today.

I mistakenly bought Caliber I trucks instead of Caliber II. They looked the same, so I thought it wouldn't matter. It did, but it seems to work after some work with the metal file.

Second minor mistake was that I bought the biggest Orangutang Kegel 80mm wheels they had in the shop. They seem a bit small in diameter and the amount of space between the dickyho-mount and the ground is disturbingly small. They do however fit very well with the 36T pulley I bought from Eskating Europe. The timing belt that came with the Dickyho-mount (HTD 320  5mm 12mm) is however a bit long. For our purposes, a slow cheap board, maybe a 40T pulley would be better. As it is now I think I need to get a new shorter belt.

During the first ride it also became clear why Loctite on the set screws is highly recommended. The motor pulley quickly came loose and one of the set screws unscrewed itself twice.

The VESC-configuration and soldering of the power cables was relatively straightforward. The BLDC-tool however seems to have a layout issue on Mac OS X. I couldn't see the panel where you see that the motor was connected so I switched to using a Windows computer.  I haven't done any loop-plug, or on/off switch yet. Will probably do so.

The KEDA 63-64 190KV motor seems fine, though in hindsight, maybe it would be worth it to buy another one with a groove for the set screws. Annoying work with the file again.

All in all, I  consider the project to be a success anyway and I think we will have a lot of fun with it. Now we just need to learn how to skate ...
```

---
## \#23 Posted by: kephart Posted at: 2019-09-18T19:22:31.117Z Reads: 36

```
![20190918_194812|375x500](upload://sSHkAKR7qHi7XoVApBVlH2gz2HR.jpeg) ![20190918_200712|666x500](upload://71Dr0t11sFr0zyNdPitrcsA2HDf.jpeg) ![20190918_200721|666x500](upload://qBE4Wr1TBxf4mX2xQTc67tgpp4w.jpeg) ![20190918_200733|666x500](upload://hVAWKIgQx7amwRKbahg4nh7nJNw.jpeg) ![20190918_200753|666x500](upload://9h3TbrzhVdvBFPSWlAvWx5FfX9I.jpeg) ![20190918_201021|666x500](upload://m6DWXhjfVQkZPElDqvwUWg8Hy3U.jpeg) ![20190918_201609|666x500](upload://9tbyjjYAt4yIu6CVjpwe2nzJMoj.jpeg) ![20190918_201858|375x500](upload://qeGAKW6Jgpjp900iRVT0Cvh6qiL.jpeg)
```

---
## \#24 Posted by: kephart Posted at: 2019-10-07T21:12:45.903Z Reads: 30

```
OK, so now we have been riding the board for awhile. I bought a new shorter timing belt after some great support from  @Boardnamics. I bought a HTD 305mm and this seems perfect for this mount. I also bought a 16T pulley to use if I want higher top speed.

We have some bad problems though with cutouts and stuttering. I will check my phase wires since I skipped on bullet connectors and bought crimp connectors for car use and I have my doubts about these.

I'm also wondering how much better a sensored motor would be. The startup is not really smooth with the KEDA. Speed-wise I'm very happy though. I don't need more speed right now, what I need is more reliability.
```

---
## \#25 Posted by: kephart Posted at: 2019-11-11T15:24:57.777Z Reads: 22

```
I did some research and fixed the phase cables with zipties to the motor and enclosure. This seems to have fixed the cutouts and stuttering. Also switched to the 16T pulley since I broke the 305mm belt :frowning_face: I should have stopped throttling when hearing that the motor didn´t move and screeched.  16T and seems to work fine even uphill. The top speed seems to be about 18-20km/h. Still only using the 6S battery.
```

---

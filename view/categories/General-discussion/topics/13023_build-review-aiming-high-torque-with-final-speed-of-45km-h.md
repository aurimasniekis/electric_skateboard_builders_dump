# Build Review - Aiming high torque with final speed of 45km/h

### Replies: 21 Views: 2818

## \#1 Posted by: krueger Posted at: 2016-11-14T00:50:42.113Z Reads: 245

```
Hello everyone!
After lots of research that’s what I put together. What are your thoughts on this?
As I live in a city with very irregular geography with lots of ups and downs on my way to work, while selecting the components I aimed to achieve high torque with a 380KV Brushless motor. I know you guys usually recommend bellow 300kv, but to compensate high KV I used small motor pulley to achieve high torque with max speed bellow 48km/h. Here’s the full build:

Motor: [Hobbyking](https://hobbyking.com/en_us/ntm-prop-drive-50-60-series-380kv-2665w.html) NTM Prop Drive 50-60 Series 380KV / 2665W / Max current: 90A – **USD 45,85**

Motor Mount: [Torque Boards](diy-electric-skateboard-kits-parts/v4-63mm-motor-mount/) v4 Motor Mount (ONLY) – **USD 32,89**

Motor Pulley: [10 Teeth Belt Pulley](https://www.aliexpress.com/item/SZS-Hot-Stepper-Motor-10-Teeth-5mm-Bore-XL-Type-Aluminum-Timing-Belt-Pulley/32759447707.html?spm=2114.10010108.1000013.4.uwAwhu&scm=1007.13339.33317.0&pvid=4de22345-1c0a-4e7f-8394-424fefcf4116&tpp=1) – **USD 1,25** (Not necessarily this one, I can get a custom 10 Teeth. The important thing is to remain at 10T, otherwise max speed will surpass 45km/h)

Battery: Pack LG INR18650-HG2 Cells 8S5P – **USD 280,00**
5A discharge BMS/PCM for 8S 28.8V 29.6V Li-ion, 432Wh. To bypass BMS low discharge, I will connect positive and negative wires going to your ESC straight to the battery instead of through the BMS.

ESC: [Torque Boards](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/) VESC BLDC Speed Controller – **USD 100,00**

(Updated)
Controller: [Benchwheel remote control](https://aliexpress.com/store/product/Electric-skateboard-refitting-parts-remote-control-bench-technology/1967440_32731985084.html?spm=2114.8147860.0.0.wgYdvV) - USD 40,00
Discarded option: [spoiler][2.4Ghz remote controller with receiver](https://pt.aliexpress.com/item/Wholesale-New-arrival-2-4Ghz-mini-remote-controller-with-receiver-for-electric-skateboard-longboard/32678995218.html?spm=2114.10010108.1000013.21.qQPOpv&scm=1007.13339.39449.0&pvid=c9dacb6a-46a5-4d2a-b315-80abb3ab95f0&tpp=1) – **USD 46,80**[/spoiler]

Trucks: [From Amazon](https://www.amazon.com/Caliber-Degrees-Blackout-Skateboard-Longboard/dp/B00O05W0VI/ref=sr_1_1?s=outdoor-recreation&ie=UTF8&qid=1478623097&sr=1-1&refinements=p_89%3ACaliber]) Caliber II Fifty Caliber 10"/50 Degrees Blackout Trucks – **USD 39,95**

Caliber Clamp: [Torque Boards](diy-electric-skateboard-kits-parts/v4-caliber-clamp/) v4 Caliber Clamp (ONLY) – **USD 32,50**

Wheels: Orangatang Kegel 80mm 80a Wheels [From Amazon](https://www.amazon.com/Orangatang-Kegel-Orange-Longboard-Wheels/dp/B00EYDHWTQ/ref=pd_sim_sbs_468_2?_encoding=UTF8&psc=1&refRID=FVH4FK0NNMJ0YM906GAZ) – **USD 60,00**

Bearings: Bones Bearings Reds Bearings [From Amazon](https://www.amazon.com/Bones-Reds-Precision-Skate-Bearings/dp/B000FDRQ1S/ref=sr_1_1?s=outdoor-recreation&ie=UTF8&qid=1478784835&sr=1-1&keywords=ceramic+bearings) – **USD 12,96**

Deck: [Bamboo](http://www.bambooskateboards.com/shop/cruisers/running-on-empty-cruiser/) Skateboards – **USD 56,00**

Pulley Kit: [Torque Boards](diy-electric-skateboard-kits-parts/36t-kegel-pulley-combo-kit/) 36T KEGEL Pulley Combo Kit – **USD 49,99**

**Total: 758,19 USD**
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-11-14T01:47:32.877Z Reads: 215

```
[quote="krueger, post:1, topic:13023"]
Motor: Hobbyking NTM Prop Drive 50-60 Series 380KV / 2665W / Max current: 90A – USD 45,85
[/quote]


Do yourself a favor ....


Get a different motor with a lower KV.  This will help at lower speeds and crappy roads....yeah ...your gearing it..and it will work..but not ideal. Check around. 

Get a lower kv motor running higher voltage since you seem to be making your own pack 8s pack. Why not go 10s.

Higher voltage means pulling less amps..and that's a good thing.  The more optimal your setup to your weight, road conditions etc...the better, faster the further it will go. Over spec the board a little in terms of motor and battery... you won't regret it
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-11-14T01:48:42.562Z Reads: 212

```
Also regarding the NTM 

https://youtu.be/FPw46nkLmV4


A video I made
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-14T01:55:01.268Z Reads: 205

```
In additional to @Michaelinvegas's comment you'll want to use something with at least 13T. 10T will skip like crazy on acceleration/braking, especially with a single drive. There's just not enough teeth in mesh at any given time.

The remote you linked has a ton of reliability problems as well, as well as very little throttle range. You should get something more reliable and easier to use. If you like trigger style remotes the GT2B or the TB mini (not nano) remote works well. Otherwise, I use the benchwheel remote myself and it's been rock solid and reliable. 

45km/h is pretty easy to acheive, but you should get a lower kv motor and increase gearing to 15/16T motor pulley and run 10s instead of 8s. Ollinboard Co's 200kv 5065 motor is a great choice for this.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-11-14T02:14:19.236Z Reads: 186

```
Thanks @Jinra....working on that motor right now lol
```

---
## \#6 Posted by: lox897 Posted at: 2016-11-14T02:41:43.554Z Reads: 183

```
380kv is way too high for an eboard. Depending on voltage, 270kv is the highest I would ever go. If you are running 10S then 190-200kv is perfect
```

---
## \#7 Posted by: saul Posted at: 2016-11-14T03:04:05.970Z Reads: 180

```
[quote="krueger, post:1, topic:13023"]
v4 Motor Mount (ONLY) – USD 32,89
[/quote]

this is only the clamp part the whole thing is like 80 something...

10t is too small. 13+, 14t/36 works great. with a 6354 on 90/97mm wheels!
kegels seemed slip too easy with the torque on a single....maybe i need to break them in or calm down..:sunglasses:
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-14T03:05:54.228Z Reads: 168

```
He has both clamp and mount on the list :P
```

---
## \#9 Posted by: Mobutusan Posted at: 2016-11-14T07:48:23.694Z Reads: 162

```
@krueger I'm no expert on the VESC, but I know that 380kv on 8s will be way over the recommended max ERPM, and could leave you with a fried VESC. I believe 60k ERPM is the "safe" max, and your setup will put your ERPM at 78k at nominal voltage and 89k+ at full charge voltage. Even on 6s, your ERPM will be too high on a full charge. 

This calculator is your friend. Good luck.
http://calc.esk8.it
```

---
## \#10 Posted by: bigpianist Posted at: 2016-11-14T11:39:34.776Z Reads: 156

```
haha guys I use dual 450kv (turnigy sk3 5045) and after setting motor limit to 60a and vesc erpm to 60k, I get some good torque and hill climbing power on 6s, not to mention it's very fast. Motors get warm but not very hot. So it's doable but lower kv is probably better. I'm using 12-36t gearing with kegels btw.
```

---
## \#11 Posted by: krueger Posted at: 2016-11-14T12:50:00.467Z Reads: 158

```
Thank you everyone who shared some of your knowledge to assist me. Considering your position on high motor kv, I have selected others to hear what you have to say about them:

Ollin Board OM5065-200kv 2200W - 84,00
Ollin Board Shipping - USD 60,00 (seriously? :weary:)

SK3 6374 192kv 2750W - USD 79,96
SK3 5065 236kv 1850W - USD 60,71
NTM 5060 270KV 2400W - USD 45,44
Hobbyking shipping - USD 30,00

Torque Boards Motor 5055 280KV 1750W - USD 70,00
Torque Boards Motor 6374 190KV 3150W - USD 120,00
Torque Boards Motor 6355 190KV 2500W - USD 90,00
DIY Skateboard shipping - USD 40,00 (also expensive shipping)

I've seen lots of people using SK3 motors. Ollin Board seems a very nice alternative, however their shipping price... No comments on that!
From my point of view the SK3 of 79,96 (total 110 with shipping) seems a viable option with good relation in terms of performance and cost.

Here are my replies to your considerations:
[quote="Michaelinvegas, post:2, topic:13023"]
Get a lower kv motor running higher voltage since you seem to be making your own pack 8s pack. Why not go 10s.
[/quote]

@Michaelinvegas I didn't go 10S because more cells in series means more volts, that would translate into more rotations per volt (kv) and too high max speed. 8S5P are 40 cells in total and 100A max discharge, which would satisfy the motor. With a lower KV motor, there will be less current consumption (maybe 60 or 80 max), thus I can make it 10S4P, which are still 40 cells. In short, I will use lower KV motor and make a 10S battery with the same 40 cells. :thumbsup:

[quote="Michaelinvegas, post:2, topic:13023"]
Over spec the board a little in terms of motor and battery... you won't regret it
[/quote]

That's exactly what I tried to achieve. I thought that maybe, more KV with adjusted gearing would improve torque significantly. But I'll definitely see to your advice of getting a lower kv motor running higher voltage. I'll check on your video on NTM later at home. Thanks for the advice!

[quote="Jinra, post:4, topic:13023"]
I use the benchwheel remote myself and it's been rock solid and reliable.
[/quote]

@Jinra Thanks for the advice, benchwheel it is then!

[quote="Jinra, post:4, topic:13023"]
Ollinboard Co's 200kv 5065 motor is a great choice for this.
[/quote]

This motor really looks great, however the shipping Ollinboard  is charging me is way too much!

[quote="saul, post:7, topic:13023"]
10t is too small. 13+, 14t/36 works great. with a 6354 on 90/97mm wheels!
[/quote]

@saul I'll change the motor, this way I can go 13T+ without fearing too high top speed. Is there a reason why you recommend 90/97mm wheels over the 80/83mm? As you mentioned wheels, what about Wheel Durometer? 78a, 80a?

[quote="Mobutusan, post:9, topic:13023"]
I'm no expert on the VESC, but I know that 380kv on 8s will be way over the recommended max ERPM, and could leave you with a fried VESC
[/quote]

@Mobutusan Thank you for this information. I used the calculator to keep max speed under 48km/h, however I did not know about VESC max ERPM limit.

[quote="bigpianist, post:10, topic:13023"]
guys I use dual 450kv (turnigy sk3 5045) and after setting motor limit to 60a and vesc erpm to 60k, I get some good torque and hill climbing power
[/quote]

@bigpianist That's exactly what I was trying to achieve with this build - torque and hill climbing. But as this is my first build, it's wise to listen what most experienced builders are saying. This time I will get lower kv motor, but on my next one I will attempt what you have done, and compare the results in terms of cost x efficiency.

One again thank you for sharing your insights.
```

---
## \#12 Posted by: Michaelinvegas Posted at: 2016-11-14T20:00:17.241Z Reads: 104

```
[quote="krueger, post:11, topic:13023"]
too high max speed
[/quote]

You do realize there is a throttle and you don't have to pull the trigger all the way in....

You want the power of the higher voltage and not the speed...

I think of as horses pulling a wagon....

Are 8 horses better or 10 horses better? It's not as simple as that but it's a mind set.... 10 horses would have an easier time pulling the same wagon. And that's what you want...the less strain you put on your parts....the longer they last.

I'm good with 6s if I wanted cause I have almost no hills and good roads in Las Vegas. But add some incline and not great roads...every thing needs to be upgraded to cope with the added stress 

Anyway in the end you will have an awesome ride that you can ride almost everywhere....

Look forward to your build🤘🏻
```

---
## \#13 Posted by: NickTheDude Posted at: 2016-11-14T20:22:27.506Z Reads: 102

```
Everyone recommends low kV because it allows you to use a higher voltage battery to achieve your desired top speed. Higher voltage means lower amps and therefor less heat in the VESC. Whenever possible you should be aiming to use the VESCs max voltage which I'm pretty sure is 10S.

If you want to reduce your top speed in favor of torque, simply increase your reduction ratio. This will actually give you a more efficient system since BLDCs are more efficient at higher RPMs.

Also, make sure you look at a motors max voltage/amps. Most smaller motors cannot handle 10S which is why 6355s are so common.
```

---
## \#14 Posted by: krueger Posted at: 2016-11-14T23:03:33.296Z Reads: 99

```
Hey @Michaelinvegas and @NickTheDude, 
I'm no expert in electronics, so let me ask you something else. If I am understanding you correctly, both of you prefer to have more more batteries in series than in paralel, meaning more volts and less amps.

[quote="Michaelinvegas, post:12, topic:13023"]
10 horses would have an easier time pulling the same wagon.
[/quote]

[quote="NickTheDude, post:13, topic:13023"]
Higher voltage means lower amps and therefor less heat in the VESC.
[/quote]

Just to illustrate my question, supose I pick this motor from [Hobbyking](https://hobbyking.com/en_us/ntm-prop-drive-50-60-270kv-2400w.html): NTM Prop Drive 50-60 270KV / 2400W - **Max current: 90A**.
Depending on the cell I choose, a 10S4P won't have sufficient Amps to "feed" the motor. In this case, while the motor can reach 90A, a 10S4P pack of **LG-ICR18650HE2**, for example, **would generate** **80A**. Under these conditions, would you still prefer Volts over Amps?
I understand that less volts means less heat in the VESC, but I think it can also mean a reduction in the motor performance. Or higher voltage would somehow compensate the Amp loss? (As I said I'm no expert in electronics).



[quote="NickTheDude, post:13, topic:13023"]
VESCs max voltage which I'm pretty sure is 10S
[/quote]

I'm going 10S, not more than that. Anyway I checked Vedder/VESC [website](http://vedder.se/2015/01/vesc-open-source-esc/) to obtain accurate information: "Safe for 3S to 12S LiPo"

[quote="NickTheDude, post:13, topic:13023"]
make sure you look at a motors max voltage/amps
[/quote]

Yes, I am paying close attention to this information, specially because I will make my own battery.

[quote="Michaelinvegas, post:12, topic:13023"]
Look forward to your build
[/quote]

Me too! :smiley:
```

---
## \#15 Posted by: NickTheDude Posted at: 2016-11-14T23:41:05.844Z Reads: 72

```
Using a VESC, yes under those conditions you still want less amps since the VESCs amp limit is much lower. Also, in general more amps in the VESC means more losses due to heat, and a higher chance of blowing it up.
```

---
## \#16 Posted by: Michaelinvegas Posted at: 2016-11-15T04:58:36.863Z Reads: 77

```
[quote="krueger, post:14, topic:13023"]
I choose, a 10S4P won't have sufficient Amps to "feed" the motor.
[/quote]

Lol yeah you will as long as you don't use laptop batteries....you will be fine
```

---
## \#17 Posted by: Namasaki Posted at: 2016-11-15T05:26:00.904Z Reads: 87

```
[quote="bigpianist, post:10, topic:13023"]
haha guys I use dual 450kv (turnigy sk3 5045) and after setting motor limit to 60a and vesc erpm to 60k
[/quote]
Ok, I have wondering about this for some time. 
So what happens exactly when your motor hits the 60k erpm limit that you set with the bldc tool?
Does the Vesc shut down or back off or does it just level out at 60k?
```

---
## \#18 Posted by: Namasaki Posted at: 2016-11-15T05:36:59.095Z Reads: 88

```
What about alien power?
They're located in the U.K. 
They sell high quality motors for reasonable price. 
I have 4 of there HEV 6355 190kv precision motors. 
Very good imo. 
10mm shaft so I had to buy my pulleys from them as well but I like the heavy duty and close tolerance construction of these motors. 
There 63mm motors have 10mm shaft
There 50mm motors have 8mm shaft
http://alienpowersystem.com/product-category/brushless-motors/
```

---
## \#19 Posted by: Jinra Posted at: 2016-11-15T08:00:04.961Z Reads: 78

```
If you set this in the motor tab,I think it just shuts off. If you use the soft erpm limit in app config, it'll throttle it back i believe. Haven't tried it myself.
```

---
## \#20 Posted by: Namasaki Posted at: 2016-11-15T12:35:18.069Z Reads: 69

```
I was just curious and since @bigpianist  has first hand experience, I would like to know how he set the limit and how well it works.
```

---
## \#21 Posted by: bigpianist Posted at: 2016-11-15T13:44:31.098Z Reads: 65

```
In my experience, you tick the "limit e rpm with negative torque" and the speed tops out I think. Like when you're going full throttle and full speed, it kinda does what the boosted board does and just stops accelerating, and keeps you at your top speed. Its quite neat. I'm not sure what happens if you don't tick the box though, could be dangerous if it shuts off during top speed.
```

---

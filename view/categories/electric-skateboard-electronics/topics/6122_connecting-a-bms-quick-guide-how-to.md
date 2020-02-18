# Connecting a BMS Quick Guide \[How-to\]

### Replies: 114 Views: 33201

## \#1 Posted by: oriol360 Posted at: 2016-07-14T23:42:38.009Z Reads: 1408

```
Hey eSk8!

Just want to share how I connected my BMS to LiPos. In this case I will be using two 4S Lipos in series to an 8S BMS...
However this guild should work out for any LiPo config you would like to use.

You will need:
BMS
LiPo Batteries
Soldering Skills

So I did not think about making this guide until I had already soldered all my components... I will update when I do this again but until then hope the pictures help.


This picture shows how the BMS is supposed to be wired.
<img src="/uploads/db1493/original/2X/5/571452b2e27f976b53b4d769a161c1accdb9abdd.png" width="689" height="362">

You will need to solder the negative leads the the B- and P- locations.
As well as the last black wire on the balance leads from the battery will need to be soldered to the B- Location.

<img src="/uploads/db1493/original/2X/f/fa5a7e680f3f2063a0a405d6f15fa0f321d5c33d.jpg" width="375" height="500">

For wiring in series, it is very important you follow this chart so nothing gets shorted when connecting your batteries.
<img src="/uploads/db1493/original/2X/9/93d42fbdc21084daec19f199e9d9bf075d60db12.gif" width="365" height="500">

You can see I have all five balance leads on the battery with the positive wire but i only have the last 4 on the battery with the negative wire(red wire removed). With the last black wire going to the B- location.
<img src="/uploads/db1493/original/2X/b/b338e047fd119998805580ce40fefd06ffde0e7c.jpg" width="375" height="500">

Make sure you plan how you are going to connect everything before actually connecting it as you will only have one chance, if you short any of your components they will not work again and just lost your money.
<img src="/uploads/db1493/original/2X/7/7c838f554a58d96d7227d4507d6ebe4f203ac9b7.jpg" width="666" height="500">

Once you have double checked everything. YOU MUST FIRST plug in the negative wire to the B- location.
<img src="/uploads/db1493/original/2X/3/3f9c927986a8d8a3a3bc71080ced102f41748e2a.jpg" width="666" height="500">

After you can go ahead and connect your balance lead to your battery and then connect them all together to the BMS.
<img src="/uploads/db1493/original/2X/3/305b175f0131e5480479e3421534c95077f7f11e.jpg" width="666" height="500">

When you are done you will have your positive lead coming from the battery and your negative lead coming from the BMS.
This will allow you to charge and discharge keeping your battery balanced.

To charge you will need to get a compatible charger(Voltage varies on your LiPo config) and DC-plug to solder... I Soldered all my connections on the a Switch. One side of the Switch has an LCD and the other side had the charger leads.

 

<img src="/uploads/db1493/original/2X/e/e285d82bb63459ab84955c5b509c37db3258f137.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/6/65e4ffc49ce8b93cc9723f796cb4638d683015b9.jpg" width="375" height="500">

After your charger should indicate when your battery is chargeing or full. (Red=Charging, Green=Full)
<img src="/uploads/db1493/original/2X/2/2b1bcb906700c6c940fa0af5ba5a089ee4b8461d.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/7/714c9975dcdf70ecb258f406e5b79d26d6152667.jpg" width="666" height="500">

In the End your build should look similar to this, all that is left is securing the electronics and organizing them on the board to your taste!

<img src="/uploads/db1493/original/2X/3/3aa1f194b1c1e5cfdd9d58de6265d13ad1dc2eaf.jpg" width="666" height="500">

Hope this helps, feel free to ask any questions.

Check out some of the components used in this build at [MiamiElectricBoards.com](http://MiamiElectricBoards.com) !
```

---
## \#2 Posted by: stuxtruth Posted at: 2016-07-15T02:28:22.465Z Reads: 974

```
Where did you get the charger
```

---
## \#3 Posted by: treenutter Posted at: 2016-07-15T03:27:33.111Z Reads: 953

```
@oriol360 thanks for this excellent write-up!
```

---
## \#4 Posted by: Bender Posted at: 2016-07-15T14:06:58.270Z Reads: 936

```
Bookmarked!
I'll be using this soon :beers:
```

---
## \#5 Posted by: Hillso Posted at: 2016-07-15T14:09:23.927Z Reads: 913

```
You can get a similar charger [here](http://www.ebay.com/itm/Intelligent-Smart-33-6V-2A-Charger-for-8S-28-8V-29-6V-Li-ion-Li-Po-Battery-EU-/321471399664?hash=item4ad93046f0:g:YXAAAOSwKIpWBgVj)
```

---
## \#6 Posted by: AugustM Posted at: 2016-07-15T17:24:55.924Z Reads: 885

```
I'll just leave this here ;)
It's my diagram for a 9S Setup, but it's is the same thing!

<img src="/uploads/db1493/original/2X/9/9df4300fce03fb4e05d7b5696b67dd2f44ca6f3b.png" width="690" height="431">
```

---
## \#7 Posted by: oriol360 Posted at: 2016-07-15T18:28:51.023Z Reads: 813

```
The Charger @Hillso  Linked is the charger I bought for 8S
this is the 8S BMS I bought: [Here](http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html)
```

---
## \#8 Posted by: AugustM Posted at: 2016-07-15T18:53:54.468Z Reads: 797

```
@oriol360 What female DC connector did you buy? Your solution seems much better than mine :stuck_out_tongue:
```

---
## \#9 Posted by: Hillso Posted at: 2016-07-15T19:44:25.494Z Reads: 774

```
@AugustM 
http://www.aliexpress.com/item/1Pcs-2-1-x-5-5mm-DC-Power-Female-Plug-Jack-Adapter-Connector-Plug-for-CCTV/32347743787.html?spm=2114.13010208.99999999.267.Ubvzvl
```

---
## \#10 Posted by: oriol360 Posted at: 2016-07-17T07:51:50.650Z Reads: 765

```
I actually got this female DC Jack that comes with a long wire already hooked up ready to solder on to your build:
https://www.amazon.com/Monoprice-Power-Pigtail-Female-Plug/dp/B004OCCARQ
```

---
## \#11 Posted by: Bender Posted at: 2016-07-17T13:32:37.586Z Reads: 725

```
What did you wrap your BMS in?
Shrink tube?
What diameter?
```

---
## \#12 Posted by: oriol360 Posted at: 2016-07-18T15:39:45.207Z Reads: 706

```
I just wrapped it in electrical tape.
It's easier for me, As I don't have to cut out the parts I need exposed.
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-07-18T16:23:14.007Z Reads: 680

```
Glad to see you in here @oriol360 after you basically saved my ass this weekend.
```

---
## \#14 Posted by: oriol360 Posted at: 2016-07-19T21:57:28.950Z Reads: 663

```
@longhairedboy Awesome Man, Glad it worked out for you! Yeah I'm trying to get on more often I just don't have time to post as much as I would like :confused:
```

---
## \#15 Posted by: help Posted at: 2016-07-19T23:14:04.455Z Reads: 645

```
made an account to ask this question. I have a 12s BMS + 50.4v 4A charger. I've wired everything up correctly from what I can tell, but it only charged 6 of the 12 cells to 4.2v, the rest are left at 3.8v. What could be the reason for this?
```

---
## \#16 Posted by: oriol360 Posted at: 2016-07-20T13:56:18.075Z Reads: 631

```
Hey @help,

Do you have any pictures of your setup we could take a look at?
Also what BMS did you get?
Sounds like one of your batteries isn't hooked up properly :confused:
```

---
## \#17 Posted by: Das53 Posted at: 2016-08-07T03:20:58.792Z Reads: 619

```
Hey... I hook...up everything they way I read...and went over it over n over....battery shocks you...thank god they didn't burn up....can u please make a video ...it would be a big help I tried..dude I tried
```

---
## \#19 Posted by: oriol360 Posted at: 2016-08-07T16:43:10.820Z Reads: 618

```
@Das53
Hey can you post pictures of your setup without actually hooking it up, to see where your connections are.
I think you might be connecting your balance plug before connecting the negative terminal. or you might be getting a short somewhere.
```

---
## \#20 Posted by: Das53 Posted at: 2016-08-08T00:18:48.523Z Reads: 624

```
Grab the balance plug was plugged in first...so I should plug in the ..negative lead first...then the balance negative wire....then the positive lead...the the balance?
```

---
## \#21 Posted by: Das53 Posted at: 2016-08-08T19:47:33.334Z Reads: 637

```
When I connect the positive to the bus it shocks up...and the balance leads isn't even connected yet
```

---
## \#22 Posted by: Das53 Posted at: 2016-08-08T19:49:34.716Z Reads: 630

```
<img src="/uploads/db1493/original/2X/6/6ceab9b395714e739e6b2e7ae508dc087197b171.jpg" width="690" height="388">
```

---
## \#23 Posted by: oriol360 Posted at: 2016-08-09T05:44:32.235Z Reads: 628

```
I'm not sure what the schematics are for your BMS 
But, Your positive should not connect to your BMS.
Only the Negative and the balance leads.

You might also have soldered the connections incorrectly. 
The negative should be going into B- and coming out of P-... it looks like you have it the other way around.

Also that positive charger shouldn't be connected there.
```

---
## \#24 Posted by: Bender Posted at: 2016-08-09T11:47:20.238Z Reads: 591

```
This beautiful diagram might help http://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/53?u=bender
```

---
## \#25 Posted by: Das53 Posted at: 2016-08-09T15:35:25.036Z Reads: 588

```
Well ..it helps a little bit...can you take a pic of your bms already hooked up...its my first time ever doing this
```

---
## \#26 Posted by: paragon Posted at: 2016-08-09T16:06:15.772Z Reads: 595

```
this might help <img src="/uploads/db1493/original/2X/d/d161b73a42ffdbe6b999890066df92fac7896483.png" width="690" height="285">
```

---
## \#27 Posted by: Das53 Posted at: 2016-08-09T16:22:41.350Z Reads: 577

```
Well....I know about batteries and their connections...but I never did the bms connections....but if I can get a picture of someone's bms already connected...it would help me lots
```

---
## \#28 Posted by: oriol360 Posted at: 2016-08-09T19:02:59.004Z Reads: 590

```
@Das53
One of the pictures from the OP is the BMS fully connecting.
This one: 
<img src="/uploads/db1493/original/2X/3/305b175f0131e5480479e3421534c95077f7f11e.jpg" width="666" height="500">

You should end up with the positive lead from the battery and the negative lead from the BMS.

From there you would connect you charging cable in parallel. I soldered them to my switch but you can see other diagrams posted above how it's connected. 

<img src="/uploads/db1493/original/2X/e/e285d82bb63459ab84955c5b509c37db3258f137.jpg" width="375" height="500">

There BMS out there that have separate solder points for charging but the one I used, uses the same points for charging/discharging.

Hope this cleared up some things.
```

---
## \#29 Posted by: Das53 Posted at: 2016-08-10T13:26:22.909Z Reads: 528

```
Ok ok....so I should put the one leaf in p....throughe the hole and bring it up through b hole...so p and b..are now using the same lead....and that black lead goes into the esc....and the red lead  that the battery comes with goes in to the esc... .so its really only the balance leads..that goes to the bms...and the negative lead that I solder plugs into the negative esc....and the battery positive goes straight in to the esc? If its so then I understand?
```

---
## \#30 Posted by: Das53 Posted at: 2016-08-14T06:27:34.870Z Reads: 524

```
Ok guys I got it to work....thank you all....20000mah skateboard...8 hour's to charge at 2 amp lol
```

---
## \#31 Posted by: kyo Posted at: 2016-08-14T07:38:53.395Z Reads: 520

```
@Das53. Maybe this helps. 

 https://youtu.be/gnEGYwBa4tk
```

---
## \#32 Posted by: Abdulz Posted at: 2016-08-14T15:23:11.944Z Reads: 517

```
Do you just use the Bms to charge , have you got a link for the Bms as this looks perfect
```

---
## \#33 Posted by: ikjahaa Posted at: 2016-08-14T15:24:23.394Z Reads: 514

```
20Ah ?! what range is that ? lol
```

---
## \#34 Posted by: Das53 Posted at: 2016-08-15T05:15:07.645Z Reads: 505

```
I am 215 pounds.  8s 20000mAh...36t/15t ....it takes me 30 miles.....  I hate to see people post up these calculation crap  that's not true......and my bms is working beautifully...
```

---
## \#35 Posted by: Das53 Posted at: 2016-08-15T05:16:33.213Z Reads: 506

```
The bus I use is this onehttp://m.ebay.com/itm/Balance-BMS-PCM-21A-w-Temp-Switch-for-8S-29-6V-Li-ion-Li-Po-battery-8S21W002-/321790758054?txnId=1622631924011
```

---
## \#36 Posted by: Das53 Posted at: 2016-08-15T05:17:26.801Z Reads: 517

```
<img src="/uploads/db1493/original/2X/8/8550ba73246cf40ac8e752903742e304287ef088.jpg" width="648" height="500">
```

---
## \#37 Posted by: Das53 Posted at: 2016-08-15T05:17:56.403Z Reads: 507

```
Someone made this not me.....this helped me so much lol
```

---
## \#38 Posted by: abenny Posted at: 2016-08-23T18:36:52.999Z Reads: 484

```
i have a similar battery setup to the one that you used as an example in this thread...im going to buy the bms you used, do i need any connectors or anything? or just soldering
```

---
## \#39 Posted by: Das53 Posted at: 2016-08-26T17:05:18.718Z Reads: 476

```
I used a 8s balance leads....and the one the bms comes....like he said one battery you don't remove and wire...and the second one..connect the black balance lead wire to the bms....that's where i messed up....battery charges beautifully
```

---
## \#40 Posted by: oneafrikan Posted at: 2016-08-26T17:15:19.221Z Reads: 505

```
For the newbies like me: could you perhaps post a parts list?

Eg: can figure out the battery, but BMS, switches, etc are harder to identify from photos. 

;-)
```

---
## \#41 Posted by: oriol360 Posted at: 2016-08-26T18:07:25.022Z Reads: 521

```
@abenny Yup just mainly soldering.  But like @Das53 Said the connector that came with the BMS.
```

---
## \#42 Posted by: Heavy1 Posted at: 2016-08-26T18:30:13.814Z Reads: 499

```
So do you plug in your charger and then turn the power switch on to act as your anti spark? Is your board then on whilst you charge?
```

---
## \#43 Posted by: oriol360 Posted at: 2016-08-26T18:37:47.990Z Reads: 510

```
Parts List:

BMS: http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html

Battery: http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=56840

Charger: http://www.ebay.com/itm/Intelligent-Smart-33-6V-2A-Charger-for-8S-28-8V-29-6V-Li-ion-Li-Po-Battery-EU-/321471399664?hash=item4ad93046f0

Power Switch: http://miamielectricboards.com/shop-1/120amp-12s-power-switch

Used These to make the 4S to 8S adaptor: http://www.ebay.com/itm/10pcs-JST-XH-4S-Connector-Adapter-Plug-W-Wire-For-4-Cell-14-8V-Lipo-Battery-/111578260237?hash=item19fa95230d:g:jHAAAOSwx~JWEz1q
```

---
## \#44 Posted by: oriol360 Posted at: 2016-08-26T18:44:06.575Z Reads: 490

```
You dont have too. The switch supports regenerative power. So power can flow back to the battery without the switch being on. It will still act as an anti spark.
Other BMS have a chargingnterminal what would be wired differently. 
This was just for the BMS that i used.
```

---
## \#45 Posted by: Heavy1 Posted at: 2016-08-26T18:49:24.257Z Reads: 472

```
Yeah nice, is that switch something you had custom made? 

Would a bms that had a charge terminal still only pick up the battery negative directly to the bms and have the balance lead positive still being the only positive connection to the bms?
```

---
## \#46 Posted by: oneafrikan Posted at: 2016-08-30T23:09:52.264Z Reads: 468

```
quick question:

i accidentally touched the black cable to another black cable, whilst chatting to my wife about our holiday.
big spark. i shat myself.

[lesson: don't discuss toddler travel tactics with your wife whilst trying to connect batteries.]

should i expect everything on that circuit to be fried, or should it be ok once i connect everything up the right way?
will the battery still be OK?

have ordered a multimeter which arrives tomorrow, so going to use that to check the various connection points to see whether anything else is shorted / buggered, but wondering whether i'm wasting time / have to think about anything else... ?
```

---
## \#47 Posted by: oriol360 Posted at: 2016-08-31T03:49:21.301Z Reads: 445

```
@Heavy1 Nope it's pretty much the same as all the other power switch on the market. as for the BMS there are a couple different ones. some can integrate both positive and negative terminals for charger, others are just negative. you would have to look at the schematics for the BMS you purchase.

@oneafrikan depends. Look around you bms.. if anything is burn or swollen or just smells really bad the bms is probably ruined. the multimeter will be a great tool to check if your batteries are still being balances by your bms. I would be careful in using it though, you do not want it to ruin your batteries further. a shoer can really hurt your batteries.
```

---
## \#48 Posted by: oneafrikan Posted at: 2016-09-01T00:16:05.338Z Reads: 423

```
@oriol360 - how would you ruin the batteries with a multimeter?
```

---
## \#49 Posted by: oriol360 Posted at: 2016-09-01T02:41:07.706Z Reads: 410

```
Sorry, I meant careful using the BMS.
```

---
## \#50 Posted by: Mikee Posted at: 2016-09-01T03:29:35.963Z Reads: 410

```
@oriol360 What kind of hubs are you using for this build?
```

---
## \#51 Posted by: oneafrikan Posted at: 2016-09-01T13:19:53.019Z Reads: 413

```
gotcha, thanks.
```

---
## \#52 Posted by: Das53 Posted at: 2016-09-09T20:46:02.193Z Reads: 406

```
I didn't want bother with power switch...so I chose hobbyking esc...8s....is alot of power and speed
```

---
## \#53 Posted by: Tijmen Posted at: 2016-12-14T19:30:51.489Z Reads: 365

```
Would there be a way to bypass the max discharge limit on this BMS? I might be wanting to hook up a motor with a higher max rating than 60A. Is there a way to do this?
```

---
## \#54 Posted by: DreadBiscuit Posted at: 2016-12-14T23:31:01.582Z Reads: 367

```
@tijmen, The way I did it was to simply not hook up the battery negative to the P- terminal.  Instead simply wire the VESC (or switch) negative directly to the battery negative.  Hope this helps.
```

---
## \#55 Posted by: flatsp0t Posted at: 2016-12-15T07:28:33.492Z Reads: 373

```
I just want to add, even if the max rating of the motor is higher, i doubt you will ever use this much.
I would recommend trying it out, before bypassing the BMS.
```

---
## \#56 Posted by: Tijmen Posted at: 2016-12-15T11:51:56.700Z Reads: 391

```
So what you're saying is that when using the system, the batteries would be hooked up directly to the ESC or switch, but when charging the power would go from the BMS, back through the ESC and then into the batteries?
And good idea about the max amp draw. The motor I'd be getting (not sure on which one), will most likely only be 5 amps more than the max draw limit of the BMS
```

---
## \#57 Posted by: DreadBiscuit Posted at: 2016-12-15T13:01:55.234Z Reads: 405

```
@ flatspot is absolutely right, you probably won't pull that many most of the time.  I bought a very cheap bms for now which is only rated at 15amps discharge.  So I went ahead and bypassed it.  I updated @oriol360's original post showing how he wired to illustrate how you would bypass the discharging function but still allow for charging of the batteries.  No electrons pass through the vesc when charging on the way to the battery.  I hope this helps.  Forgive my crude MS paint editing methods.   <img src="/uploads/db1493/original/3X/6/1/61994640faaf599f99f4a08dda5adf23ab73c571.jpg" width="666" height="500">
```

---
## \#58 Posted by: Cuprani Posted at: 2017-02-13T23:48:12.009Z Reads: 416

```
Could anyone please advice with the following setup?

I have a 12S setup with 3 lipo's of 4S.
I have [this](http://s.aliexpress.com/Vn6JFfUj) BMS
I use a simple 50,4V charger

I only want to use my BMS for charging. Not for discharging.

Is this the correct setup? Will it work correctly?
[img]https://sites.google.com/site/nilsvdg2/home/20170214_002021.jpg[/img]

Also I have a question about the balance leads.

I have a 4S lipo, with a 5-Pin balance connector.
The first is red and is off course positioned before the first cell. The last is black and is positioned behind the last cell.  The other three are between each cell.

That's 15 balance wires in total for the Lipo's 

The BMS has 12 balance wires.
And 2 negative connectors on board. B- and P-.

The charge port connects to the P-, and the + of battery 3.

I assume that's why I can discard the red wire from the balance cable from te lipo (the first pin) and use pin 2,3,4,5 from Lipo Nr3 for the first 4 balance wires from the BMS.

As pin 5 from lipo 3 is the same as pin 1 from lipo 2 I can again discard the red wire (pin 1) from lipo nr2' balance connector en connect pin 2,3,4,5 with the BMS balance cables 5,6,7 and 8.

For the last lipo (lipo one) I can again discard the red balance wire (pin one). Pin 2,3,4 will connect to wire 9,10 and 11 from the BMS. 

What should I do with pin 5 from Lipo 1?
1. Should I connect this to cable 12 from the balance wires? 
2. Or to B- of the BMS? 
If I choose option one, do I need to connect B- to the black main cable of Lipo 1, or could I just ignore that connection?
```

---
## \#59 Posted by: Namasaki Posted at: 2017-02-14T02:39:25.505Z Reads: 393

```
A 4s Lipo has 5 balance wires:
Black = ground
color= cell 1
color= cell 2
color= cell 3
Red= cell 4
This is the standard for all Lipos.
Black is always ground and Red is always the Last cell in the pack.
A hobby charger uses the ground wire from the pack
your bms does not use the black balance wire but uses the main ground instead, that is why it only has 12 pins for 12s.
Here is a diagram of how I connected five 2s Lipos in series to a 10s bms:
It's not the same setup your doing but the principle is the same.
<img src="/uploads/db1493/original/3X/8/b/8b17159038497ac9b8207b616799b74d28b5a0cd.png" width="665" height="500">
As you can see, you don't omit any of the red balance wires and you omit all of the black balance wires.
```

---
## \#60 Posted by: Namasaki Posted at: 2017-02-14T02:57:20.046Z Reads: 372

```
Your bms is rated for 60a and can handle discharge as well as charge.
You really should use it for both. Your Lipos will have more protection that way.
if you do charge only, you will need to connect the pack ground wire to B- because the bms uses that as ground for the balance wires.
```

---
## \#61 Posted by: Cuprani Posted at: 2017-02-14T06:29:30.316Z Reads: 384

```
So instead of discarding the first pin of the lipo balance (the red wire), I shouldn't connect the last pin (black) to the balance wires and use the red one.

Really think it ain't necessary to use the BMS for discharge as the VESC is set to a safely cut off at low voltage.
```

---
## \#62 Posted by: Cuprani Posted at: 2017-02-15T08:12:13.500Z Reads: 391

```
@Namasaki
Just to make sure, if I alter your scheme to this, it should work fine charging the lipo's with the BMS and discharging them without.

[img]https://sites.google.com/site/nilsvdg2/home/BMS%20in%20parallel.jpg[/img]
```

---
## \#63 Posted by: nmagz3 Posted at: 2017-02-15T08:18:43.921Z Reads: 353

```
 @oriol360 Bro!  Thanks so much for this post :slight_smile: You and @Namasaki have the most straight forward explanations for the BMS.  Bookmarked :calling:
```

---
## \#64 Posted by: Namasaki Posted at: 2017-02-15T13:29:45.461Z Reads: 360

```
I have never bypassed the BMS on discharge myself but I think it will work the way you have it.
I was mainly showing how to connect the balance wires.
Note: Some BMS's have a ground port in the balance plug in which case you would use the the black balance wire from pack number one.
Note: I'm not sure about port N-  never seen that before. Just make sure that is for charge neg. 
if not, I think you'll need to connect charge neg to B-
Then again I'm not positive about bypassing. 
Frankly I don't recommend bypassing but rather spend the money for a BMS that will handle discharge. You'll be glad you did. 
My advice is, never skimp on batteries or electronics.
```

---
## \#65 Posted by: Namasaki Posted at: 2017-02-15T17:05:08.104Z Reads: 366

```
[quote="Cuprani, post:61, topic:6122, full:true"]
So instead of discarding the first pin of the lipo balance (the red wire), I shouldn't connect the last pin (black) to the balance wires and use the red one.

Really think it ain't necessary to use the BMS for discharge as the VESC is set to a safely cut off at low voltage.
[/quote]
The red wire is always the balance wire for the last cell in pack. 
The black wire is always ground, not a balance wire.
Most BMS's use main ground for balance. That's why they don't have the extra pin. 
Although the red and black wires are connected between packs in series, use the red wire for balance and omit the black wire for a more direct route to the cell being balanced. 
It's better to discharge through the BMS because the Vesc only monitors total pack voltage so you could possibly have one cell drop bellow safe voltage before the Vesc would shut down.
A BMS monitors the voltage of each cell or parallel cell group providing better over discharge protection. 
Not only that, it will also protect against over charging by regen braking. I'm not sure that's the case when you bypass. 
Also the BMS will protect against shorts if use for discharge. 
I did actually short my battery once wile the BMS was on and it's short protection tripped and shut the system down in an instant so nothing was damaged. 
Not the BMS, not the Vescs, not even the battery. 
This is why I say, don't skimp, buy a quality BMS with high amp capability and wire it for charge/discharge. 
In the long run you'll be glad you did. 
Or, you can buy a cheap BMS  like this guy. 
http://www.electric-skateboard.builders/t/bms-broken-again/17693
```

---
## \#66 Posted by: Namasaki Posted at: 2017-02-15T17:11:15.047Z Reads: 315

```
This is what I've been using since last summer and I have had no problems at all with them. 
http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html
```

---
## \#67 Posted by: Tobi Posted at: 2017-02-15T18:03:34.523Z Reads: 319

```
how to order on bestechpower ?
```

---
## \#68 Posted by: Namasaki Posted at: 2017-02-15T18:48:25.430Z Reads: 330

```
Send an email to 
lucy@bestechpower.com
Requesting to purchase the BMS by model number. 
They will complete the transaction by email. 
They accept Paypal and their minimum order requirement is 2. 
Total cost for 2 of the bms's I use with shipping to USA was about $136
It's really a good deal considering that they have a built in HV e-switch saving up to $60 on your build
And they easily handle 80a continuous and up to 240a peak current discharge and 20a charge.
Note: I'm pretty sure they ship to EU as well.
```

---
## \#69 Posted by: Cuprani Posted at: 2017-02-16T19:04:49.928Z Reads: 334

```
@Namasaki
Thanks for the advice, only too late for me :slight_frown:
My BMS is already broken.

I have the BMS from battersupports.com (12S 60A) which is used a lot here with positive feedback.
I already have a high voltage switch. If I new about this BMS with build in switch before, I would have definitely gone for that. 

I use my BMS now with three 4S lipo's.
I wired my cables and connectors and tested the BMS with a volt meter.
Black on B- and than I've tested the balance wires one by one.

At the sixt pin (in the middle of the connector for battery two) it didn't measure any current. All further pins no current either. I've tested my wiring and those are good for 100% sure. Really think it came in broken, never even used it. I will open a dispute at AliExpress and I will ask them to send me a new one. Right now I will use my Turnigy balance charger (1S to 6S) to charge the battery's balanced in parallel till I receive my new BMS.
```

---
## \#70 Posted by: Namasaki Posted at: 2017-02-16T20:43:01.751Z Reads: 302

```
The balance current on the Bestech is only 126ma
I'd imaging that's it's similar on the battery supports. 
Possibly your meter isn't set for that low of a reading. 
Therefore showing zero
Also balancing happens at the end of charge cycle so there may be nothing wrong with your BMS

Note: I just checked and the Battery Supports BMS balances at 60ma
```

---
## \#71 Posted by: willpark16 Posted at: 2017-02-17T01:51:19.910Z Reads: 291

```
What was ur quoted price
```

---
## \#72 Posted by: Namasaki Posted at: 2017-02-17T02:15:21.904Z Reads: 303

```
$136.50 for 2 with shipping and PayPal fee.
```

---
## \#73 Posted by: willpark16 Posted at: 2017-02-17T02:49:18.502Z Reads: 302

```
Hmm alright thanks man!
```

---
## \#74 Posted by: ofekp Posted at: 2017-04-15T20:27:29.306Z Reads: 293

```
Hey man,
Why is your charger connected in parallel to the VESC? Is that correct?
I think the **VESC's negative** should be connected to **B-** and the **chargers's negative** is the only thing that should be connected to **P-**
Am I correct? Have you figured it out yet?
Thanks!
```

---
## \#75 Posted by: NeverStopSeeking Posted at: 2017-05-05T07:52:56.403Z Reads: 277

```
Hi, i am reading you for a long time and finally decided to make my electric skateboard.

About BMS i have some questions if anyne is so kind to reply or to redirect me to the topic where you already talked about it:
1-  In a configuration of 2 3S Battery  to create a 6S battery can i use 2 separate 3s BMS for each battery connected in parallel to the charger port?  ( for time reason, I can not find on ebay europe a 6s bms) 

2- When i will connect the power suply/charger to the bms, it will automatically drain the max current the bms can take and /or the charger can give? ( to estimate charging times)

3- What voltage power supply should i get for a 3s BMS ?
 and what voltage power supply 6s BMS if i decide to take this one? 
i can not find the max voltage the bms board take, only max current ...:disappointed_relieved:

4- Anyone know where to buy cheap BMS and power supply in europe?

If i said some eresy please forgie me :sweat_smile:
```

---
## \#76 Posted by: facepalmsareus Posted at: 2017-07-14T18:49:20.876Z Reads: 227

```
Does anyone know why a bms might drop voltage? I have mine wired up like in this post but it for whatever reason my bms drops voltage accross it now (it did not a week ago) to the point where it cannot even get my vesc to turn on. I thought about bypassing it by simply running a wire from the B- to the P-. Does anyone know if that wold work?
```

---
## \#77 Posted by: Sapphirinia Posted at: 2017-07-28T02:15:01.946Z Reads: 222

```
Does the e switch mean I can easily hook up a on off switch to it without adding anything else?
```

---
## \#78 Posted by: mmaner Posted at: 2017-07-28T02:26:51.784Z Reads: 220

```
If you are referring to the BeaTech BMS's then yes.  They come with leads to connect a switch.
```

---
## \#79 Posted by: Namasaki Posted at: 2017-07-28T02:29:01.567Z Reads: 220

```
any 12v 2 pole automotive switch will work as long as it is not a momentary switch
```

---
## \#80 Posted by: SilentException Posted at: 2017-07-28T10:14:48.102Z Reads: 225

```
Well, technically you _could_ use momentary switch but you will have to hold it pressed while riding :grin:
```

---
## \#81 Posted by: Sapphirinia Posted at: 2017-08-28T13:42:07.678Z Reads: 218

```
Looks like it'll take forever to get hose adaptors. Can I do it without them?
```

---
## \#82 Posted by: Sapphirinia Posted at: 2017-08-29T18:24:23.588Z Reads: 216

```
Fail... <img src="/uploads/db1493/original/3X/6/e/6e0a33623a22dd46c044d1c83e85ae86c6325c5d.jpg" width="375" height="500">
```

---
## \#83 Posted by: flywithgriff Posted at: 2017-08-29T18:25:04.157Z Reads: 212

```
What is this??
```

---
## \#84 Posted by: Sapphirinia Posted at: 2017-08-29T18:28:18.103Z Reads: 209

```
Trying to wire up the bms. Was trying to switch the connection from the 4s battery to the 8s BMS. I was having a hard time getting the 3rd wire in so I used tweezers to pull it back out and accidentally touched 2 together and now I hope I didn't destroy the battery.
```

---
## \#85 Posted by: flywithgriff Posted at: 2017-08-29T18:34:33.447Z Reads: 208

```
It shouldn't have damaged the battery. Thats tough luck though.
```

---
## \#86 Posted by: BenTheBarre Posted at: 2018-02-10T23:44:55.334Z Reads: 177

```
Hey oriol, 

Is it necessary to solder one ground Lead from one pack to the negative terminal of the bms? What will happen if this is not done, and both ground leads are cut?
```

---
## \#87 Posted by: tojo Posted at: 2018-03-21T12:06:07.583Z Reads: 172

```
Hi man
Your diagram look right, but the charger don't cross over the bms, so i don't understand this point. Can you help me to understand please ? 
The black wire of the charger will be on the P- of the BMS  ?
If i have a B1- on my bms (7pin for 6s), Do i have to take also the same wire (balance cable) to connect to the B- of the BMS ? Does the last pin served to something ?

Thanks a lot!
```

---
## \#88 Posted by: tomerwei Posted at: 2018-04-04T20:24:37.695Z Reads: 165

```
Sorry for the beginner question, but can someone show a pic on the exact way to connenct the BMS to the Charge port. and do you know if this port is good enough:
https://www.ebay.com/itm/1pc-Iron-5-5x2-1mm-DC-Power-Female-Jack-Socket-with-Waterproof-Cover-Ring/221909154788?_trksid=p2485497.m4902.l9144

Thanks!
```

---
## \#89 Posted by: DullElysium Posted at: 2018-04-15T06:11:24.337Z Reads: 166

```
I'll just hijack this since I don't want to make a new thread for every question I have.

I just wired up my BMS and when I tried to connect my charger to the setup I got a big spark that scared the shit out of me. 

I'm just wondering if I got something wrong

This is how I have everything wired up. I excluded further connections since they were not connected to anything at the moment. Just tried to check that my setup can charge.

![BMS wiring check|267x500](upload://sTUtTVWcbjDLdOpTQyee31d4Z8l.jpg)

Oh and I used a charger from a hooverboard that I have.
Input: 100-240VAC, 50/60Hz 2A
Output: DC 42V 2A

This should be ok, no?
```

---
## \#90 Posted by: MannyM0E Posted at: 2018-04-15T06:40:15.651Z Reads: 156

```
Make sure that your charger port wire on the tabs are correct. I had one that had black wire onto positive tab and the red wire into the negative tab.
```

---
## \#91 Posted by: DullElysium Posted at: 2018-04-15T07:43:06.415Z Reads: 152

```
Yeah i actually had to change the tip on my adapter for a regular dc-style plug and everything should be correct on both ends. Plus on the inside and so on. The female part has three connectors though, where one of the pins seems to be a contact switch. Atleast there’s connection between two of the outer pins until a plug is inserted.

I’ll have to double check the positives and negatives before next try, but i’m curious if there’s more possibilities as to why there’s a spark. I should be able to connect the charger with no anti spark-connectors in that loop, am I right?

EDIT:
Ok, upon further investigation, it seems that the female plug I have has this contact-switch inside and I have wired my negative lead to it. The burn marks on my male connector lead me to the conclusion that the switch-contact was pressed so tightly in that it's not in contact with the positive of the female plug but it will be in contact with the positive of the male plug when trying to plug in. So it seems that my problem was a short circuit after all.
```

---
## \#92 Posted by: Hendrix Posted at: 2018-05-13T01:50:30.245Z Reads: 139

```
my  lithium ion batterys have stopped charging is there any reason that could have happend
```

---
## \#94 Posted by: Matrom Posted at: 2018-07-25T21:53:03.364Z Reads: 116

```
Great post! Thank you.
Do you think that [this bms](https://m.aliexpress.com/item/32840727181.html?pid=808_0000_0201&spm=a2g0n.search-amp.list.32840727181&) works the same way, except that it is labeled -C where you have -N?
```

---
## \#97 Posted by: Thatdudedominic Posted at: 2018-11-03T05:06:35.835Z Reads: 95

```
Why does my bms (12s) have 13wires and not 12
```

---
## \#98 Posted by: Andy87 Posted at: 2018-11-03T13:08:30.307Z Reads: 100

```
Depending on the bms you have it can be that you need to connect on of the leads to the battery minus.
Which bms you have?
There where no schematics delivered with your bms?
```

---
## \#99 Posted by: Thatdudedominic Posted at: 2018-11-03T13:26:34.377Z Reads: 106

```
![image|281x500](upload://hHKoZQtXq2LqPUKd4oGNRKFSJtc.jpeg) ![image|281x500](upload://s5Dgy5LWG1SDotKRbBr8YOsHnuC.jpeg) ![image|375x500](upload://w3UtTJs8UOmj4GlN99WQaWS7Ni3.jpeg)
```

---
## \#100 Posted by: Andy87 Posted at: 2018-11-03T13:30:58.212Z Reads: 92

```
You can see, first pin is b-
If you have a multimeter you can check if the b- pin is connected to the B- terminal on the pcb.
Sometimes it’s like this and than you don’t need to connect the first balance wire to your battery
```

---
## \#101 Posted by: Thatdudedominic Posted at: 2018-11-03T13:35:37.990Z Reads: 96

```
So the b- is going to the first neg then all the rest are pos
```

---
## \#102 Posted by: Thatdudedominic Posted at: 2018-11-03T13:47:51.045Z Reads: 101

```
Hope this is correct
```

---
## \#103 Posted by: Andy87 Posted at: 2018-11-03T13:58:13.855Z Reads: 112

```
The drawings you got a bit confusing me.
Looks like the drawing is upside down to the pcb.
You wire it up for charge only?
My d140 is wired up like this
![image|569x500](upload://pWoSoxgw5rSptUYnulwiIHKMTYG.jpeg) 

In my case the b- and the B- are on the pcb connected. So no need for the first lead to be connected to the first pack minus.
If that’s not the case with your bms than you need to connect the first lead to the first pack minus.
From lead b1 the leads gonna be connected  between cell 1 and 2.
If you connect the balance lead on the plus of pack one or minus of pack 2 doesn’t matter.

If you have a time @b264 please have a look too that I don’t tell something totally wrong.
```

---
## \#104 Posted by: b264 Posted at: 2018-11-03T19:00:20.919Z Reads: 112

```
*It depends totally on the specific BMS* but in most cases if you aren't discharging through the BMS, you can leave B- unhooked if it's connected to B0 in the balance leads.  But if you have the load connected through the BMS, you'd need to do it the other way like your image above.
```

---
## \#105 Posted by: Rotti Posted at: 2018-11-03T19:20:59.105Z Reads: 112

```
I have just finished wiring up my BMS and i tried charging my board with it.
Everything seemed to be working, the light of my charger turned red and my battery indicator showed that the percentage of the battery was going up.
But then my battery indicator reached 100% but the light of the charger did not turn green. Is my BMS still balancing or what is the problem  here? I am a little worried to overcharge my battery, so i unplugged the charger for now.
Or is my charger never turning green, because my ESC consumes power from it, because the ESC and the charging port are wired in parallel?
```

---
## \#106 Posted by: Andy87 Posted at: 2018-11-03T19:25:41.305Z Reads: 112

```
Most bms just balance when reached 4.2v.
Plus check if your battery indicator is set to the right voltage. Usually they multi voltage indicators which need to be set to the right max voltage.
If you have a multimeter you can check the actual voltage of your pack to make sure all is good.
```

---
## \#107 Posted by: Gabegds2001 Posted at: 2018-11-08T03:05:56.426Z Reads: 105

```
I have 4x3s batteries in series and am wondering which balance wires actually connect to the bms because there are 4 coming out of the battery but only 3 are used??
```

---
## \#108 Posted by: b-rad Posted at: 2019-01-24T21:01:22.276Z Reads: 92

```
[quote="Namasaki, post:64, topic:6122"]
Some BMS’s have a ground port in the balance plug in which case you would use the the black balance wire from pack number one.
[/quote]

How do you know if your BMS has a ground port in the balance plug? if so would you use the negative balance wire first then for the next 4 packs use the positive wire first? im using this 12s BMS from battery supports. 

Should i hook up the BMS using all positive leads first based on this BMS?

http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html
```

---
## \#109 Posted by: J_Dizzle Posted at: 2019-01-24T21:29:06.371Z Reads: 83

```
Yes you balance plug has a ground pin, you can tell because you have 12 positive balance wires on the plug(one for each cell) and then there is a thirteenth wire on the left. you can leave this wire unatatched, because you will be connecting that negative balance wire to your B- port on the bms. I'm assuming you are discharging through the BMS, although the wiring will be that same whether you discharge or bypass the bms
```

---
## \#110 Posted by: b-rad Posted at: 2019-01-24T21:37:34.565Z Reads: 81

```
No my BMS has only 12 balance wires
```

---
## \#111 Posted by: J_Dizzle Posted at: 2019-01-24T21:40:22.461Z Reads: 86

```
?? the one you linked has thirteen. Either way, you connect all 12 positive balance wires the the 12 pin connector in order, and attatch your negative balance wire to the B-
```

---
## \#112 Posted by: b-rad Posted at: 2019-01-24T21:56:04.224Z Reads: 89

```
Oh im sorry i ment to send the 12s 100a version same bms just 12s.. ive attached the link below..

so can i just follow this diagram for my 12s battery supports BMS? 

![aq|566x428](upload://bqmuJcwTSlK679gtXoemMwOk6ty.png) 



http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html
```

---
## \#113 Posted by: J_Dizzle Posted at: 2019-01-25T04:51:12.473Z Reads: 86

```
Yes. Are you discharging through it or bypassing? This diagram isn’t accurate for discharge BMS
```

---
## \#114 Posted by: Namasaki Posted at: 2019-01-25T05:07:45.064Z Reads: 86

```
The above diagram is a modified version of the original below.

The Battery Supports also know as Supower bms does not have a ground pin on the balance connector port.
It also does not have a separate pad for charging ( C-)
You will connect 
the charge negative wire to the (P-) pad.
The battery negative wire to the (B-) pad
The battery negative wire to the ESC for bypass bms or The Esc negative wire to the (P-) pad for discharge bms
Battery positive goes straight to the ESC positive and charge port positive.


![41%20PM|664x500](upload://avkTxlFxXbBUxFcv2lDo3KSP8tA.png)
```

---
## \#115 Posted by: GUAN1111 Posted at: 2019-03-16T13:54:41.219Z Reads: 72

```
Hi, I have built a electric longboard. I used it one summer but I wanted to upgrade. It was a hazel to unplug the battery's every time and plug them in to the balance charger.

Therefore I decided to add a BMS, 3 pin charge port and a small battery presenting indicator for easy use.. I decided to bypass BMS. I started with wiring the cables like the picture below, but forgot plug in the motor ore the balance wires to the battery's(I did not plug in the XT-90). When I plugged inn my charger the BMS became super hot(to hot to touch). I though it was because my battery balance leads were not plugged inn. Therefore I plugged in my balance leads and tried again. This time the 3 pin charge port and the charger welded together. Then I plugged in the XT-90 to complete the main circuit. This was a bad decision on my behalf, because the battery's started to expand, my cables and connecters started to smoke, and the VESC MOSFETs melted through the heat shrink. This lead to all my electronics getting destroid. :-(

I believe the wiring is the problem. I did not have the motor plugged inn. Can this have an effect on what happened.

Can anyone please take a look at my wiring an tell me what I have done wrong. Thanks ;-)
![Untitled|690x360](upload://1ur6wV5qy1K3UuoWIg1mtVwKQeo.jpeg)
```

---
## \#116 Posted by: ZachTetra Posted at: 2019-04-01T01:14:25.451Z Reads: 69

```
Looking for help with people who bought a D140 through li-tech.  Does the 12s unit have a 9 pin and 4 pin or 2 9 pins with the last 5 of the second set unused?  Pictures on the forum show 9 and 4 but the site shows 9 and 9

http://www.litechpower.com/product-detail/HCX-D140LI12S15A-05.html#
```

---
## \#117 Posted by: ryanrauch Posted at: 2019-06-16T04:47:55.371Z Reads: 39

```
if you connected 5 more lipo batteries in parallel to this diagram, does each battery share all of the connections with one of the existing batteries?

I'm a little confused about how to connect the bms to a set of lipo batteries that are both in series, and in parallel.
```

---
## \#118 Posted by: Namasaki Posted at: 2019-06-16T16:34:10.350Z Reads: 36

```
[quote="ryanrauch, post:117, topic:6122"]
does each battery share all of the connections with one of the existing batteries?
[/quote]

Yes, you parallel the main and balance connections
```

---

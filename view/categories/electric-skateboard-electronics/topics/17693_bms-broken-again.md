# Bms broken again

### Replies: 37 Views: 3003

## \#1 Posted by: Tobi Posted at: 2017-02-14T16:25:20.248Z Reads: 271

```
hi, for 1 year i builded my own electric longboard with a 10s3p lithium ion (lg He4)
in this time my bms has broken 3 times.

as bms i used 

this one 

http://www.ebay.de/itm/36V-Batterie-Schutz-BMS-PCB-Board-fur-10-Packs-Li-ion-Cell-Max-40A-Balance-/131504012429?hash=item1e9e3ffc8d:g:NQ8AAOSwEeFVSH8X

i pulled and charged through bms they never lasted 3 monthes ...

as tutorial for my battery i used ;

http://www.e-sk8.fr/forum/viewtopic.php?f=8&t=649

why my bms always breaks ? all balance wires are 100 % correct i checked several times. maybe it´s because of it does only support 40 amps discharge ?

what bms would you suggest ? iam german so pls excuse my english.

greets
```

---
## \#2 Posted by: Namasaki Posted at: 2017-02-14T16:56:20.710Z Reads: 253

```
Stop throwing your money away on cheap bms's from eBay and buy a quality BMS from either battery supports or Bestech. I've been using Bestech since July 2016 with no problem.
```

---
## \#3 Posted by: Tarzan Posted at: 2017-02-14T17:02:23.271Z Reads: 245

```
You could bypass the bms for discharging and only use it for charging.
Since you used quality cells, drifting shouldn't be a problem.
If you pull 50 amp through a 40 amp BMS the breakdown is programmed!
```

---
## \#4 Posted by: Tobi Posted at: 2017-02-14T17:57:26.226Z Reads: 232

```
what bms is used in space cell ?
```

---
## \#5 Posted by: mkd Posted at: 2017-07-09T14:12:24.099Z Reads: 205

```
How can I bypass the bms for discharging? Do you have a wiring circuit?
```

---
## \#6 Posted by: rich Posted at: 2017-07-09T16:09:41.782Z Reads: 203

```
@mkd 

BMS B- to BATTERY MINUS
BMS C- to CHARGE PORT MINUS
BATTERY PLUS to CHARGE PORT PLUS

Discharging is connected to the battery directly. You need additional plugs or soldered cables on battery plus and minus. In my case i soldered short cables with bullet connectors to my anti-spark input ports. I plugged it just for this picture so you can see how it looks.

<img src="/uploads/db1493/original/3X/c/c/cc0ed9b11e677e31a281db4a1306106e357d6ca0.jpg" width="690" height="388">
```

---
## \#7 Posted by: mkd Posted at: 2017-07-10T06:22:30.671Z Reads: 189

```
@rich 
Thank you very much :)

Is it possible to bypass this bms for discharging as it uses the same port for charging and discharging?
BMS: https://hobbyking.com/de_de/6s-li-ion-10a-pcm.html

<img src="/uploads/db1493/original/3X/7/0/702a8db65b947f037edc97479808dd7557a57859.jpg" width="690" height="219">

And another question I've got: Is it possible to use a XT90 to split my positive wire into two ?

Thanks for your help !!
```

---
## \#8 Posted by: rich Posted at: 2017-07-10T14:51:13.223Z Reads: 174

```
You are welcome @mkd! 
Of course you can bypass this BMS as well. 
Do you use Lipo or Li-ion? 
Which Setup do you use in general? 
Which charger?
Which way you connect discharge ( on/off switch, key loop, XT90 Antispark)?

Hehe, some questions but otherwise it's hard to help.....
```

---
## \#9 Posted by: mkd Posted at: 2017-07-10T15:28:20.153Z Reads: 173

```
@rich

Thats good news.

I use two of these Lipo in Series (5800mAh / 6S): https://hobbyking.com/en_us/turnigy-5800mah-3s-25c-lipo-pack.html

The charger I want to use (24V / 6,25A / 150W): https://www.amazon.de/gp/product/B01MFFDI1Z/ref=ox_sc_act_title_1?smid=A2Z54WBF904K0X&psc=1

I want to use a XT90 Antispark to connect discharge.

The picture shows how everything is supposed to be wired (I wanted the system to be modular): 

<img src="/uploads/db1493/original/3X/b/6/b61aff142e867877708f497aba2378bf7c24b286.jpg" width="690" height="389">

Hopefully I could answer all your questions. 

Do the parts fit together and is the wiring circuit correct? 

Thanks for your help :slight_smile:
```

---
## \#10 Posted by: rich Posted at: 2017-07-10T19:27:10.612Z Reads: 166

```
Do you plan a huuuuuge enclosure? Too much connectors here... :joy:
I don't like XT90 connectors at all, they are too big and you don't need them, also you can't bend the cables the way you like (the same problem with XT60).
I prefer single bullet connectors so you can route the cables any direction. I like 4mm bullet connectors (90A), the same as in XT90 but nice and compact, or 5,5mm bullets (140A but big).

But one picture speaks more than 1000 words....

<img src="/uploads/db1493/original/3X/b/b/bb9fef11d11e7b6fb60619ff7a044465ee87499f.jpg" width="690" height="388">

Ok, first of all, your wire diagram shows discharging through the BMS, THIS IS NOT BYPASSED and you would damage your tiny BMS immediately, or at least it would shut off everytime when you pull the throttle!! You need to connect discharge minus to battery minus, now it's only connected to C- /P- on BMS.

Like this:

<img src="/uploads/db1493/original/3X/6/7/67c9d720fd22ee08e838d5ec5ba26ba30ef557a4.jpg" width="690" height="388">

You can plug plus of Lipo 1 directly to minus of Lipo 2, this is what i do, it's 5,5mm bullet male/female.
If you put BMS and charging port in the battery section you can save cables and space.
5,5mm bullet connectors for charging cables is way too much, i use 3,5mm (still too much). And 18AWG wire for charging and BMS connections is enough.

I think you'll use to much cables, keep it short.

[quote="mkd, post:9, topic:17693"]
The charger I want to use (24V / 6,25A / 150W): https://www.amazon.de/gp/product/B01MFFDI1Z/ref=ox_sc_act_title_1?smid=A2Z54WBF904K0X&psc=1
[/quote]

DON'T USE THIS POWER SUPPLY!!!!!!!!!!!
YOU NEED 25,2V LI-ION CHARGER, this is something different.

Also you need a fuse for safety.
I don't trust Loop keys and you should buy an anti spark switch. 
Esk8.de sell them for 29,90 free shipping, including fuse.
It's so nice to have a switch!!!

It is dangerous to play around with Lipos and BMS, just one wrong cable and you could get in troubles :wink:
```

---
## \#11 Posted by: chiskate Posted at: 2017-07-10T19:58:53.126Z Reads: 146

```
It's probably overheating. Need a heat sink on those MOSFETs (big ICs). That's why they left nice big holes for you!
```

---
## \#12 Posted by: chiskate Posted at: 2017-07-10T20:00:55.379Z Reads: 141

```
Yours will probably fail like OP's - those MOSFETs need to be able to dissipate heat when under load!
```

---
## \#13 Posted by: rich Posted at: 2017-07-10T21:40:50.023Z Reads: 136

```
What do you mean? A bypassed BMS should not get warm when discharging because there is no load.
```

---
## \#14 Posted by: chiskate Posted at: 2017-07-10T21:57:11.389Z Reads: 134

```
Ah, I missed the part when you said you were bypassing. Hopefully you are using another mechanism for over-discharge/over-current protection? Otherwise that's really dangerous. :-)
```

---
## \#15 Posted by: Jinra Posted at: 2017-07-10T22:02:13.961Z Reads: 130

```
Throw a fuse on there and you're all set. For me personally, I'm not using anything besides cell fusing. I'll risk it :)
```

---
## \#16 Posted by: rich Posted at: 2017-07-10T22:05:23.053Z Reads: 129

```
I use Lipos so i'm good with my fuse and vesc settings only :wink:
```

---
## \#17 Posted by: chiskate Posted at: 2017-07-11T02:42:45.840Z Reads: 128

```
That's your prerogative, but for the record and anyone else considering this architecture, it's very dangerous and likely to catch fire.

Fuses are not substitute for BMSs. Remember, fuses are designed into circuits to protect chassis wiring from overheating and starting fires, and not from the various failure modes that LiPo's can experience including a failing or buggy VESC. There's a reason you'll never see this architecture in any shipping product.
```

---
## \#18 Posted by: rich Posted at: 2017-07-11T15:01:06.397Z Reads: 120

```
I would say 95% of the people using Lipos without BMS.... just a balance charger for charging. In my case i bypass my cheap BMS just because of easy charging.
You are right that everybody should use BMS on any build....... but in real world i think it's more dangerous when people make wrong balance cable connections and short their Lipos instead of just take the risk.
[quote="chiskate, post:17, topic:17693"]
There's a reason you'll never see this architecture in any shipping product
[/quote]
Is there a product with Lipos and not Li-ion out there?
```

---
## \#19 Posted by: Jinra Posted at: 2017-07-11T15:06:58.943Z Reads: 117

```
Technically starry (and i think the new evolve) uses lipo pouches, but starry is also one that has blown up even with a bms
```

---
## \#20 Posted by: rich Posted at: 2017-07-11T15:11:44.156Z Reads: 124

```
Ok, interesting...

[quote="Jinra, post:19, topic:17693"]
blown up even with a bms
[/quote]

😂😂😂
```

---
## \#21 Posted by: mkd Posted at: 2017-07-11T16:09:48.169Z Reads: 122

```
@rich
Thank you so much for your help!

I've worked over my wiring circuit (Is the vedder anti spark switch from esk8 connected correctly?): 

<img src="/uploads/db1493/original/3X/8/9/8917eae65d921956ea21e78cd39059fb1af88b39.JPG" width="666" height="500">


Is this the kind of charger I am looking for?
(Li-ion / 25,2V / 3A)
https://de.aliexpress.com/item/High-quality-Output-25-2V-3A-Li-ion-Li-Po-Battery-charger-Used-for-6-Series/32616801501.html?spm=a2g0s.13010208.99999999.269.zxPkOZ

How long will charging take with 3A?

Thank you
```

---
## \#22 Posted by: rich Posted at: 2017-07-11T17:53:41.810Z Reads: 112

```
Yes, looks good now.
The charger is also the right one.
Just as a thought, if you have time to wait for charger from china i would consider buying a better BMS, too. For the price of the bypassed hobbyking BMS + Antispark switch you could get a BMS with switch and enough power for discharge, too. 

Charging time i would say is about 1,5-2,5 hours for 5000mAh, depends on BMS as well.
```

---
## \#23 Posted by: mkd Posted at: 2017-07-12T16:20:05.890Z Reads: 109

```
@rich

Thank you very much :slight_smile:

I will have a look at all the parts again and then decide which parts I will use finally.
```

---
## \#24 Posted by: mkd Posted at: 2017-10-06T09:39:41.345Z Reads: 105

```
@rich

Hello
Can anyone Tell me how to bypass this bms?
I have only got P- and B- but no C-
<img src="/uploads/db1493/original/3X/a/4/a4a3c3d71266ff74604b80731e44506eada0a5e5.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/1/c/1cb61622b11bae59d768aaea39511e35b6aaaecd.jpg" width="375" height="500">
```

---
## \#25 Posted by: rich Posted at: 2017-10-06T12:39:34.518Z Reads: 99

```
I guess P- is also C-, otherwise it wouldn't make sense.
For balance wires connect b1+ to b6+, there is no b1- connection between Lipo and BMS in your case.
```

---
## \#26 Posted by: mkd Posted at: 2017-10-06T15:04:12.250Z Reads: 100

```
If P- is also C-, does that mean that I can‘t bypass this bms?
```

---
## \#27 Posted by: Jinra Posted at: 2017-10-06T15:29:14.106Z Reads: 101

```
No, you can always bypass BMS. Use P- for charger negative, hook up B- like normal to battery negative, but have a second line on battery negative for your ESC as well.
```

---
## \#28 Posted by: thisguyhere Posted at: 2017-10-06T17:34:27.539Z Reads: 98

```
[quote="mkd, post:24, topic:17693"]
Can anyone Tell me how to bypass this bms
[/quote]

<img src="/uploads/db1493/original/3X/5/2/52cee61a721a34d1a2c758fa3d6e71ac64ad1034.jpg" width="521" height="500">
```

---
## \#29 Posted by: mkd Posted at: 2017-10-09T09:29:47.390Z Reads: 95

```
@rich @thisguyhere @Jinra

Thank you very much :) 

I've got one last question (hopefully! :weary:)

Is it of importance which contact (long or short) of the power jack is connected to either the charger minus or plus?


<img src="/uploads/db1493/original/3X/8/2/82a695ed2389fec394b6a43d8623583f5844eea9.png" width="519" height="499">
```

---
## \#30 Posted by: rich Posted at: 2017-10-09T11:44:32.788Z Reads: 90

```
Inner contact is always plus and outer contact is minus. Hard to tell from your picture, you can see it better on the back of the charging port. In my case it looks like this:

<img src="/uploads/db1493/original/3X/d/b/db7cedb83604f70a5c741ec302e1d84cc3467394.jpg" width="690" height="388">
```

---
## \#31 Posted by: SilentException Posted at: 2017-10-09T11:49:06.604Z Reads: 91

```
As @rich said, normal convention is negative outside, positive inside (pin). The socket you have is crappy, I wouldn't push over 2A on that. Also, when soldering cables to the socket, keep the disposable plug with cable in the socket. It will help avoid bending the pin inside due to heat and melted plastic.
```

---
## \#32 Posted by: thisguyhere Posted at: 2017-10-09T17:15:54.355Z Reads: 85

```
connect your charger into the port, use a multimeter to make sure

positive voltage means polarity is correct, negative voltage means it's reversed.
```

---
## \#33 Posted by: mkd Posted at: 2017-10-29T10:05:29.112Z Reads: 75

```
Thank you very much for your answers. I've been very busy but finally here are some pictures of my port. 
Hopefully you can help me with these pictures to find out which contact is used for either minus or plus?
Otherwise I have to use the method as described by @thisguyhere. 

 <img src="/uploads/db1493/original/3X/f/2/f22fa9b2c37bdfbc57fce0a8ec7f6e9352cdc053.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/3/4/346d47217bc8f2dae2214aa9a3cd5b7bac38bbba.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/2/5/255bf4442d2707db7948e7b4bea0403f50ba8e9f.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/0/c/0c192aba15b51142be35e1c0b69aef9a7340f6b2.JPG" width="666" height="500">
```

---
## \#34 Posted by: rich Posted at: 2017-10-29T10:19:47.210Z Reads: 73

```
As said, normally the inner contact in the middle is plus and the outer minus. To check it with multimeter is a good idea, too. Also you can check the data on the back of your charger, usually it's written there. In my case it's standard assignment, inner plus, outer minus.

<img src="/uploads/db1493/original/3X/b/5/b52247c87282eff1acbe3e125d03e6f60322df98.jpg" width="690" height="388">
```

---
## \#35 Posted by: mkd Posted at: 2017-11-04T09:39:57.127Z Reads: 60

```
@rich 
  http://www.electric-skateboard.builders/t/bms-broken-again/17693/10

How do I wire the two 3s balance leads to a 6s bms? The Bms has only got six cables. Which cables are not needed and which are connected together? 

Tank you
```

---
## \#36 Posted by: rich Posted at: 2017-11-04T15:01:41.669Z Reads: 51

```
The safest way is to buy 3s extensions and use the male connectors for the lipo balance female connectors. The you can solder the correct wires together. It is very important that (as in my scheme) lipo A is power negative and lipo B is positive. Also the correct order of the balance wires is a must otherwise you get serious troubles. Triple check it and use a voltmeter. In my second picture you can see the assignment of the JST-XH connectors. And you have to connect B- before you plug the balance connector to the BMS. Don't use the first (negative) wire of your 3s (4pin) balance wires!!!

<img src="/uploads/db1493/original/3X/d/5/d5b765f83147e79dc3fb3d6f1596daaab3a758a5.jpg" width="690" height="376">

<img src="/uploads/db1493/original/3X/a/8/a898409ed70a0599d75fb8b87cd9a92914134d20.jpg" width="690" height="307">
```

---
## \#37 Posted by: Eboosted Posted at: 2017-11-04T15:02:44.844Z Reads: 45

```
I have that same bms and I use it only for charging, my cells have been balanced for almost 1 year, however I'm sure if they would be balanced as well if I wouldn't have used bms as all my other builds without bms
```

---

# Vesc, battery pack and motormount for MountainBoard build

### Replies: 38 Views: 2372

## \#1 Posted by: CruelSummer Posted at: 2018-02-11T18:01:55.398Z Reads: 215

```
Hey! 
This is my first build and I want to start with a mountainboard with dual setup!
I read a lot of topic but some questions still exist so better ask!

This is what i have: 

Turnigy graphène 4000mAh 6S 45C Lipo pack  x 4 
from https://hobbyking.com/fr_fr/graphene-4000mah-6s-45c-w-xt90.html


![IMG_2613|375x500](upload://cw8Yw8QtlTXmOUgCxNgPfNkBTFm.jpg)

MAYTECH VESC x2
 from https://zcplushies.com/products/maytech-vesc-bldc-vedder-electric-speed-controller
connected via CAN bus 

![2018_02_03_IMG_0297|666x500](upload://f5sbKGPiB8h25cC9Sl4ysUq8hop.JPG)

Turnigy Aerodrive SK3 - 6374-192kv Brushless x 2
from https://hobbyking.com/fr_fr/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
![IMG_2619|375x500](upload://nAObfCqf0QJUyREag2N2ONb5whr.jpg)

My board ( basic mountain board with basic trucks )
![IMG_2615|666x500](upload://r91sWJj3pSRkIY3AGBu8uNAW0mD.jpg)

Wheels ( looks like Trampa SUPERSTAR Wheels bc they have the same spec )

![IMG_2616|375x500](upload://xsIf0IMyDNI1B15vcaB0Pl03VBg.jpg)

I also have some connectors for my battery.

First, i have somes questions about my lipos: 

![IMG_2614|375x500](upload://zrOEcalfRoAWAC6s9pzZjaQn7J4.jpg)

I want to put them in series and parallel to create 12s 8000mAh 44.4v Batterypack
to show you what i want here is a sheme 
![E0F62EA8-5013-4685-9C27-77B60DF58454|689x410](upload://5ZGJ6bUv7rn87EMmcrn1K7GRKSx.jpg)

Is it possibe to use them like that or i Need a BMS ?
I will charge them 2 by 2.

Secondly, I'am looking for motormount, pulley and belt that will fit with my motor.

I know i got "normal trucks" so i'm interresting by INFINITY Trucks by trampa.
http://www.trampaboards.com/infinity-trucks--solid-hanger-body-with-12mm-solid-axles--mega-strong-p-11151.html
Where can i find motormount (cheap if possible) adapted to my trucks (or trampa trucks) ?


I will talk about VESC later, my main concern is the battery pack and motormount.

Thanks!
```

---
## \#2 Posted by: Colson003 Posted at: 2018-02-11T18:36:08.210Z Reads: 173

```
http://www.electric-skateboard.builders/t/motor-mounts-kits-for-trampa-atb-and-mbs-matrix-old-type-matrix-ii-ats/44749
```

---
## \#3 Posted by: Riako Posted at: 2018-02-11T19:08:02.009Z Reads: 167

```
Hey CS ! 
Good start ;) , no problem for your wiring, and yes the last connector you need is the // one (before your swith and then vescs and motors). But that is a lot of wiring and XT connectors !.. secures them for emtbing !
Tcheck Colson link, maybe Idea could also make the mount for your actual trucks (but I will go with a spring upgrade too)
:v:
```

---
## \#4 Posted by: CruelSummer Posted at: 2018-02-11T19:14:40.477Z Reads: 153

```
I am thinking about his motormount but it will probably not fit with my trucks but i will discuss with him :grin: thanks
```

---
## \#5 Posted by: CruelSummer Posted at: 2018-02-11T19:25:35.311Z Reads: 146

```
Thanks Rakio  :grinning:
I was worried about the wiring bc it's lipo cell and i read they was pretty dangerous. 
According to you i don't need a BMS to survey the discharge ?
To fix them properly i amm using Heat Shrink from : https://hobbyking.com/en_us/turnigy-heat-shrink-tube-30mm-red-1mtr-1.html

Last one , where i put the switch ?
```

---
## \#6 Posted by: Riako Posted at: 2018-02-12T00:55:55.772Z Reads: 131

```
No you don't need it (but you could if you want to charge them easyer way...not sure about that too, deepending of your chagrer. I got a dual raktor working good actualy).
You got a solid pack :muscle: I make a 12s 8ah with 2x 6s8Ah15c Graphene too (but low C rating in this conf.) and it work all good.
I used lipo also on my emtb and other build, no worries for you and your pretty hight discharge capacity (if your carrefull when wiring them correctly). 
An other good way to be sure : 
https://img4.hostingpics.net/pics/788428IMG20171028192816.jpg
```

---
## \#7 Posted by: Rithblu Posted at: 2018-02-12T02:54:15.064Z Reads: 122

```
www.allterraincreations.com
```

---
## \#8 Posted by: CruelSummer Posted at: 2018-02-12T15:13:28.842Z Reads: 116

```
[quote="Riako, post:6, topic:46126"]
No you don’t need it (but you could if you want to charge them easyer way…not sure about that too, deepending of your chagrer. I got a dual raktor working good actualy).

You got a solid pack :muscle: I make a 12s 8ah with 2x 6s8Ah15c Graphene too (but low C rating in this conf.) and it work all good.

I used lipo also on my emtb and other build, no worries for you and your pretty hight discharge capacity (if your carrefull when wiring them correctly).

An other good way to be sure :

https://img4.hostingpics.net/pics/788428IMG20171028192816.jpg
[/quote]

Hell yeah!  stay in touch i will show my battery pack later. I'm just waiting for some more connections
```

---
## \#9 Posted by: Pimousse Posted at: 2018-02-12T15:23:26.447Z Reads: 105

```
Don't wire GND and 5V between both CAN bus port !
```

---
## \#10 Posted by: CruelSummer Posted at: 2018-02-12T15:42:34.806Z Reads: 100

```
[quote="Pimousse, post:9, topic:46126, full:true"]
Don’t wire GND and 5V between both CAN bus port !
[/quote]

My scheme isn't correct ? 
How do i need to wire them ?
```

---
## \#11 Posted by: darkkevind Posted at: 2018-02-12T15:45:06.321Z Reads: 98

```
I have these for sale?

http://www.electric-skateboard.builders/t/trampa-mtb-motor-mounts-worldwide-shipping/46183
```

---
## \#12 Posted by: Pimousse Posted at: 2018-02-12T15:47:34.994Z Reads: 93

```
Not from your scheme but from your VESCs picture.
Tell your reseller that he's selling wrong CAN-bus connectors.
Only the 2 middle wires need to be connected, not the black and red one.
That can lead to fry your VESC.
```

---
## \#13 Posted by: CruelSummer Posted at: 2018-02-12T15:47:54.838Z Reads: 97

```
[quote="darkkevind, post:11, topic:46126, full:true"]
I have these for sale?

    Trampa MTB Motor Mounts (worldwide shipping) New Items For Sale

    Brand new, never used aluminium motor mounts for Trampa mountain board trucks. 
Comes with all fittings. 
£70 + shipping 
I can ship anywhere in the world but you pay for it :wink: 
Payment by PayPal. I’ll ship the same day if before 3pm. 
 [20180212_120331]
 [20180212_120408]
 [20180212_120418]
[/quote]

How much to ship in France ? 
And would it fit with my morors ? they are pretty big
```

---
## \#14 Posted by: CruelSummer Posted at: 2018-02-12T15:52:23.497Z Reads: 94

```
![image|375x500](upload://fefmTrkBvOF7eNeHFdKL14XgakJ.jpeg)

Which one ?
```

---
## \#15 Posted by: Pimousse Posted at: 2018-02-12T15:53:10.274Z Reads: 88

```
#1
10 char
```

---
## \#16 Posted by: CruelSummer Posted at: 2018-02-12T15:55:38.703Z Reads: 88

```
[quote="Pimousse, post:15, topic:46126, full:true"]
#1

10 char
[/quote]

I remove them. :grin:
I need to find another CAN bus connector ?
```

---
## \#17 Posted by: Pimousse Posted at: 2018-02-12T15:58:21.826Z Reads: 89

```
No.
Just remove (or cut) red and black wires.
http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142?u=pimousse
```

---
## \#18 Posted by: CruelSummer Posted at: 2018-02-12T16:06:32.485Z Reads: 86

```
If i cut them no need of JST-PH 2MM, they will work together after all ?
```

---
## \#19 Posted by: darkkevind Posted at: 2018-02-12T16:50:31.486Z Reads: 88

```
£11 to ship to France, tracked.

I'm pretty sure it can take some pretty beefy motors! :smile:

![20180212_164829|666x500](upload://nA5EjQkTUysnVO6sijaY0PqpN05.jpg)

![20180212_164850|666x500](upload://Ti0BRk7Rk0bljBSfkCte9LuKE6.jpg)
```

---
## \#20 Posted by: JonathanLau1983 Posted at: 2018-02-12T16:59:02.188Z Reads: 84

```
[quote="CruelSummer, post:18, topic:46126, full:true"]
If i cut them no need of JST-PH 2MM, they will work together after all ?
[/quote]

You can usually pull the wire out if you lift the tab a little.
```

---
## \#21 Posted by: Nemesis Posted at: 2018-02-12T18:52:28.982Z Reads: 79

```
Concerning your trucks/mount situation.... you could just get the super cheap easy to get spares for   https://www.mbs.com/parts/12101-mbs-ats12-truck-system-white-1 they are a straight swap out for the ones you have ie no hard to get hold of and expensive riser needed, i know @Idea made mounts for that truck maybe hes still got some in stock?. 

Obviously the MBS ATS 12's are not the best truck for abusive riders but will work well enough for bombing about on.
```

---
## \#22 Posted by: CruelSummer Posted at: 2018-02-12T19:16:25.313Z Reads: 79

```
Cheap alternative but I've already ordered 

http://www.trampaboards.com/infinity-trucks--solid-hanger-body-with-12mm-solid-axles--mega-strong-p-11151.html
Thanks :grinning:
```

---
## \#23 Posted by: CruelSummer Posted at: 2018-02-12T19:18:41.930Z Reads: 78

```
[quote="JonathanLau1983, post:20, topic:46126"]
You can usually pull the wire out if you lift the tab a little.
[/quote]

I don't understand what you mean by pulling out the wire :disappointed_relieved: 
Just want my 2 vescs working together
```

---
## \#24 Posted by: Acido Posted at: 2018-02-12T19:52:04.964Z Reads: 73

```
Pull it out from the white plug
```

---
## \#25 Posted by: pat.speed Posted at: 2018-02-12T20:04:26.136Z Reads: 74

```
Instead of cutting the red and black wires there is a small little tab on the white plug. If you push it in with a needle or something small you will be able to just slide the whole wire and metal socket out
```

---
## \#26 Posted by: CruelSummer Posted at: 2018-02-12T20:11:35.983Z Reads: 74

```
![image|667x500](upload://wKQEf9EDLLLIwaUmAT9zaYFM6CL.jpeg)

You mean push theses ?
```

---
## \#27 Posted by: pat.speed Posted at: 2018-02-12T20:12:20.448Z Reads: 72

```
Nope on the plug in wire piece



![IMG_1168|440x500](upload://ApzZBF6V83RnhOkLW2SCU2TvtES.JPG)
```

---
## \#28 Posted by: Sapphirinia Posted at: 2018-02-12T20:48:06.169Z Reads: 68

```
But don't let the metal pins touch each other!
```

---
## \#29 Posted by: GrecoMan Posted at: 2018-02-12T20:50:09.797Z Reads: 68

```
it’s a can cable, as long as it’s not plugged in he doesn’t have to worry
```

---
## \#30 Posted by: Sapphirinia Posted at: 2018-02-12T20:50:36.247Z Reads: 67

```
Oh, ok. I thought it looked like a balance plug
```

---
## \#31 Posted by: GrecoMan Posted at: 2018-02-12T20:51:06.920Z Reads: 66

```
everything looks like a balance plug when you’re tired 🤣

nah but the sensors, uart, and every other port on the vesc (excluding ppm) is the same connector as balance cables, just different pin counts
```

---
## \#32 Posted by: Sapphirinia Posted at: 2018-02-12T21:16:22.525Z Reads: 62

```
I have too many explosive flashbacks lol
```

---
## \#33 Posted by: Pimousse Posted at: 2018-02-12T21:17:59.380Z Reads: 63

```
Not quiet the same.
VESC : JST-PH
Balance plugs : JST-XH
```

---
## \#34 Posted by: GrecoMan Posted at: 2018-02-12T21:19:35.953Z Reads: 62

```
i could’ve sworn i’ve stolen a balance cable and plugged it into my uart port 🤔
```

---
## \#35 Posted by: Pimousse Posted at: 2018-02-12T21:21:41.509Z Reads: 66

```
Maybe, but you did force a bit, right ? :slight_smile:
https://en.wikipedia.org/wiki/JST_connector 

JST-PH pin pitch : 2.00mm
JST-XH pin pitch : 2.50mm
```

---
## \#36 Posted by: CruelSummer Posted at: 2018-04-09T19:52:36.057Z Reads: 53

```
Hey! 
After a long journey I’m back with good news Builders :laughing: . 
I think the best way to show you how far I am now is by showing you some pics: ![image|375x500](upload://dnp3Et4yjSWahRNQ5Xp8SPq4exh.jpeg)

![image|375x500](upload://oxqIp4GPROGfeW8efs8f1dhbXph.jpeg)

It was the moment when I got the motormount and the Trampa truck. 

![image|375x500](upload://Ap4gIuDiiSLtmi6OKh4jYevryzB.jpeg)![image|374x500](upload://8s6CjYM9uIQ0AirDqXhcPOu6vK4.jpeg)

I found out that I my board was i little too "basic" so i pimped it with some colours!  :heart_eyes:

![image|375x500](upload://xwWvstAGMzEqDlyAFp2Xct0HHl8.jpeg)![image|375x500](upload://itbRwF8P6rm3Ye4swtEsPa509IL.jpeg)![image|374x500](upload://9iWlcAdK41HY6FxP3NmAFhnVfML.jpeg)


HERE I AM NOW! :yum: :sunglasses: 
Thanks to your advices I have almost finish my work I appreciate the good energy! 


Stay in touch because now i need to configure my VESC with VESC tool and I think it will be pretty hard hahah!
```

---
## \#37 Posted by: ksfacinelli Posted at: 2018-04-17T17:01:54.859Z Reads: 46

```
Wow, Nice build where did you get your chain drive components?  Did you have to mod?

Thanks,
Kevin
```

---
## \#38 Posted by: CruelSummer Posted at: 2018-04-18T17:43:51.886Z Reads: 45

```
I really don't know if OVERION ship outside of france but i think he does. My chain drive come from his website:

http://www.overion.fr/produit/transmission-pour-kit-e-mtb/ 

It fits very well with Trampa trucks and  MBS rockstar II rim :grinning:
```

---

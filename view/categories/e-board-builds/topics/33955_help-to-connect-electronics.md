# Help to connect electronics

### Replies: 38 Views: 1554

## \#1 Posted by: Nicoalix Posted at: 2017-09-25T20:53:14.837Z Reads: 151

```
This is my shopping list

https://docs.google.com/spreadsheets/d/1kAeMj_4PdVV2QlHndLh8U6AN_a2wn8UF6PU3kZ69W-w/edit?usp=sharing

Can you help me complete it with connectors, converters, and anything else i might need in terms of electronics to connect everything? It is the first time that I do something like this and I have no experience at this point.
Can you recommend a charger with integrated bms? (if this exists)
Any security tips? I'm really scared of burning the engine or vesc.

Thank you!
```

---
## \#2 Posted by: Nicoalix Posted at: 2017-09-26T09:37:38.462Z Reads: 124

```
Is this diagram correct?
<img src="/uploads/db1493/original/3X/d/e/de2a1d0ea7ed4a597c71e2da540c69ab702cb1b3.jpg" width="690" height="402">
```

---
## \#3 Posted by: Nicoalix Posted at: 2017-09-26T10:24:06.134Z Reads: 112

```
I have this unused battery charger
http://www.hobmodel.com/CARGADOR-MAXPRO-EASY-50

What would happen if you used this charger to charge a 9s1p 8000mAh battery?
Will it not run or will it charge the batteries slow?
```

---
## \#4 Posted by: scepterr Posted at: 2017-09-26T10:25:37.809Z Reads: 105

```
Battery indicator doesn't plug into vesc just battery, also with 125kv motor 12s would be best or higher kv with 9s. 
You can't use that charger for 9S
```

---
## \#5 Posted by: Nicoalix Posted at: 2017-09-26T10:36:02.027Z Reads: 97

```
Thanks @scepterr, the XT-60 plug (battery - focbox) have 2 exits, one for focbox, one for battery indicator, is not like that?
```

---
## \#6 Posted by: Nicoalix Posted at: 2017-09-26T10:41:10.269Z Reads: 94

```
[quote="scepterr, post:4, topic:33955"]
You can't use that charger for 9S
[/quote]

if I have 3x3s1p 8000mAh (or 4x3s1p 8000mAh), can I charge the batteries with a 3s 8000mAh? would not charge in series too?
```

---
## \#7 Posted by: scepterr Posted at: 2017-09-26T10:46:50.083Z Reads: 90

```
You could switch them to all series or charge each 3s pack itself. There are 3 sets of wires on the focbox, the xt60, the 3 phase leads opposite it, and a 3pin wire on the side for ppm/remote receiver
```

---
## \#8 Posted by: Nicoalix Posted at: 2017-09-26T10:49:17.949Z Reads: 83

```
The idea is to duplicate the battery lead before reaching the focbox, maybe I am wrong.
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-26T10:51:12.586Z Reads: 83

```
Right...that has nothing to do with the focbox. You could do it that way or splice it in or solder it to the terminals of one of the connections between battery and vesc
I think you're overcomplicating it 😉
```

---
## \#10 Posted by: Nicoalix Posted at: 2017-09-26T10:58:36.627Z Reads: 86

```
[quote="scepterr, post:9, topic:33955"]
one of the connections between battery and vesc
[/quote]

now I understand, you mean the wire with the interrogation, I have to delete it.
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-26T11:01:25.895Z Reads: 81

```
There is nothing to connect here, if you connect voltage indicator here that's also connected to the battery you will fry the focbox <img src="/uploads/db1493/original/3X/2/8/28283f9699fbb4a364ab0315f52b320e536f958b.jpg" width="690" height="488">
```

---
## \#12 Posted by: Nicoalix Posted at: 2017-09-26T11:02:54.057Z Reads: 76

```
that is, I had doubts about whether I had to use the 5v output of the focbox to power the battery indicator, so the interrogation, I see no
Thanks @scepterr
```

---
## \#13 Posted by: Nicoalix Posted at: 2017-09-26T11:14:11.685Z Reads: 76

```
Updated diagram with 12s and BMS, is everything okay?
```

---
## \#14 Posted by: MontPierre Posted at: 2017-09-26T11:21:39.759Z Reads: 77

```
Battery indicator looks good now but charger shouldn’t be connected to vesc ! 

It goes to BMS which will charge your batteries.
```

---
## \#15 Posted by: MontPierre Posted at: 2017-09-26T11:26:44.203Z Reads: 77

```
<img src="/uploads/db1493/original/3X/3/c/3c270d2dac8353fae7063a170cd368936c6170af.png" width="664" height="500">

This should help. This is a set up without bypassing discharge, you’ll have to check how your BMS needs to be wired, check pictures of it or any documentation with it. You just need to connect your antispark to this diagram.
```

---
## \#16 Posted by: Nicoalix Posted at: 2017-09-26T11:58:15.680Z Reads: 61

```
[quote="MontPierre, post:15, topic:33955"]
You just need to connect your antispark to this diagram.
[/quote]

it's OK now?
```

---
## \#17 Posted by: Nicoalix Posted at: 2017-09-26T14:58:57.814Z Reads: 60

```
Can I use two 6s chargers by dividing the charging input by 2? one for 2x3s and other for 2x3s

https://www.gearbest.com/charger/pp_778615.html?vip=860527&gclid=Cj0KCQjw9afOBRDWARIsAJW4nvyXPS8kvIYcOkDfbQBrziXOStxxKqocM1e303CYRr3dCsv-Dnk-ZccaAm2UEALw_wcB

In case of being use to do it, when doing with this charger, I would need a BMS?
```

---
## \#18 Posted by: MontPierre Posted at: 2017-09-26T16:26:43.490Z Reads: 62

```
I have noticed that you have 3x 3S batteries. This makes 9S not 12S unless you add one more 3S battery. 

Also, please research more on difference between BMS charging and via external LiPo charger like imax. They are completely different and require different set ups. IMAX is an external charger- you’ll charge each battery separately, without need of BMS. But BMS is more than just for charging!!!!   

I’m sorry but I don’t have time now to explain all of it to you, I’m at work at the moment, perhaps one of the other guys will have a moment. 

Nevertheless please do a research, both BMS and imax chargers have been covered on this forum in extreme detail. When I built my board I have spent few weeks just Reading forum, to gain knowledge ;)
```

---
## \#19 Posted by: Nicoalix Posted at: 2017-09-26T16:40:08.798Z Reads: 60

```
Thnaks @MontPierre
I think my low level of English is creating a bit of a mess with respect to BMS and iMAX.

let's start with the argument that I will use 4x6s1p 8000mAh 30c

I would rather use the diagram shown at the beginning of the post, using a charger and a BMS, or, on the other hand, eliminate the BMS and use two external 6s chargers, dividing the load into two ports, parallel charging and serial discharging.
```

---
## \#20 Posted by: MontPierre Posted at: 2017-09-27T14:38:26.539Z Reads: 60

```
No worries!

@Nicoalix I think you meant 4x 3S not 4S ;) 

IMAX charger will charge only one 3S battery at the time so you’ll have to charge them 4 Times. It is a pain but totally doable. 

Bms will protect your electronics from frying in case of a short so it is recommended to use. Also it will prevent from over discharging if your batteries and switch off board when they his safe limit.
```

---
## \#22 Posted by: Nicoalix Posted at: 2017-09-28T09:45:43.202Z Reads: 48

```
I'm evaluating the idea of using 2x Turnigy B6 Compact 50W 5A Automatic Balance Charger 2 ~ 6S Lipoly
They have a current drain for 200mAh balance, which is more than triple than other BMS and + - 0.02V threshold.

https://hobbyking.com/media/file/391476037X129399X17.pdf

They seem a good option, if someone has tried, I would like to know your experience.

I would need two power supply, but I do not know which is best suited to the needs.
12v 5A 60w Power supply
16v 3.75A 60w Power supply
It seems that the ideal would be 16v and 5A but I can not find one with these characteristics, could someone clarify that power supply would be the most appropriate? between these two or others.
```

---
## \#23 Posted by: MontPierre Posted at: 2017-09-28T09:59:11.674Z Reads: 46

```
Charger looks good but If you want to charge all batteries at once you will need 4 chargers :) they can charge ONE battery at a time - it can be any battery which will have 2 - 6 S inside. 

As for power supply - go for one with more Amps - then you can charge quicker ( should battery allow higher amps charging). Voltage its not as important as charger will step it up anyway.
```

---
## \#24 Posted by: Nicoalix Posted at: 2017-09-28T10:01:59.427Z Reads: 41

```
[quote="MontPierre, post:23, topic:33955"]
they can charge ONE battery at a time - it can be any battery which will have 2 - 6 S inside.
[/quote]

Sorry @MontPierre I do not understand this part, specs indicate it can charge 6s Lipo.
I have 4x3s for discharging connected as 2x3s and 2x3s for charging,
can i use a 12v with 10A then? not explode anything? ^^
```

---
## \#25 Posted by: Nicoalix Posted at: 2017-09-28T10:45:38.907Z Reads: 38

```
Ok, I understand where the problem is, I would need a balanced board for every 2x3s battery.
```

---
## \#26 Posted by: MontPierre Posted at: 2017-09-28T10:53:25.923Z Reads: 39

```
Indeed charger can charge a battery which is up to 6S. It won’t be able to charge two 3S batteries. It is only able to charge one battery at the time. It has balance ports - see below. As you can see there is only ONE 3 Cells port. Also there is only one + and - for battery connection.

https://rclexa.co.uk/image/cache/catalog/item_pictures/1batteries/chargers/Turnigy%20B6%2050W%205A/Turnigy%20lipo%20charger%20B6%206%20cell%203-800x800.jpg

In terms of charging current - I have the same batteries - they are rated at 5C. Your charger specs say it will do max of 5A. 

http://www.catalog-rc.com/index.php?route=product/product&manufacturer_id=124&product_id=732&page=11

See Specifications tab.

5C means you can charge it at 5x Capacity. Capacity is 8Ah so 5x8 = 40A. 

I wouldn't charge them at such high current - it is absolute MAX! 

Safe is 1C - thats general recommendation. So in this case 8A. I charge mine at 5 Amps as this is a max for my charger. I have 10 S set up and batteries are full within an hour of charging so higher current is not necessary. The lower Amps while charging the longer your battery will last. 5A will be totally fine for you. at 5A batteries don't even get warm. 

I hope this explains.
```

---
## \#27 Posted by: Nicoalix Posted at: 2017-09-28T12:52:30.254Z Reads: 38

```
Thanks for that explanation, it is very helpful.

On the other hand, after understanding how the battery balance works, I still seem to think that a charger like the imax b6 v2 seems to be a better option than the bms that are sold in batterysupport:

**imax b6 v2:** Balance Current: 200mA / cell
**44V 48V 50.4V 12S 45A 12x 3.6V Lithium ion LiPolymer Battery BMS:** Balance current: 60mA / cell

I'm looking at the wrong specifications, or is it true that this makes the balance of the batteries much more effective with the imax b6?
```

---
## \#28 Posted by: MontPierre Posted at: 2017-09-28T13:03:14.403Z Reads: 36

```
This could well be true, it will be quicker at balancing your cells but having a BMS its a huge advantage. yes, a downside is that it will take much longer to balance but in my opinion thats small price to pay when you have protection from it while running a board. Read on about BMS and decide for yourself.
```

---
## \#29 Posted by: Nicoalix Posted at: 2017-09-28T13:06:09.735Z Reads: 37

```
[quote="MontPierre, post:28, topic:33955"]
Read on about BMS and decide for yourself.
[/quote]

I have done it, and I have understood that using a VESC, in my case FOCBOX, the support provided by the BMS to protect the batteries, already does the VESC itself

I'm wrong?
```

---
## \#30 Posted by: Nicoalix Posted at: 2017-09-28T13:12:13.522Z Reads: 37

```
[quote="MontPierre, post:26, topic:33955"]
see below. As you can see there is only ONE 3 Cells port. Also there is only one + and - for battery connection.
[/quote]

is it the same for the imax b6 v2? I only see one port of 3S
https://ae01.alicdn.com/kf/HTB1qLBkOVXXXXbfapXXq6xXFXXXJ.jpg
```

---
## \#31 Posted by: MontPierre Posted at: 2017-09-28T13:16:26.770Z Reads: 33

```
Yes, and I have this model. I'm not aware of any charge that can charge two batteries together but since I haven't looked into this I might be wrong. 

On the left of balance ports you have place to plug in leads from your battery - plus and minus. Only one thought.
```

---
## \#32 Posted by: MontPierre Posted at: 2017-09-28T13:18:33.185Z Reads: 34

```
Vesc has protection, but It won't for example shut down your board if ONE cell gets too low. It only measures all the cells in series. BMS looks at all of them individually which helps.
```

---
## \#33 Posted by: Nicoalix Posted at: 2017-09-28T13:24:19.021Z Reads: 35

```
Ok, definitely BMS seems to be the safest option then. Thanks for your tips!

If I connect the BMS in a way that works both in charge and in the discharge (if I do not do this, I suppose during the discharge I did not balance the batteries), I need a BMS capable of withstanding the continuous charge that will receive the  VESC, I'm going to use 4x3S1p 8000mAh / 20 / 30c (not sure about C yet), with 60A should it be enough? What happens when I send 240A for a few seconds for example to vesc?

is it the same if in the future I will use two vesc? or would i use a 120A BMS?
```

---
## \#34 Posted by: MontPierre Posted at: 2017-09-28T13:45:39.235Z Reads: 40

```
If you bypass BMS on discharge it will not protect electronics and batteries ( VESC ) during your riding. This means that Batteries will be directly connected to VESC during riding. It will only work as a charging solution. 

BMS Amperage choice should be based on MAX amps your motor can pull. It is 75A so 80A is plenty. You could get away with 60A but if you decide to go for 2 motor set up in the future it will not be enough. 

Most of guys have 80A BMS.

Charge will be supplied by your external power supply. I have this one and works perfectly. 
It is large and heavy but charges quickly. 

https://www.banggood.com/36V-37V-42V-45V-5A-Battery-Charger-For-10s-10x-3_6V3_7V-Lithium-Li-ion-Battery-p-1115729.html?rmmds=myorder 

Your charger voltage must be equivalent of number of cells in series times 4.2V ( maximin voltage Lipo cell will be charged to). So it is 12 x 4.2V = 50.4V

Something like this one, but do a research you might find something cheaper on Aliexpress or ebay. 

http://www.batterysupports.com/432v-44v-504v-4a-lithium-ion-lipo-battery-charger-12s-12x-36v-p-167.html 

Then you have to look at the connector charger has. Port you will install in your enclosure should be a female version of your charger plug so they can connect. If you are struggling then you can find a set of female and male ports and cut off plug that comes with your charge and put on different one of your choice :) thats what I did, was dead easy. This is what i have. 


http://www.ebay.co.uk/itm/3-4-5-6-8-Pins-Microphone-Chassis-Sockets-Plugs-Male-Female-CB-Ham-Radio/231359930831?ssPageName=STRK%3AMEBIDX%3AIT&var=530622215034&_trksid=p2057872.m2749.l2649

http://www.ebay.co.uk/itm/3-4-5-6-8-Pins-Microphone-Chassis-Sockets-Plugs-Male-Female-CB-Ham-Radio/231359930831?ssPageName=STRK%3AMEBIDX%3AIT&var=530622215036&_trksid=p2057872.m2749.l2649

plus this nice metal screw on cap to protect port from water and dust - otherwise you can get a short and blow whole board.

https://www.aliexpress.com/item/2Pieces-Aviation-Plug-Cover-Waterproof-Connector-Plugs-Dust-Metal-Cap-for-GX16/32808625537.html
```

---
## \#35 Posted by: MontPierre Posted at: 2017-09-28T13:48:27.343Z Reads: 35

```
Here is mine mounted on my board. 

<img src="/uploads/db1493/original/3X/a/b/ab39892e612c1e2cc4792f5190742181d6429dff.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/9/d99969dcd540775c62298e83abc24d2ad14e6ef7.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/d/2/d2db5b6992c536a8f1dbb6a8197ee079d790b9aa.jpeg" width="375" height="500">
```

---
## \#36 Posted by: MontPierre Posted at: 2017-09-28T13:50:07.504Z Reads: 34

```
I also recommend getting BMS from Bestech as it has built in Switch so you don't need anti spark. It will save you money ( something like 20 euros ) and space in the board :)
```

---
## \#37 Posted by: Nicoalix Posted at: 2017-09-28T16:48:31.518Z Reads: 34

```
[quote="MontPierre, post:36, topic:33955"]
oney ( something like 20 euros ) and space
[/quote]
You mean an antispark like this?
https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html
```

---
## \#38 Posted by: Nicoalix Posted at: 2017-09-28T17:50:14.944Z Reads: 31

```
[quote="MontPierre, post:34, topic:33955"]
if you decide to go for 2 motor set up in the future it will not be enough. 

Most of guys have 80A BMS.
[/quote]

Even if I use one of 80A, do I limit the input at each VESC to 40A? being its maximum 60A, or does it not work like this?
```

---
## \#39 Posted by: Nicoalix Posted at: 2017-10-01T22:49:12.035Z Reads: 27

```
Can anyone take a look at my diagram and tell me if you see anything strange or something that can be improved?
As you will see, I try to bypass the BMS during the download, using a single loop-key that will change from charge to discharge.

Can I cause damage if I start charging the batteries with the loop-key in ON mode?

I have seen that in many cases people use fuses, I have put them without knowing very well which should use.

<img src="/uploads/db1493/original/3X/3/7/3737a5ab35c20d485d7e9e8e55787889f770b488.jpg" width="689" height="379">
```

---

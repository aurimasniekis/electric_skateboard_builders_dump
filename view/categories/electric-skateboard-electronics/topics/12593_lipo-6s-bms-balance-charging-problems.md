# LiPo 6S BMS Balance Charging Problems

### Replies: 49 Views: 4399

## \#1 Posted by: JdogAwesome Posted at: 2016-11-06T19:22:47.129Z Reads: 264

```
Let me explain my situation first; I'm working on building my Electric Longboard and at the moment I'm working on the battery for it. Currently I'm trying to use 2 3S 5Ah LiPo's in series to drive my board and I'm trying to setup the BMS for it. Anyways right now I'm trying to charge the battery through the BMS and I'm having some trouble doing so. First, when I plug the B+ and B- terminals into the main leads of the LiPo and give 25.2V to the P+ and P- terminals it draws current and starts charging the battery, great! Problem is when I plug the balance cable into the BMS, it immediately stops drawing any current to charge the LiPo. When I remove the balance plug it then immediately starts drawing current again. As you can see this is a big problem as the BMS needs to be able to balance the cells as well. If anybody has any ideas on why it's doing this please let me know! 

Link to BMS on AliExpress: http://s.aliexpress.com/UFFzEv2Q

<img src="/uploads/db1493/original/3X/6/b/6b7d03b5da66bfab73a6cc2d64a4ca4fdc39dd9b.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/b/6b95a992acace2887b9f1fdd2cef4c9d9e6fdedc.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/4/5/45a70058e3ab58e20773455807d76e2f8675921b.jpg" width="690" height="388">
```

---
## \#2 Posted by: Maxid Posted at: 2016-11-06T19:26:36.049Z Reads: 242

```
How can a 6S battery result in a 5S balancer cable? I know that BMSs usually omit the ground wire but that should still leave 6 cables to hook up to the BMS
```

---
## \#3 Posted by: 2-alex-2 Posted at: 2016-11-06T19:38:22.280Z Reads: 238

```
This bms uses bothe the - and + for balancing with the 5 cables for inbeteeen the cells

<img src="/uploads/db1493/original/3X/1/3/1359896b5894fb404e47e894296891ade8525148.PNG" width="281" height="499">

I also have this bms but haven't wired it up yet.
```

---
## \#4 Posted by: JdogAwesome Posted at: 2016-11-06T20:40:44.799Z Reads: 206

```
@2-alex-2  yeah I have everything wired up correctly, I think, but I'm still having these problems. I've checked the cells on the balance leads and they all add up to the right voltages, it's just not charging it when the balance lead is connected.
```

---
## \#5 Posted by: 2-alex-2 Posted at: 2016-11-06T22:25:05.570Z Reads: 198

```
Have you wired the balance leaded the right way
```

---
## \#6 Posted by: JdogAwesome Posted at: 2016-11-06T22:36:25.716Z Reads: 193

```
I'm pretty much 100% sure I have but, can you see any problems with it?
```

---
## \#7 Posted by: JdogAwesome Posted at: 2016-11-06T22:43:44.027Z Reads: 188

```
Yeah I just went over the balance leads and there definitely properly connected... I think the BMS may just be broken.
```

---
## \#8 Posted by: 2-alex-2 Posted at: 2016-11-06T22:49:12.795Z Reads: 181

```
From both - should be from the bottom of the balance lead. Over next day or so I will be wiring mine up but first I'm testing what D- is for as I think that should be the discharge - not P- so got the check first.
```

---
## \#9 Posted by: JdogAwesome Posted at: 2016-11-08T21:05:05.907Z Reads: 168

```
@2-alex-2 HEY! So I figured out my problem! I needed to be giving it 26V on the P+ and D- NOT P- terminals! At ~26.1V it draws around 5A though changing the voltage will change how much current it draws.
```

---
## \#10 Posted by: 2-alex-2 Posted at: 2016-11-08T21:16:06.101Z Reads: 166

```
For charging or discharging as I was in contact with the seller and he garanteed me that D- doesn't need to be used. So I have borrowed a voltage regulator to try and figur out everything.
```

---
## \#11 Posted by: 2-alex-2 Posted at: 2016-11-08T21:18:48.722Z Reads: 163

```
What voltage is the battery out as the over voltage might have kicked in or have you discharged it first.
```

---
## \#12 Posted by: JdogAwesome Posted at: 2016-11-08T21:34:22.613Z Reads: 161

```
@2-alex-2 are you using the same BMS as I am? All I know is that using D- is working for me so I'm fine with that lol.
```

---
## \#13 Posted by: 2-alex-2 Posted at: 2016-11-08T21:38:55.478Z Reads: 162

```
Yea I have the 5a version but haven't finished wiring it up. So what do you have where? As I was going to wire up B-/B+ battery then P-/P+ for charging then have a led indicator attached to D- as a discharge which should then indicate weather one cell is down.
```

---
## \#14 Posted by: 2-alex-2 Posted at: 2016-11-08T21:40:05.284Z Reads: 162

```
As ther two side on the bms looks like there is a hvc and a lvc which I thin D- is the lvc and P- is the hvc
```

---
## \#15 Posted by: JdogAwesome Posted at: 2016-11-08T22:02:01.911Z Reads: 162

```
I was originally following @VladPomogaev instructable [HERE](http://www.instructables.com/id/Fast-Electric-Skateboard-LiPo-Charging-System-BMS-/?ALLSTEPS)  and he was using the 5A  version so there might be a difference between the two other than the amperage it can handle. 

Here is a pic of how I have not wired up now.
<img src="/uploads/db1493/original/3X/9/c/9ce134a272cfec926c0ee0ae2a6ae3e95fc07e36.jpg" width="690" height="388">
```

---
## \#16 Posted by: 2-alex-2 Posted at: 2016-11-08T22:58:32.317Z Reads: 152

```
Ok have just soldered mine all up and the smd next to the balance plug get really hot do yours do this ?
```

---
## \#17 Posted by: JdogAwesome Posted at: 2016-11-08T23:20:17.878Z Reads: 148

```
@2-alex-2 yeah the SMD resistors are getting very hot on mine to but that's because it's fully charged. I don't actually think that I shoiuld be using the D- terminal because it's not properly driving the gates of the MOSFET and there getting very hot. I think that my BMS may be broken... So don't use the D- port because I also don't know if it will stop charging when the LiPo is full.
```

---
## \#18 Posted by: 2-alex-2 Posted at: 2016-11-08T23:36:16.740Z Reads: 146

```
Yea think I had a balance lead wrong that why mine were getting hot. But D- does stop on lvc but I will only be using a led indicator on D- and charge through P-/P+
```

---
## \#19 Posted by: ayospringroll Posted at: 2016-11-08T23:51:31.403Z Reads: 140

```
Would you mind showing a picture of how your BMS is wired with the LED?
```

---
## \#20 Posted by: JdogAwesome Posted at: 2016-11-08T23:53:32.902Z Reads: 139

```
@2-alex-2 what do you mean by lvc and hvc?
```

---
## \#21 Posted by: 2-alex-2 Posted at: 2016-11-09T08:20:02.161Z Reads: 124

```
Will do once it's all wired up. But what I hope it will do is if a set of cells become unbalanced and drop lower then led will got off. As esc will only detect the overall voltage. Lvc= low voltage(so you discharge side)  cutoff Hvc= hivoltage cutoff(so you charging side)
```

---
## \#22 Posted by: JdogAwesome Posted at: 2016-11-14T15:03:58.531Z Reads: 119

```
Ended up being that my BMS was not working properly so I contacted the seller on AliExpress and he shipped me a new one. Will update this post to make sure that using a new BMS fixes the problem.
```

---
## \#23 Posted by: ayospringroll Posted at: 2016-11-18T00:49:48.036Z Reads: 119

```
Did you ever get the BMS working? I just got mine in the mail and I wanted to see how you wired yours.
```

---
## \#24 Posted by: JdogAwesome Posted at: 2016-11-18T05:24:52.375Z Reads: 118

```
Not yet but once it arrives ill put up a diagram of how I wired it so you can see.
```

---
## \#25 Posted by: 2-alex-2 Posted at: 2016-11-18T08:37:16.418Z Reads: 110

```
I haven't finished it yet battery is connected but I currently do have a charger for this yet.
```

---
## \#26 Posted by: 2-alex-2 Posted at: 2016-11-18T15:02:18.769Z Reads: 104

```
@JdogAwesome what charger are you using anyway.
```

---
## \#27 Posted by: JdogAwesome Posted at: 2016-11-18T15:29:58.730Z Reads: 106

```
@2-alex-2 I'm using the BMS to control the charging but for a power supply I'm using this, 
 http://s.aliexpress.com/RRF3URVb
```

---
## \#28 Posted by: JdogAwesome Posted at: 2016-11-18T15:39:44.161Z Reads: 106

```
@2-alex-2 im also going to be using [this](http://www.ebay.com/itm/371462338310?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT) to finer control the voltage and current limit of the PSU. If you get a little nicer PSU that has current limiting in it then you'd wouldn't need this but mine doesn't have it. And if you dont mind waiting a couple weeks for shipping from china [this](http://www.ebay.com/itm/DC-DC-CC-CV-Buck-Converter-Step-down-Power-Supply-Module-7-32V-to-0-8-28V-12A-XG/282240615119?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D39107%26meid%3D310e2ca924ed4372880ab14b419afde6%26pid%3D100005%26rk%3D1%26rkt%3D6%26sd%3D282197484000) ones a tad bit cheaper.
```

---
## \#29 Posted by: 2-alex-2 Posted at: 2016-11-18T18:33:58.248Z Reads: 109

```
Yea I already have the socket but my lipo/liion  charger won't just charge it has to balance charge which it's a pain.
```

---
## \#30 Posted by: JdogAwesome Posted at: 2016-11-18T21:09:26.185Z Reads: 109

```
Oh you mean without using a BMS? I was using an Imax B6 but I killed it now im using a Hitec Multi Charge X1 AC which is literally just an Imax B6 AC but with a different body and a lot more expensive lol.
```

---
## \#31 Posted by: 2-alex-2 Posted at: 2016-11-18T21:17:06.059Z Reads: 107

```
Not been looking at laptop power supplies but not sure if would be suitable. Like what happens to the power when the bms turns of with over voltage ?
```

---
## \#32 Posted by: JdogAwesome Posted at: 2016-11-18T23:18:16.823Z Reads: 102

```
Id recommend using a PSU like the one I linked but if you want to use a laptop one that would work if you can find one for 25.2V. And when the BMS shuts off it just stops saturating the MOSFET's that let current through so it stops drawing current to charge the LiPo.
```

---
## \#33 Posted by: 2-alex-2 Posted at: 2016-12-23T18:07:48.673Z Reads: 96

```
Finally got mine wired up and it accepts a charge but no voltage coming out of P-,P+ so think mines faulty as well have message seller see if they send a new one or not.
```

---
## \#34 Posted by: ayospringroll Posted at: 2016-12-27T13:08:57.615Z Reads: 92

```
You should have your charging device be connected to P- P+. A voltage should be coming out of B- B+ where the batteries should be connected to. Thats how i have my BMS wired and it works fine without a problem. If it helps im using a 25.2V laptop charger to charge my 6s system.
```

---
## \#35 Posted by: 2-alex-2 Posted at: 2016-12-27T18:27:59.055Z Reads: 90

```
Yea but power should also come out of P-P+ as that's how the low voltage cutoff works if you don't use P your bypassing the bms for discharge and only using th bms for charging. Which is what I want to do but was going to use P- for an led indicator so that is bms pics up a dead cell the led will go off.
```

---
## \#36 Posted by: pau Posted at: 2017-06-22T09:39:56.137Z Reads: 79

```
hey what kind of psu did you use.
is it the same like this
[psu](https://www.ebay.de/i/252467458994?chn=ps&dispItem=1&ul_ref=http%253A%252F%252Frover.ebay.com%252Frover%252F1%252F707-134425-41852-0%252F2%253Fmpre%253Dhttps%25253A%25252F%25252Fwww.ebay.de%25252Fi%25252F252467458994%25253Fchn%25253Dps%252526dispItem%25253D1%2526itemid%253D252467458994%2526targetid%253D295891958382%2526device%253Dm%2526adtype%253Dpla%2526googleloc%253D9042959%2526poi%253D%2526campaignid%253D804030660%2526adgroupid%253D42479307755%2526rlsatarget%253Daud-318516063737%253Apla-295891958382%2526abcId%253D1078836%2526merchantid%253D112387644%2526gclid%253DCj0KCQjw1a3KBRCYARIsABNRnxvCvJetnHhEQhOvNRW3Q6rZpw5SKPe50_1Lh2Yw7tJwegH6h7My5VEaAsZvEALw_wcB%2526srcrot%253D707-134425-41852-0%2526rvr_id%253D1238917545652)

my doesnt not stable draw current.
it goes up and down. between 0,4A - 1A 
but it shuld be 4,5A

and i connected the psu directly to the batty. without bms. just for trying
```

---
## \#37 Posted by: JdogAwesome Posted at: 2017-06-22T22:32:05.559Z Reads: 77

```
Yeah that's the type of PSU I use, except it's a 24V 10A one.
```

---
## \#38 Posted by: pau Posted at: 2017-06-27T19:29:11.616Z Reads: 74

```
how did you wired it up? because there two plus connectors and two minus connectors?
```

---
## \#39 Posted by: JdogAwesome Posted at: 2017-07-02T05:35:29.748Z Reads: 67

```
Hey sorry for the late reply been crazy busy recently, not sure what you mean exactly, are you talking about the multiple PSU outputs or the inputs to the BMS?
```

---
## \#40 Posted by: pau Posted at: 2017-07-02T19:13:44.558Z Reads: 65

```
no worries.
psu outputs.
```

---
## \#41 Posted by: JdogAwesome Posted at: 2017-07-03T00:36:27.213Z Reads: 57

```
On the PSU terminal block theres 3 input terminals for the AC connections L, N and Ground (Live and Neutral for L and N) and then there are a couple + terminals and a couple - terminals, there all connected together and are there just so you can connect multiple wires if need be.
```

---
## \#42 Posted by: Charles Posted at: 2017-07-24T22:03:28.783Z Reads: 49

```
hey there @JdogAwesome i have the same one and was wondering the same thing that @Maxid was wondering. how does a 6s battery result in a 5s cable? also could you send a digram of how you wired the whole thing up ?
```

---
## \#43 Posted by: Maxid Posted at: 2017-07-25T05:10:58.166Z Reads: 52

```
Dude he explained it right after me asking that question.
```

---
## \#44 Posted by: Charles Posted at: 2017-07-25T13:40:08.544Z Reads: 51

```
So on both the batteries the red balance cables are soldered to each other and one of the red cables has two wires soldered to it
```

---
## \#45 Posted by: Maxid Posted at: 2017-07-25T13:48:03.616Z Reads: 51

```
??????? :confused:

It is in the third post - make sure you understand what the picture shows.
If you don't understand that, don't build a battery!
http://www.electric-skateboard.builders/t/lipo-6s-bms-balance-charging-problems/12593/3?u=maxid
```

---
## \#46 Posted by: Charles Posted at: 2017-07-25T14:14:49.047Z Reads: 52

```
I'm not building a battery ( I really can't do that ) I'm using ones from hobby king . The thing is that in the pictures on the first post it looks there are 5 wires comin out of the BMS and you said that they usually omit the ground wire. but there are two batteries so he omitted the ground on both of them. But then one of the connections on one of the batteries has two wires soldered to it. I hope that wasn't confusing. It's my first build so I'm just figuring things out. :worried: if you could help me that would be really appreciated

<img src="/uploads/db1493/original/3X/6/3/63d2e0db6c7e9f19ad5767befd10ad898b97528d.JPG" width="690" height="388">
```

---
## \#47 Posted by: Maxid Posted at: 2017-07-25T14:39:24.714Z Reads: 48

```
you are confusing serial connecting two 3S batteries with BMS connecting.
The BMS he showed had 5 connectors because the sixth cell was connected to the main port just like ground.
So 7-2=5.
```

---
## \#48 Posted by: Charles Posted at: 2017-07-25T14:50:22.012Z Reads: 48

```
What is main port and what is ground im sorry I'm really stupid :joy:
```

---
## \#49 Posted by: ReeCorDs Posted at: 2017-11-24T15:44:10.356Z Reads: 33

```
Can someone help me please to complete my wiring diagram? I do not understand it :disappointed_relieved:

That would be very very nice! :slight_smile: 

<img src="/uploads/db1493/original/3X/6/7/674e5cf4c293f4d336856bd3abc9f0f5ab072e11.jpg" width="690" height="331">
```

---

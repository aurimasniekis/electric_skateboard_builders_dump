# Lipo bms 60A or bypass?

### Replies: 12 Views: 1043

## \#1 Posted by: m4almbergs Posted at: 2017-07-21T18:36:37.668Z Reads: 145

```
I am currently planing on doing a 8s lipo bms battery set up and have some questions i can't find the answer to in any thread ( or mixing answers, some say yes some say no....) 

i am planing to use 5 x 8000mAh 2S1P 30C for my 8s pack, and this bms/charger [bms](http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html)/[charger](http://www.batterysupports.com/29v-336a-5a-lithium-ion-battery-charger-8s-8x-36v-lion-lipo-p-261.html) from battery supports 

the most important question is if I 60A bms is enough? (when searching the forum about this some say yes and still many people opt for a 80A or 100A one)  If 60A in not enough i have to bypass the bms for discharge sens ther is no 80A or 100A bms for 8s, many people do bypass the bms but whit li-ion can you do that whit lipo? 

from what i have seen the vesc can only handle 50A continuously any why so 60A bms shuld not bottleneck it right?  I know that the vesc can handle much higher peak amp but what about the bms is it 60 continuously? if so what peak can it handle. 

i am asking kind of specific questions about the particular bms from battery supports but i know a lot of people use the bms and charger her so any one ho have one  and know the answer to thes questions would be highly appreciated!
```

---
## \#2 Posted by: ninja Posted at: 2017-07-21T19:16:53.798Z Reads: 139

```
60A bms is enough!! Don't bypass it. Bms have many protections, also overcurrent protection, so it will not allow drain more like 60A from your battery. I have 60A BMS from batterysupport.com  and it works like charm. Actually I never seen current drawn from battery even close to 60A on my rides.
```

---
## \#3 Posted by: TowerCrisis Posted at: 2017-07-21T19:25:22.878Z Reads: 134

```
I'd have to agree with @ninja. I've also got a 60A BMS from them. Although my build isn't complete, it works like a charm.


Side story, my first build was very sketchy. It had two 6S cells, each with its own BMS, connected in parallel because the BMS I had was rated for low current. So I put them in parallel to double the max battery current. Anyways, the limit ended up being around 30A, and even with that I was able to comfortably accelerate and climb steep hills. 60A is plenty, but I wouldn't go lower to guarentee that it's safe.
```

---
## \#4 Posted by: m4almbergs Posted at: 2017-07-21T19:29:04.336Z Reads: 123

```
okey thank you! sound really good. my motor can handel 100 amp and batteries can out put much more than 60 so i din't want my bms to bottleneck my system that is all. 

[quote="ninja, post:2, topic:28214"]
Actually I never seen current drawn from battery even close to 60A on my rides.
[/quote]
really? interesting not even during steep hills or start from standstill?  what is  the max amp draw you recorded?
```

---
## \#5 Posted by: m4almbergs Posted at: 2017-07-21T19:32:03.081Z Reads: 116

```
good to know that more than only 1 think 60A is enough.:+1: 

haha wow that really sounds sketchy! i would not dare to ride that.

@ninja what battery set up do you have? lipo or li-lion?
```

---
## \#6 Posted by: TowerCrisis Posted at: 2017-07-21T19:39:15.881Z Reads: 115

```
Not sure how new you are to this, but when I was first setting up my VESC it surprised me.

The battery current and the motor current are different. Looking at the graphs in the bldc tool, you can see this. During my tests, my motor was drawing ~20A when I gave it some resistance, but the vesc was only drawing around 3A from my power supply. This is because battery voltage and VESC output voltage are usually not the same. The most common time your battery voltage and motor voltage will be the same is when you are at your max speed, which takes less current than when you're accelerating.
```

---
## \#7 Posted by: ninja Posted at: 2017-07-21T19:40:05.852Z Reads: 108

```
Never ride from stand still, I always push to start, but normally on flats I had 10A - 20A max.  On the hill it was 40 max., if I remember correctly.

I have li ion, samsung 25r, 8s4p, single drive, sk3 245kv., 83mm wheels.

Anyways on the vesc you'll never set more A on batt max like BMS has, so no worry!
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-21T19:49:06.155Z Reads: 106

```
I've got this BMS in my 8s4p li-ion pack. To be honest, I thought 60A wasn't enough as my pack could put out 80A, but then my motor is only rated for 60A! :confused:
 
I'm bypassing discharge through the BMS, I've been using it for a couple of weeks like that now and it's working well, I'm not sure how good it would be not bypassing it though...

I'm charging with a 33.6v 2A charging brick through a DC Jack.
```

---
## \#9 Posted by: ShutterShock Posted at: 2017-07-21T22:01:00.499Z Reads: 100

```
I got the 60A 12S bms from batterysupports.com (SuPower) too!  I'm still waiting for it to come in the mail, but I'm planning to run with the 60A protection too.
```

---
## \#10 Posted by: m4almbergs Posted at: 2017-07-21T23:00:44.917Z Reads: 99

```
i will run a 200kv motor from esk8.de and 83mm wheels ( about the same as you.. kind of) so it is realy nice to hear you say this :point_down: I will go for the 60A one and not bypass it. [quote="ninja, post:7, topic:28214"]
Anyways on the vesc you'll never set more A on batt max like BMS has, so no worry!
[/quote]

@darkkevind how come you say that 60A wasn't enough? ninja also have a battery that can put out more than 60A and acording to his findings the amp draw from battery never got close to 60A. this is the contrary opinions about this subject I don't understand......:thinking:
```

---
## \#11 Posted by: m4almbergs Posted at: 2017-07-21T23:05:58.857Z Reads: 87

```
any one have the 5A charger i [linked](http://www.batterysupports.com/29v-336a-5a-lithium-ion-battery-charger-8s-8x-36v-lion-lipo-p-261.html) or a similar one? is it any good? dose the fan get loud? I prefer the 5A one if it is not to loud sens i will be abel to charge my batteries in abot 2h insted of 5 whit the 2A one. and i will still be charge under 1C so it shuld be fine for my lipos right?
```

---
## \#12 Posted by: darkkevind Posted at: 2017-07-21T23:59:12.541Z Reads: 85

```
No, I said I thought it wouldn't be enough.. turns out it is.
```

---

# Final Compatibility check!

### Replies: 48 Views: 1854

## \#1 Posted by: pigeonic Posted at: 2017-02-25T16:59:59.516Z Reads: 152

```
I've been in limbo for the past month because I'm afraid my setup wont work properly. So here it is!

Batteries:
https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html x6 (4 in Series 2 in parallel. 8s2p)

Charging:
https://hobbyking.com/en_us/turnigy-accucel-8-150w-7a-balancer-charger.html
https://hobbyking.com/en_us/turnigy-reaktor-pro-350w-23a-power-supply-100-240v-ac.html

BMS:
https://hobbyking.com/en_us/8s-li-ion-pcm-charge-5a-discharge-15a.html

Motor:
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html

Would this be ok? 

(yet to purchase a vesc)
```

---
## \#2 Posted by: Sander Posted at: 2017-02-25T17:08:43.730Z Reads: 142

```
You know right your max ampere usage must be below 15A or the BMS will get cooked. And that means your batteries are kinda overkill/useless because they have such high discharge rate.
```

---
## \#3 Posted by: pigeonic Posted at: 2017-02-25T17:13:50.060Z Reads: 133

```
Any suggestions? Saw this batteries being used in another post. So i thought it'd be great
```

---
## \#4 Posted by: makevoid Posted at: 2017-02-25T17:14:52.809Z Reads: 124

```
maybe use it only for charging and bypass it for discharging?
```

---
## \#5 Posted by: pigeonic Posted at: 2017-02-25T17:18:33.518Z Reads: 117

```
use the BMS for charging but bypass it for discharging? wont it kill the batteries quicker since the motor sucks power rapidly
```

---
## \#6 Posted by: Sander Posted at: 2017-02-25T17:18:58.067Z Reads: 111

```
Everything is perfect expect for the BMS, the bms only tolerate up to 15A, and your motor 80A. So you will not get the max power with that bms because the max is 15a and it will fry. If you bypass it like @makevoid said, only use it for charging. Then everything should work just fine :)
```

---
## \#7 Posted by: pigeonic Posted at: 2017-02-25T17:20:43.818Z Reads: 105

```
Like what I posted earlier. I'm just afraid that the batt will be killed rapidly? (something about rapid discharge destroying batteries?) without the bms.
```

---
## \#8 Posted by: Sander Posted at: 2017-02-25T17:21:55.030Z Reads: 102

```
[quote="pigeonic, post:7, topic:18233, full:true"]
Like what I posted earlier. I'm just afraid that the batt will be killed rapidly? (something about rapid discharge destroying batteries?) without the bms.
[/quote]

I don't think you should be worried about that.
```

---
## \#9 Posted by: pigeonic Posted at: 2017-02-25T17:24:21.915Z Reads: 92

```
Let's hope you're right. I'll be scouring for a higher A bms at the same time
```

---
## \#10 Posted by: pigeonic Posted at: 2017-02-25T17:25:15.593Z Reads: 91

```
Also asking, will the VESC be able to manage the amount of power going into the motor?
```

---
## \#11 Posted by: Sander Posted at: 2017-02-25T17:25:52.985Z Reads: 87

```
No problems, the VESC is 60V and 240A.
```

---
## \#12 Posted by: pigeonic Posted at: 2017-02-25T17:28:08.395Z Reads: 82

```
so in summary, would it still be necessary for a BMS?
```

---
## \#13 Posted by: Sander Posted at: 2017-02-25T17:30:06.307Z Reads: 84

```
[quote="pigeonic, post:12, topic:18233, full:true"]
so in summary, would it still be necessary for a BMS?
[/quote]

You don't really need a BMS. Only if you want to charge your board like a laptop(one wire).
```

---
## \#14 Posted by: makevoid Posted at: 2017-02-25T17:31:36.852Z Reads: 75

```
maybe you could add an anti spark switch or a fuse at least against rapid discharge (ex: faults / short-circuits)
```

---
## \#15 Posted by: pigeonic Posted at: 2017-02-25T17:33:15.958Z Reads: 76

```
I'd really like to charge with one wire :joy:
```

---
## \#16 Posted by: pigeonic Posted at: 2017-02-25T17:34:35.707Z Reads: 79

```
do I also have to utilise a voltmeter(?) like what onloop recommends?
```

---
## \#17 Posted by: makevoid Posted at: 2017-02-25T17:41:00.182Z Reads: 82

```
I suggest to search for somebody who knows electric circuits before/while connecting everything together to prevent you creating a short circuit. With any battery but with lipos more than others you risk to make the battery damage itself because of a short circuit.The multimeter lets you test that the current is flowing in the direction you want (checking voltage), and if you turn the knob to the Ω part of the "pie" you will be able to check resistance (for example if a end of a wire is connected to the right end, to see if a material is conductive etc). So either learn some basic things about circuits or get a help from somebody that knows and if you can get a multimeter, get it. ^^
```

---
## \#18 Posted by: pigeonic Posted at: 2017-02-25T17:45:59.485Z Reads: 77

```
Appreciate the advice. Will definitely read more myself and find someone!
```

---
## \#19 Posted by: Namasaki Posted at: 2017-02-25T21:18:51.131Z Reads: 71

```
Excellent battery choice!
And don't let anyone tell you these batteries are overkill. They are not. 
Even with these batteries, there will be a little voltage sag. 
But much less sag than lower power batteries.
```

---
## \#20 Posted by: Sander Posted at: 2017-02-25T21:24:41.214Z Reads: 71

```
[quote="Namasaki, post:19, topic:18233"]
And don't let anyone tell you these batteries are overkill
[/quote]

I said it was overkill for a 15A Bms, not for a 60A bms.
```

---
## \#21 Posted by: Namasaki Posted at: 2017-02-25T23:19:54.939Z Reads: 64

```
Actually I was not referring to anything you said. Or anything that had been previously posted on this thread.
In Fact, I agree with everything you've said in this thread.
I just thought I would throw that in just in case someone later came around saying that the batteries where a bad choice because they're  overkill.
Because I have found through testing that having a battery pack capable of 10X the current needed is a really good thing. Voltage sag is greatly reduced which equals better performance and better range. However, there are some who believe that a 60a battery pack is plenty for an E-skate and sure it can be in certain situations. I once had such a 10s battery on my build and it worked fine on flat ground but as soon as I started tackling hills, my range was cut more than in half because of excessive voltage sag.
```

---
## \#22 Posted by: pigeonic Posted at: 2017-02-26T05:44:55.328Z Reads: 60

```
I'll take note! Thanks!!
```

---
## \#23 Posted by: NickTheDude Posted at: 2017-02-26T05:59:11.529Z Reads: 57

```
[quote="pigeonic, post:1, topic:18233"]
https://hobbyking.com/en_us/turnigy-5000mah-2s-7-4v-60c-hardcase-pack.html x6 (4 in Series 2 in parallel. 8s2p)
[/quote]

You'll need 8 of those. Two 8S packs wired in parallel would give you 8S2P.
```

---
## \#24 Posted by: pigeonic Posted at: 2017-02-26T06:14:32.613Z Reads: 52

```
the packs are 2s each, so just 4 of them to form 8s and another 2 in parallel to from 2p no?
```

---
## \#25 Posted by: NickTheDude Posted at: 2017-02-26T06:16:40.457Z Reads: 55

```
You'd need to make 2 separate 8S packs and then wire those two packs in parallel.
```

---
## \#26 Posted by: pigeonic Posted at: 2017-02-26T06:19:51.447Z Reads: 56

```
Right I see, totally forgot about that. Don't think I have enough real estate on my board though. Any alternatives?
```

---
## \#27 Posted by: pigeonic Posted at: 2017-02-26T06:23:28.290Z Reads: 58

```
wait actually, I don't see how I cant wire just 2 separate packs in parallel?
```

---
## \#28 Posted by: Namasaki Posted at: 2017-02-26T06:50:54.467Z Reads: 61

```
@NickTheDude Is absolutely correct and for the life of me I don't know why none of the rest of us caught that! 
In order to to have 8s 2p you need 16 cells or eight 2s packs. 
You might consider a 10s 1p using 5 packs which is smaller and lighter and a better match for a 192kv motor. You will have a little more top speed and still get 10+ miles of range. Use a good 10s BMS and a brick charger. (This is the setup I use)
Or 8s 1p with your balance charger if you don't mind a little less top speed and range. 
I'm guessing around 20+ mph and 8+ mile range.
```

---
## \#29 Posted by: pigeonic Posted at: 2017-02-26T10:14:57.664Z Reads: 59

```
I am actually seriously considering getting enertion's space cell pro 3. As all these parts (batteries and chargers) quite a sum just to bring them into singapore. What do you think of the space cell pro 3/4?
```

---
## \#30 Posted by: Namasaki Posted at: 2017-02-26T14:48:10.508Z Reads: 55

```
It is my opinion that a battery pack with 60a capability is fine for flat land riding but if you have lots of hills to ride then you need more power which means higher current capability.
This is my situation and why I built a 300a battery pack. 
Because when I tried to use a 60a pack, I suffered extreme voltage sag which greatly reduced range. 
But not on flat ground, riding at moderate speed.
```

---
## \#31 Posted by: DaveMess Posted at: 2017-02-26T15:42:07.280Z Reads: 51

```
Yeah I was reading through this and I'm like "uuuhhh guys he's got 12 cells somehow arranged 8s2p" haha whew glad you guys saw it. The 2P doesn't refer to having 2 extra batteries in parallel. It refers to having a second 8s battery in parallel ( so think 8s x 2). If you only put the 2 batteries in parallel you'd be trying to feed you VESC with one 8s pack and one 4s pack. idk exactly what will happen there but it will never be good for the poor 4s pack trying to support such a high load. Just grab 2 more packs and you'll have a wicked powerful 8s2p that can push like 250a if you need it to.
```

---
## \#32 Posted by: Esrapp21 Posted at: 2017-02-27T00:12:42.377Z Reads: 44

```
Wait, I think I am missing something. Do you really need both a bms AND a balance charger? I figured one would be enough. Is the bms for discharge?
```

---
## \#33 Posted by: pigeonic Posted at: 2017-02-28T09:51:57.447Z Reads: 40

```
Do I not need a BMS and a Balance Charger for the batteries? Hell, is a BMS even neccessary at all??
```

---
## \#34 Posted by: Esrapp21 Posted at: 2017-02-28T12:30:16.723Z Reads: 38

```
The purpose of a balance charger is to charge each cell equally to balance voltage. The point of a BMS is to disperse the incoming power equally among the cells. However, the BMS can also limit discharge, but the VESC shouldn't cause a problem for discharge if set up right.
```

---
## \#35 Posted by: Esrapp21 Posted at: 2017-02-28T12:41:06.820Z Reads: 41

```
The good thing about a BMS though is you can solder it inside the board and just charge the board with a laptop charge with the right amps and volts. Bad thing about BMS is you can't really check on it easily to see if it is still working well and doing its job.

Good thing about balance charge is it is very reliable to get you a good charge. Some also have different settings for different types of charges, such as to put it in storage it can somewhat drain the battery. The bad thing about the balance charger is the user interface and process. You have to set your battery preferences, plug the positive, negative, and balance lead in, and select your charge every time. So if you plan on loaning it to a friend, you will have to give them a tutorial on that.
```

---
## \#36 Posted by: pigeonic Posted at: 2017-03-01T17:03:25.157Z Reads: 39

```
I calculated  the price overall, and it is similarly priced to the space cell pro 4, should I just get that instead?
```

---
## \#37 Posted by: Esrapp21 Posted at: 2017-03-01T18:23:00.127Z Reads: 37

```
I had the same idea. I got the sc3 because it was about the same price otherwise but it had a warenty from one company instead of a few from multiple.
```

---
## \#38 Posted by: pigeonic Posted at: 2017-03-02T07:57:48.657Z Reads: 36

```
Is it reliable?
```

---
## \#39 Posted by: Esrapp21 Posted at: 2017-03-02T13:01:51.118Z Reads: 38

```
I actually just finished it the other day, and due to rain I haven't tested it yet. I will hopefully test it later today. But from what I have heard from other people, I think it is pretty reliable.
```

---
## \#40 Posted by: pigeonic Posted at: 2017-03-04T09:48:16.008Z Reads: 37

```
Just a question to put out there, what's the minimal voltage (literally the lowest possible) to run an e-board?
```

---
## \#41 Posted by: Esrapp21 Posted at: 2017-03-04T12:45:02.732Z Reads: 35

```
Probably a 6s is the absolute lowest voltage you want, but most people do 8s or above. With 6s don't expect much power wise.
```

---
## \#42 Posted by: pigeonic Posted at: 2017-03-04T15:28:08.407Z Reads: 33

```
In that case, placing a car battery wouldn't work then (?). I might be considering to build a custom battery pack, hell I want to build one as it is cheaper for me to access those cells, will it be tough to build one?
```

---
## \#43 Posted by: Esrapp21 Posted at: 2017-03-04T15:46:02.946Z Reads: 31

```
Most car batteries have high amps, low volts I believe. Plus the chemistry of the battery is off so there won't be as much support on the forum for that. A lot of people build there own custom battery, and if you have the materials (spot welder, nickel strips, cells) then that is a great solution.
```

---
## \#44 Posted by: pigeonic Posted at: 2017-03-04T16:39:56.873Z Reads: 32

```
Those stuff are easy to get here, and at a really great price. Probably will learn how to build one, and lay off my board for the next few weeks or so
```

---
## \#45 Posted by: pigeonic Posted at: 2017-03-08T14:13:21.137Z Reads: 26

```
Bump this chat a lil' I managed to get my hands on some LG 18650 S3 2200mAh (Blue) batteries recycled off some laptop batteries, is it good ? @barajabali
```

---
## \#46 Posted by: barajabali Posted at: 2017-03-08T14:40:52.910Z Reads: 26

```
its not good unless you're running in like 20p or something. <img src="/uploads/db1493/original/3X/8/8/8840235fcee148ce37b63d1fcc78a3010b53c573.PNG" width="281" height="500">
```

---
## \#47 Posted by: pigeonic Posted at: 2017-03-08T16:16:27.152Z Reads: 22

```
What batt's would you recommend then, ones that are bang for buck, and where to get em?
```

---
## \#48 Posted by: barajabali Posted at: 2017-03-08T16:31:09.163Z Reads: 21

```
Best value are the Samsung 25Rs.
```

---

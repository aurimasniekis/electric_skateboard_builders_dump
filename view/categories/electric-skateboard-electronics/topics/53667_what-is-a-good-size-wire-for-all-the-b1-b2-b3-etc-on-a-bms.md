# What is a good size wire for all the B1+, B2+, B3+ etc. on a BMS?

### Replies: 19 Views: 992

## \#1 Posted by: ToucanSam Posted at: 2018-04-27T16:25:23.178Z Reads: 118

```
I am going to be using the BMS for charging purposes only.

I notice that the B- wire to the BMS is a larger wire and all the B1+, B2+, B3+ wires are smaller.

**What size wire is good for all the little + wires?**

I am putting together a 12s6p battery made of Samsung 30q cells and I have a 12s 150A BMS on the way from SuPower Battery.
[This is the BMS I have ordered.](http://www.batterysupports.com/44v-48v-504v-12s-150a-12x36v-lithium-ion-lipolymer-battery-bms-p-394.html)

I already have all my cells spot welded together [like this.](https://imgur.com/a/WlHKjq3)

I just have to solder on the final positive and negative terminals, and all the little BMS connections.

I hope this is enough information to explain my question, thank you for your time :slight_smile:
```

---
## \#2 Posted by: Mathias Posted at: 2018-04-27T16:55:52.442Z Reads: 113

```
There is the very important distinction between those wires that conduct the full battery current on discharge (also on charge), and those that are only there to balance. 
In general it is a good idea to go with very high current rating for discharge cables, such as B-, P-, or the wires that connect of the series cells to each other (I guess the thick red and black ones from your photo). 

For the balance cables B1+ etc it is the opposite: looking at the specs of your BMS, it has a max balance current of 60 mA. So I would be a good idea to go with cables that are rated for few 100 mA. The only reason why there could ever be much higher current through those would be a short, and in that case if you are lucky the cable fuses out and prevents your battery from getting damaged or even catching fire. For cables like that going far above what is needed, doesn't make it safer. 

[quote="ToucanSam, post:1, topic:53667"]
I am going to be using the BMS for charging purposes only.
[/quote]

You mean you bypassed it? But why get a 150 A BMS then? Or am I getting this wrong? 

Be careful with the discharge. Your BMS is fused with 150 A, but I doubt that your discharge cables can take that much. This wouldn't really be ideal, since your cables are a weaker link in the chain than the fuse. If you bypassed the BMS, I would suggest to solder in a fuse at some other point. I also have a bypassed BMS but I have a soldered a fuse right at one of the battery terminals. 

For the discharge cables it really depends on your setup. They need to be able whatever you'll set as combined battery current for all your ESCs. 
What are those cables in your photo rated for? How does it compare to your setup? I guess you'll be fine unless you run 4 extremely strong motors with strong 4 ESCs. With two VESC4 you won't melt those cables for sure. Four VESC6 without extra care would be a battery fire waiting to happen.
```

---
## \#3 Posted by: ToucanSam Posted at: 2018-04-27T17:12:47.715Z Reads: 94

```
I was told to get a BMS rated for more than what my battery could produce, since this battery should be capable of 90A to 120A I picked out a 150A BMS. Is this wrong? I don't really know how they work I'm just following instruction for the BMS.

Also I will be running dual 6374 motors. I have a couple VESC's from Torque Boards on the way. The VESC6 was just too expensive -.-
```

---
## \#4 Posted by: Mathias Posted at: 2018-04-27T18:25:36.432Z Reads: 83

```
I was confused by this:
[quote="ToucanSam, post:1, topic:53667"]
I am going to be using the BMS for charging purposes only.
[/quote]
If you do not discharge through your BMS, like many people here including me prefer to do, then there is no point in getting a 150 A BMS. I have a 20 A BMS, because that's enough for charging and balancing, as long as it's bypassed. In that case you could have saved a lot of money. But as I said: one should still put a fuse at some point. 

In general I don't agree that one should use a BMS that is fused at more than the battery can do. That defeats the whole point. The BMS is fused, so it breaks the circuit at a current BEFORE the battery gets damaged. I mean 150 A will still protect you from a dead short in some cases, but it won't protect the battery in all cases, since it allows much more current than the battery can safely provide. The fuse should be the weakest link. Never the battery or the wires. 

But in any case: you'll probably be fine since your to VESC4 will not be able to draw extremely high current for enough time to damage your wires or your battery. But just to be on the safe side: what current are your discharge wires rated for?
```

---
## \#5 Posted by: ToucanSam Posted at: 2018-04-27T18:53:05.105Z Reads: 72

```
I should still be able to cancel my BMS order. You recommend a 20A for charging then?

Also I will have to check on the amperage rating for my wires when I get home in a few hours. They should be perfectly fine for more than what im pushing though. I'll get back to you on that.
```

---
## \#6 Posted by: E1Allen Posted at: 2018-04-27T19:39:22.327Z Reads: 77

```
![2017-09-03_131833|583x500](upload://1AQ6YyIbKHWtJznPxlisiONywB5.jpg)

The balance leads. B1,2,3,4 ect carry very little current.  Any one of these small wires will work for the balance current.  30ga even has 800mah rating and that's with a much longer wire than a balance lead.
```

---
## \#7 Posted by: Mathias Posted at: 2018-04-27T21:20:52.292Z Reads: 65

```
I'm using this one (you'd need to find a 12s one of course):
https://www.ebay.com/itm/Battery-Protection-BMS-PCB-Board-for-10-Packs-36V-Li-ion-Cell-max-40A-w-Balance-/271803920379?hash=item3f48c6affb

Be careful when you pick one, that you have a decent balance current. But most anyway have around 40-60 mA. This is not much for a large pack, but my 4p pack was always perfectly balanced. Just make sure that the battery is balanced when you install it. The BMS will handle slow drifts. 

Some people will tell you otherwise and you can find plenty of discussions about bypassing BMS like this one:
https://www.electric-skateboard.builders/t/a-final-word-on-bypassing-bms-for-discharge/18351

But in my opinion there is no reason to use a BMS for discharge as long as you are using proper VESC settings and simply put a fuse, which you can get for a few dollars on ebay. On the contrary, I think a BMS is a potential source of cutouts of your brakes if you e.g. go downhill and your battery is almost fully charged. Many people use a BMS as a 100$+ fuse, and it is more dangerous than my 2$ fuse. The part of limiting the discharge current is perfectly covered by the VESC.
```

---
## \#8 Posted by: ToucanSam Posted at: 2018-04-27T21:53:21.000Z Reads: 55

```
Alright, well I cancelled the 150A order and I'll pick up a more reasonably priced one for 30-40A. I'll also order a fuse, what amperage fuse would you suggest for a 90-120A battery?
And does it matter where I put the fuse? I was gonna put it right down by my xt90 splitter near the vesc.
```

---
## \#9 Posted by: Mathias Posted at: 2018-04-27T22:16:14.334Z Reads: 52

```
I think 150% of your max current is a good size. As I said: depends a bit on the cables etc and on how much current you want to really draw. ~100 A on 12s is 4-5 kW of power, which is A LOT. And you will only draw it for a very short time. So if you really use all the juice you might go with 150 A. But then check if your cables can take 100 A! Many will not. I'm using 100 A fuse for 60 A max on 10s4p, and that's pretty powerful. 
You won't need the fuse to protect the battery in normal operation. That's done with the VESC battery current limit. This is in case a short in case e.g. a cable is damaged or something like that.

As for the position of the fuse: the closer to the battery terminal the better. If your discharge cables that go from the battery to the VESC get damaged, then a fuse at the splitter won't help.
```

---
## \#10 Posted by: ToucanSam Posted at: 2018-04-27T23:14:21.460Z Reads: 48

```
Okay cool well you've been very helpful thank you I appreciate all your information! I'll pick up a better BMS for just charging and I'll grab a fuse. I want to accelerate as fast as possible so I'll look at what current the cables can handle to judge which fuse to get. I want to set the VESC to let the current to each motor go up to 60 but between 2 motors that's all my battery can handle. Hopefully the cables are good 0.0
```

---
## \#11 Posted by: deucesdown Posted at: 2018-04-27T23:29:22.734Z Reads: 43

```
[quote="ToucanSam, post:1, topic:53667"]
What size wire is good for all the little + wires?
[/quote]

I like 22awg silly cone wires for the balance leads. It's a bit too big for the connector but any smaller or non-silicone and I feel they're too fragile.
```

---
## \#12 Posted by: ToucanSam Posted at: 2018-04-28T01:14:37.817Z Reads: 41

```
Okay so home now, I am actually using 14awg wire rated for 200 degrees Celsius but that's all the information I have about the wire you see in the picture above. Do we think maybe I should get myself some bigger wire? It will hurt my heart to have to heat up the batteries again but if I need bigger wire I need bigger wire.

Edit: For the record I can still use bigger wire on the final positive and negative terminals, those aren't soldered yet :slight_smile:
```

---
## \#13 Posted by: Mathias Posted at: 2018-04-28T02:00:29.865Z Reads: 38

```
Shit, I'm pretty sure 14 awg is not enough for these currents, sorry! I mean under normal conditions you will barely ever reach currents as high as 100 A, and probably only for a short time. But 14 awg is really pushing it... I would not risk 100 A discharge through those, even for a short time. 

And yeah, heating up the battery during soldering is an issue. Especially for an eboard, with the vibrations and all you don't want to risk a cold solder joint, and you really need to heat it up good. Best solution might be to solder to a new piece of Nickel strip, and the spotweld that one on top of the others, making sure that you have many weld spots for good contact and stability. 

The issues with building a monster board with 4 kW :joy:. This thing is going to be powerful. And thinking about it: The VESC4 will for sure be the bottle neck for the power of your board, and you should think about heatsinks. Otherwise you'll be down to 35 A or so continuous of motor current after they warm up.
```

---
## \#14 Posted by: ToucanSam Posted at: 2018-04-28T02:28:40.730Z Reads: 38

```
Hmm. I watched a video of some electricians soldering 18650 and according to them it doesn't hurt anything if you keep the heat source on for less than 5 seconds. Fingers crossed they're right but everyone says something different. 

I was looking into wire sizes and I guess I have to go over to Home Depot or something to find some good lower gauge wire. I looked at the National Electrician Code and some blog posts on picking wire sizes and I think 8awg would work perfectly as it's rated for 105A to 125A which will be fine. 

Do you think you can explain a little about the VESC4? Brush-less motors use higher amperage to accelerate and higher voltage for higher rpm as far as I know. So the VESC will only try to draw high amperage when accelerating at lower rpms. Will the VESC4 have over heating issues even if the higher amperage is only for a small time? It is rated for 240A Burst and 50A - 60A continuous. So I assumed that it wouldn't be the bottleneck because based on its specs it can handle the acceleration I'm going for. I can look into figuring out how to get a good heat sink onto them but they come packaged up pretty well -.- what am I missing that makes heating such a big issue?
```

---
## \#15 Posted by: Mathias Posted at: 2018-04-28T03:13:10.221Z Reads: 37

```
[quote="ToucanSam, post:14, topic:53667"]
Hmm. I watched a video of some electricians soldering 18650 and according to them it doesn’t hurt anything if you keep the heat source on for less than 5 seconds. Fingers crossed they’re right but everyone says something different.
[/quote]
It's definitely difficult...

8 awg is a lot, but that's definitely safe. As I said: 100 amp will be extremely rare, I'm sure. 

[quote="ToucanSam, post:14, topic:53667"]
Do you think you can explain a little about the VESC4? Brush-less motors use higher amperage to accelerate and higher voltage for higher rpm as far as I know. So the VESC will only try to draw high amperage when accelerating at lower rpms. Will the VESC4 have over heating issues even if the higher amperage is only for a small time? It is rated for 240A Burst and 50A - 60A continuous. So I assumed that it wouldn’t be the bottleneck because based on its specs it can handle the acceleration I’m going for. I can look into figuring out how to get a good heat sink onto them but they come packaged up pretty well -.- what am I missing that makes heating such a big issue?
[/quote]
It's not gonna be a bit issue I guess... Peak power is insanely high, and just from accelerating or flat ground riding you probably won't run into overheating issue. Only when you run at really high power at long time you'll be able to heat the ESC up so high that it reaches the 80°C and starts to reduce the power. 
I'm also running dual VESC4 with 6355 motors and 10s4p. I only reach 80°C when I do really fast and extended uphill riding. Then the torque and power reduction is definitely noticeable. But it's so rare in my case that I don't bother heatsinking. 
I just assumed from the huge battery and huge motors that you're going for really high end performance. You can just try for a while, maybe it will be fine for your riding style or the area you ride in. It's still gonna be a powerful board...
```

---
## \#16 Posted by: ToucanSam Posted at: 2018-04-28T04:53:56.506Z Reads: 30

```
Not gonna lie you're spot on with a goal being high end performance, and i'm kinda bummed about the heating thing so i'm definitely gonna look into cooling. But hey I think those are all my questions so thank you very much sir you have been of great assistance :smile:
```

---
## \#17 Posted by: Mathias Posted at: 2018-04-28T05:13:23.176Z Reads: 30

```
No problem, man! I love to talk about this shit :wink:
PS: Maybe look into FOCBox. Those come with heatsink housing...
```

---
## \#18 Posted by: MannyM0E Posted at: 2018-04-28T06:12:10.859Z Reads: 29

```
Mybad for interfering with your type convo. But I seen you said a fuse ! Closer to the batteries the better. Will it go to the pos/neg wire of the batteries?
```

---
## \#19 Posted by: rey8801 Posted at: 2018-04-28T06:25:05.742Z Reads: 29

```
Sorry to answer instead of you, but I read this interesting conversation and I though to contribute. For the last question. Only on the positive. Between battery and vesc is a good place.
About the BMS I used a BMS for discharge too, but next time I will also probably go for a charge purpose only. The cost, but also the space you saved under the deck is noticeable, moreover in case you build a short deck. As fuse you can also think about the one for Rc cars. Those are nice because in case the break the circuit you just need to reposition them. Here an example 100A 50A 60A 80A 150A  12V Car Truck Audio Amplifier Circuit Breaker Fuse Holder AGU Style Stereo Amplifier Refit Fuse Adapter
 http://s.aliexpress.com/BJZJV7RV?fromSns=Copy to Clipboard. Choose the right A.
```

---

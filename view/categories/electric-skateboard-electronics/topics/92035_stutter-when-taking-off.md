# Stutter when taking off

### Replies: 39 Views: 692

## \#1 Posted by: tkc Posted at: 2019-04-28T05:42:19.038Z Reads: 210

```
Hey guys, I’m having trouble with my setup. I have a Focbox Unity with Wowgo AT hub motors. Everything works great when I’m moving but starting off the motors stutter so I have to kinda kick start.

Is this something I can fix in the Unity app on my Android? I ran the setup for the motors and I’m running them sensored. I’m running everything at 60 amps output since that’s what my battery pack is.
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-04-28T05:48:32.287Z Reads: 205

```
What kv? And what gearing
```

---
## \#3 Posted by: TowerCrisis Posted at: 2019-04-28T05:48:40.703Z Reads: 200

```
If you have sensors and it's still stuttering, then it's likely a configuration issue. Are you sure it's running in sensored mode, and did you do the proper motor setup?
```

---
## \#4 Posted by: tkc Posted at: 2019-04-28T06:00:42.731Z Reads: 191

```
I don’t know the KV as Wowgo doesn’t publish that info. No gearing as the Wowgo AT motors are hub motors. And yes, as I said in OP I ran the setup and I’m running in sensored mode.
```

---
## \#5 Posted by: Jinra Posted at: 2019-04-28T06:21:17.525Z Reads: 180

```
what are your sensor readings
```

---
## \#6 Posted by: tkc Posted at: 2019-04-28T13:18:30.602Z Reads: 166

```
Not sure how to read them on the Unity? Is that something I do on the Terminal screen?
```

---
## \#7 Posted by: meesie Posted at: 2019-04-28T13:22:19.068Z Reads: 161

```
have you set them up in sensored FOC mode?
```

---
## \#8 Posted by: tkc Posted at: 2019-04-28T13:34:18.951Z Reads: 158

```
As I put in my original post, yes I did.
```

---
## \#9 Posted by: meesie Posted at: 2019-04-28T13:35:25.493Z Reads: 156

```
yes but are you using **_FOC_**
```

---
## \#10 Posted by: rich Posted at: 2019-04-28T13:41:31.083Z Reads: 153

```
[quote="tkc, post:8, topic:92035, full:true"]
As I put in my original post, yes I did.
[/quote]


Can't find any info there. I bet you run sensored BLDC mode that's why the motors are stuttering. You have to set them up in sensored FOC.

How big are you wings and at which speed you can take off? :wink:
```

---
## \#11 Posted by: tkc Posted at: 2019-04-28T13:55:51.293Z Reads: 148

```
Where can I confirm this setting in the app?
```

---
## \#12 Posted by: mmaner Posted at: 2019-04-28T14:07:06.704Z Reads: 143

```
[quote="tkc, post:8, topic:92035, full:true"]
As I put in my original post, yes I did.
[/quote]

Actually you didn't. There's is a very distinct difference between sensored and FOC. You might be a little more receptive to advice and do some research so you know what questions you ask.
```

---
## \#13 Posted by: Jinra Posted at: 2019-04-28T15:26:01.754Z Reads: 135

```
If you're using the app take a pic of your motor screen so we can see Hall positioning
```

---
## \#14 Posted by: tkc Posted at: 2019-04-29T01:13:00.776Z Reads: 132

```
![image|243x500](upload://eKKzPcv91LWSwlsAi2cROiPDJYb.jpeg)
```

---
## \#15 Posted by: tkc Posted at: 2019-04-29T01:20:03.227Z Reads: 127

```
Interestingly enough, I re-run setup and a small status bar at the bottom says “Both Motors Sensorless” for a split second. Perhaps the wires aren’t in the right place? I thought it was able to auto detect the various sensor wires too?
```

---
## \#16 Posted by: barajabali Posted at: 2019-04-29T01:25:49.372Z Reads: 126

```
You need to change the sensorless erpm value in the full tool.

Are you on the latest firmware? 23.43
```

---
## \#17 Posted by: tkc Posted at: 2019-04-29T01:38:56.467Z Reads: 125

```
When you say “full tool” do you mean the Windows app? Ugh, making my life so complicated with my Mac and iPhone! Haha. I’ll run a Windows VM and pray I can talk to the device. The firmware is the latest it said to upgrade to via the app, not sure the version #.
```

---
## \#18 Posted by: barajabali Posted at: 2019-04-29T01:42:27.207Z Reads: 124

```
Check the firmware tab to see which one you’re on. We released a new fw a week or so ago
```

---
## \#19 Posted by: Jinra Posted at: 2019-04-29T02:29:32.340Z Reads: 116

```
Those hall values are missing. Also your motor inductance values are widely different for some reason.
```

---
## \#20 Posted by: tkc Posted at: 2019-04-29T03:42:31.915Z Reads: 112

```
Yes, it’s currently 23.43
```

---
## \#21 Posted by: tkc Posted at: 2019-04-30T00:48:32.035Z Reads: 103

```
@barajabali any ideas for next steps?
```

---
## \#22 Posted by: barajabali Posted at: 2019-04-30T01:07:31.197Z Reads: 103

```
Send an image of your unity to motor connections. We will get it sorted
```

---
## \#23 Posted by: tkc Posted at: 2019-04-30T03:22:36.074Z Reads: 98

```
@barajabali Best I can do. I had to make my own wiring hardness so maybe I don’t have the pin outs correct. Of course Wowgo doesn’t tell you what’s what!

![image|666x500](upload://iafktLNsH1akp8UtBCUSUuGjvRo.jpeg)
```

---
## \#24 Posted by: tkc Posted at: 2019-05-01T21:51:36.756Z Reads: 96

```
@barajabali Any idea?
```

---
## \#25 Posted by: barajabali Posted at: 2019-05-01T21:54:03.694Z Reads: 97

```
It could literally be anything in that pile of wires man. So many solder points and connections..
But your app isnt reading your sensor values according to the image above so something has to be wrong with the wiring
```

---
## \#26 Posted by: tkc Posted at: 2019-05-01T22:31:45.160Z Reads: 92

```
Pile of wires? It’s a 1:1 relationship of sensor wires to wires coming into the Focbox. I have to use a cable ribbon between them because they don’t make an adapter from those motors straight to the Focbox. But I don’t know what wires go where. Isn’t the Focbox made to auto detect or no?
```

---
## \#27 Posted by: barajabali Posted at: 2019-05-01T22:33:25.103Z Reads: 91

```
Is your app still not detecting the sensors? 

I believe it autodetects most of them but there are some that matter I think @Blasto can you add your input?
```

---
## \#28 Posted by: Blasto Posted at: 2019-05-01T23:00:36.951Z Reads: 88

```
Well if the sensors are not detecting, the pin is not correct
```

---
## \#29 Posted by: tkc Posted at: 2019-05-01T23:01:25.924Z Reads: 90

```
Well I guess the biggest problem is that nobody knows the pin output on these wowgo motors. Who knows what colors mean what to them.
```

---
## \#30 Posted by: barajabali Posted at: 2019-05-02T00:08:26.426Z Reads: 89

```
Yea you can run sensorless though. Just increase the open loop erpm and you’ll get some better low end torque
```

---
## \#31 Posted by: tkc Posted at: 2019-05-02T02:41:33.001Z Reads: 82

```
I don't mind running sensorless, it's just when I try to start the board shakes like the motors want to go back and forth rather than just moving straight. If I give it a little push off then everything works fine. What is that about?
```

---
## \#32 Posted by: Deodand Posted at: 2019-05-02T02:45:23.278Z Reads: 77

```
That's pretty much how running sensorless works, it's the reason why most boards run sensors to avoid cogging. My guess is with some googling you could find a proper pinout for your hubs. I'd also re-run motor calibration as it looks really assymetric with the inductance measures is strange.
```

---
## \#33 Posted by: sameerpinheiro Posted at: 2019-05-17T03:31:05.678Z Reads: 67

```
Hey @barajabali, I am new to the forum, I live in Chicago and have a boosted v1 with red blinking lights. How can I get in touch for a repair/possible new battery? Tyvm!
```

---
## \#34 Posted by: huntercasillas Posted at: 2019-05-17T04:55:58.621Z Reads: 69

```
That’s not really something people here can fix. You’ll need to contact boosted. They charge $400 + shipping to replace V1 batteries.
```

---
## \#35 Posted by: sameerpinheiro Posted at: 2019-05-18T16:54:02.961Z Reads: 56

```
@huntercasillas, i thought building DIY batteries/setting BMIs to them was right around people here's alley! If my battery is unfixable, il need a DIY one. Not spending 750 + my old board for a refurbished one for sure!
```

---
## \#36 Posted by: sameerpinheiro Posted at: 2019-05-18T16:54:58.182Z Reads: 54

```
Problem is, im not good enough to mess with a BMI, much less making sure i dont build something that will potentially hurt me hahahahaha. Any suggestions?
```

---
## \#37 Posted by: huntercasillas Posted at: 2019-05-18T17:52:05.443Z Reads: 50

```
It is, but Boosted is very proprietary and doesn’t want anyone messing with their things - kind of like Apple.
```

---
## \#38 Posted by: sameerpinheiro Posted at: 2019-05-18T18:59:00.898Z Reads: 45

```
Well, they should have maintained V1 servicing then, hahahahahah, because im not getting rid kf a board because of a battery
```

---
## \#39 Posted by: huntercasillas Posted at: 2019-05-18T19:02:07.470Z Reads: 43

```
My V1 died and I turned it into a DIY build. Here’s the [link](https://www.electric-skateboard.builders/t/tesla-boosted-loaded-vanguard-10s4p-focbox-unity-dual-6354-black-caguamas-caliber-trucks-eboosted-enclosures/94187?u=huntercasillas&utm_source=share&utm_medium=ios_app)
```

---

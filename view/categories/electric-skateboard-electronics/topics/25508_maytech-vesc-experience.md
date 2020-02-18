# Maytech VESC experience

### Replies: 14 Views: 4653

## \#1 Posted by: Nexo Posted at: 2017-06-16T16:55:26.896Z Reads: 519

```
First of all, I want to send big HELLO to all Esk8 community. I am completely fresh user of this forum, but I was reading many of your articles before I started my DIY project of electric mountainboard and I found it really helpful.

Secondly, I am sorry if my english is not so good. But I will do my best to find correct words to express my ideas and thoughts clearly :slight_smile:


I have started thinking about this project last year. Reading hundreds of topics, looking for parts (some of them used) and making some drawings and calculations.
Finally I decided to start building. 

Board: Next Black Chili mountainboard. It was pretty cheap and in a really good condition.
Batteries: 3x4s Multistar 10.000mAh packs, 12s in total, 10C
Motors: 2x Maytech | MTO6374-190-HA, 190KV, 3550W, sensored, up to 12s
VESCs: 2x Maytech MTVESC50A
Drivetrain: gear ratio 6.13:1, 8 teeth motor sprocket, 49 teeth wheel sprocket, 05B-1 chain
Remote: Maytech remote and controller set
Voltage meter and anti spark switch for safety :slight_smile:

But let's get to the point. I have lost around 250-300$ for vescs already. One vesc came to me damaged, so I needed to send it back to get new one.
I thought that if I have sensored motors and vesc it will be a good idea to use it. But it wasn't. Both vescs are burnt now. Mosfets fried with a difference of only 2 days. I got information from Maytech that it was definitely my fault that it happened. First suspect was dust and dirt, but my vescs are closed in ABS enclosure that is almost completely sealed. I am furious about my vescs being useless now, but I need some guidance what have I done wrong?

I just want to mention, that board has never been used at full speed for long or even short period of time (it is way too scary) and both vescs were used with exactly the same settings and connected via can-bus.

Is 12s voltage really safe for vesc?
Does using sensored mode may lead to this situation?
Do you have any ideas about my "newbie mistakes"?

Please feel free to ask for anything :slight_smile:<img src="/uploads/db1493/original/3X/0/9/092753b4f72c5a38fcc9ad136749c9556cf6244b.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/6/2/628719540748b8c2019660cf46090db5f1f1b4aa.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/0/c/0cb0cdfe6327b2a3cb0bb3edb187981cb00df74e.jpg" width="281" height="500">
```

---
## \#2 Posted by: Challlsss Posted at: 2017-06-16T17:53:50.938Z Reads: 458

```
I personally don't have experience from Maytech VESC but while doing research on this forum was advised against it. The reasoning being that some people have a good experience with Maytech and others, (you) don't. If I had to guess I'd say it was the VESC not what you did. But I don't want to definitively say anything. Do you have VESC Settings screenshots handy?
```

---
## \#3 Posted by: Jaraya92881 Posted at: 2017-06-16T18:03:17.679Z Reads: 455

```
I have 4 maytech vesc, they all work in bldc no issues. The only issue is FOC which hasn't been working for me with their hubs but not a big deal for me. So.... you'd have to share your VESC configuration for others to help on what possible blew out your vesc. :)   My blew out a DRV because of FOC but i knew what i did wrong so no longer is this an issue for me.  

Also i'd recommend to order through Maytech reseller not alibaba so you get a better warranty, the alibaba direct may not always give you best warranty support.
```

---
## \#4 Posted by: Nexo Posted at: 2017-06-16T18:10:48.801Z Reads: 430

```
unfortunaltely, I don't have any screennshots saved, but I am pretty sure that if you will ask me for any parameters I will remember them because I wasn't changing much :slight_smile: ...i hope so
```

---
## \#5 Posted by: Challlsss Posted at: 2017-06-16T20:09:30.185Z Reads: 412

```
I'd want to know max current, and voltage settings and if they were foc or bdlc
```

---
## \#6 Posted by: psychotiller Posted at: 2017-06-16T20:24:33.578Z Reads: 397

```
I have used almost everyone's vescs. And I've blown DRVs and mosfets from every single vendor.  Every time I've been able to get a replacement. I'm also a reseller now and sell maytech vesc's on my site. 

I have blown drv's on 2 of mine. I ended up sending them to @JohnnyMeduse and he fixed them for $45. He also made them foc worthy!.

For the record, I have had mixed results with foc and maytech. Some have worked and some didn't so I ran sensored bldc instead. Still a viable controller. 

If you're dead set on running 12s invest in Ollin Controllers. 

With maytech, I recommend 8s to 10s.
```

---
## \#7 Posted by: Jaraya92881 Posted at: 2017-06-16T20:43:29.621Z Reads: 380

```
Thanks for the input mr. Tiller :)
```

---
## \#8 Posted by: Nexo Posted at: 2017-06-16T20:56:45.910Z Reads: 371

```
as far as I remember it was:

motor max: 60A
motor min (regen): -60A
battery max: 50A
battery min: -25A
absolute max: 130A

minimum input voltage: 8V
maximum input voltage: 50,4V
cutoff start: 42V
cutoff end: 39,6V

BLDC
```

---
## \#9 Posted by: Martinsp Posted at: 2017-06-16T21:10:14.758Z Reads: 357

```
Yup... Maytech VESCs suck... My first one failed most probably because they dont trim the legs of JST hall connector and these pierced through the positive lead of my battery... So i sent it back (their customer service as far as my experience goes was very good). So they sent me back a new one... I took it out of that plastic it was in and trimmed the leads, second was to check all connections and if there are any solder balls present that could short out (solder balls are pretty much just loose pieces of solder) and lastly upload firmware that i know is original and not "messed with" by Maytech. The vesc worked in FOC mode perfectly without halls (i didnt try them because i only put halls in one of my motors yet) but after around a month the VESC from Maytech broke for no apparent reason... The settings were 100% the same as on my other VESC that I build (meaning i had all good quality and genuine parts) and that VESC works well so far no issues in any mode. So there is probably something that they changed either some parts are low quality to keep the cost down or maybe it is that they use the same values of parts but different in such a way that is cheaper for them... 

Bottom line is that it is a chinese VESC... not that it would be bat taht it is manufactured in china but it is suspiciously cheap... i mean cmon they sell them on aliexpress it cant be as good as 200USD VESC :D 

Id never buy it again trust me.. the 90 USD or whatever is not worth the hustle and frustration and even worse such as fail in high speed... 
The VESC is one of the most important parts of an electric longboard it is not wise and responsible to try to get it as cheaply as possible...
```

---
## \#10 Posted by: Nexo Posted at: 2017-06-19T13:38:01.087Z Reads: 317

```
I decided to give you some more photos of my case. On both of my vescs I can see mosfets are burnt. But something that bothers me more is a quality of soldering on them...but, I think that "fighting" with Maytech is pointless anyway
I will be very glad if you will give any advices about that

I was informed once again by Maytech that this situation was completely my fault but I need some guidance. According to that please let me know about any of your ideas dear Esk8 community! :slight_smile:

One more thing, I was asked about basic parameters of my vesc, and I sent that my maximum input voltage was changed to 50,4V (4,2Vx12) but this value was not reached anyway, but in case IF IT WILL BE then it should affect braking with fully charged battery only, right?
<img src="/uploads/db1493/original/3X/9/5/95a1fa19aca9a2eabaabbd28a7945871e494f05a.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/0/9/092658d3ec692c85e5716a4c99e425b19eba0e5e.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/2/3/23040363dd48034f63ed37c80de08cae82df7bf1.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/d/e/de006a30e3df971451c509c92b0a1e9c37f8b4da.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/7/3/7394e8b510ed46872d9a2ad1de6c164cb0113f46.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/e/4eb5c68de0c5bd37aef9242bcb5e5a787c419f63.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/e/b/ebd4d38201b24cccf81a88800c2b29697a368fa5.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/f/6/f6046264e4c048b58538b63a4cc518440ed4a065.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/a/a/aa2fc0d5709f2d51bd5007bc78ac3797f8a24ad2.jpg" width="281" height="500">
```

---
## \#11 Posted by: Martinsp Posted at: 2017-06-25T20:13:10.914Z Reads: 284

```
Hey!
Sorry, i missed your post, just seen it.
First thing I would do is take that heat shrink off of the VESC because on the pictures it is hard to tell what is dirty and what is burnt. The shunt looks like it got pretty damn hot but that should not matter so much, measure its resistance and if it is the same as the other one (you most probably dont have accurate enough meter to measure 5mOhms precisely so measuring both and comparing is better). Also the mosfet you circled on one of the photos got hot too... measure it if its shorted... the one will most robably have to be replaced. Also dont forget to measure the gate resistors (can be found in schematic on github) because those usually blow with the mosfets.
```

---
## \#12 Posted by: Nexo Posted at: 2017-07-09T18:43:47.765Z Reads: 268

```
ok guys,

my conclusion from that situation is that I need to avoid Maytech VESCs at all costs

I did some research about ESCs and VESCs, and here is what I think:

1) I am not very interested in regenerative braking, because in my opinion it is more like "marketing thing", but maybe I am wrong :wink:
2) I would like to stick to my 12s setup instead of 8s, my motors are ready to be used with 12s lipo and it is really cool to use their full power :slight_smile: 
3) I am not really into any sensored mode and foc stuff. As far as I know, it may only cause problems in my case, and NO ISSUES is my number one priority
4) I would like to pay some more money for controller that will work good for a long time, instead of changing crappy VESCs all the time, but on the other hand, price for 2 VESCs 6.4 is kind of scarry :stuck_out_tongue:

...it is really hard to look at my board being useless, but I need to make a choice about the speed controller

once again I would like to mention that my setup is:
12s lipo with 190KV motors, so ERPM is somewhere around 59.000 already...maybe that is my problem?

thank you for any ideas :slight_smile:
```

---
## \#13 Posted by: meesie Posted at: 2017-10-24T14:29:52.924Z Reads: 222

```
59.000 is indeed dangerously close to the maximum of 60.000.

i don't have a lot of knowledge about this topic but i believe you can limit the max ERPM in the bldc tool.
can anyone with more VESC-knowledg confirm?
```

---
## \#14 Posted by: Martinsp Posted at: 2017-10-24T17:27:03.417Z Reads: 220

```
I use 245kv on 10S setup which is over 60k (72k if I remember correctly). The way to avoid blowing your VESC is to disable the "limit ERPMwith negative torque" in the motor config tab (keep limits here at + and - 60k) and then limit your ERPM in the "soft RPM limit" in the PPM tab. I have it set to start at 52kand end at 55k. This worked out perfectly for me using @Ackmaniac`s firmware in watt mode. I can spin the motor at full throttle/max rpm with no load without going over the set 55k.
```

---

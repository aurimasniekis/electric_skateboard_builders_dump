# XT60 connections or Solder?

### Replies: 11 Views: 240

## \#1 Posted by: Rinze Posted at: 2019-12-29T11:13:11.845Z Reads: 67

```
Hi all,

I have a question for my new build.
I know soldering the cables is better, but I like to use XT60 connections.
I think this is easy plug and play, and if something would be broken or want/need to be replaced, it would be easy if there would be XT60 connectors.
But on the otherside I don't know if this is a good idea because of the high voltage.

I want to use Samsing 30Q batterys (12S8P) so this would be 120A & 44,4v (max 200A & 50,4v)

* **ESC:**  Dual FSESC6.6 200A @flipskytech01
* **Motors:**  2 x 6384 190 KV Motors @flipskytech01
* **Anti spark:**  Anti spark Switch Smart Enhanced 200A @flipskytech01
* **Battery:**  12S8P Samsung 30q
* **BMS:**  FPM (FPML12S150F873)

See below the connections:
![Connections|257x500](upload://vFSVxXfaC1pILaiv06nNg3RJZea.jpeg)

Thanks in advance :slight_smile:
```

---
## \#2 Posted by: Chaki Posted at: 2019-12-29T13:13:07.723Z Reads: 63

```
I have both XT90 and XT60 connector in my boards. XT everything. It's wort it if something is wrong just unplug and fix no need to cut and resolder. If u are worried just use the the bigger XT90. But personally IAM totally fine with XT60s they can Handel 60A. There are worst bottlenecks than Xt60. 

Like u can see I have more XT connectors then I wrote "XT" in this post. 

All in all u be fine.
```

---
## \#3 Posted by: Rinze Posted at: 2019-12-29T13:37:09.224Z Reads: 60

```
Hi Chaki,

Thanks for the help. This is good info for me.
XT90 would be indeed maybe a good idea :slight_smile:
This because i want to use is a Flipsky 6384 190kv 4000w (2x) and on there website they say "Max Current: 95 Amps" per motor AND a Big Size Dual FSESC6.6 for 200A.

Maybe it is overkill to use XT90, but since I have no experience with this, this would be (for my feeling) the save choice.
```

---
## \#4 Posted by: mynamesmatt Posted at: 2019-12-29T13:46:03.515Z Reads: 55

```
[quote="Rinze, post:1, topic:104972"]
But on the otherside I don’t know if this is a good idea because of the high voltage
[/quote]
The voltage has nothing to do with it. it's the current.
Your battery has a peak output of 160a and continuous output of 120a. You will rarely pull 120a for more than 5 seconds. same with your motors, except the current is split across 3 cables instead of 2.
Also, your fsesc will not pull 200a from your battery. Even the trampa vesc can only pull 80a from the battery on one side. So even if you pull 160a I'll be impressed that it doesnt melt. I would however recommend the xt90 connector. it's tough as nails and you'll never worry about it. Also you can use the xt90S connector so that you get anti spark in case your anti spark button shits itself. Please do some more reading before you dive into this as something like this can hurt you. Also head onto esk8 news. alot better than here lol
```

---
## \#5 Posted by: Rinze Posted at: 2019-12-29T14:27:37.358Z Reads: 53

```
Thanks for the advice.
The extra anti sprak is also a good idea :slight_smile:

Updated my connection overview:
![Connections|290x500](upload://XD4xeS3v9eN7tYemOnhhIDQsES.jpeg)
```

---
## \#6 Posted by: PixelatedPolyeurthan Posted at: 2019-12-29T15:00:09.896Z Reads: 47

```
[quote="mynamesmatt, post:4, topic:104972"]
Please do some more reading
[/quote]

yeah please do.
i don't think the volt meter will work like that? and it is pretty stupid, just solder is on or buy a [DAvEga](https://forum./t/davega-x-accepting-orders/7935) 

Flipsky anitspark is shit. all antisparks fail in the end. Just use an [XT90S loopkey](https://forum./t/how-to-make-an-xt90s-loopkey-sro/2325)

flipsky esc is pretty bad too. get a Focbox Unity  or trampa vesc or even the new [NEOBox from Jeff Wu.](https://forum./t/neobox-open-source-focbox-variant-hw-6-design/12426)

Also go join the other forum, this one is shit.
```

---
## \#7 Posted by: mynamesmatt Posted at: 2019-12-29T17:19:27.486Z Reads: 44

```
[quote="PixelatedPolyeurthan, post:6, topic:104972"]
i don’t think the volt meter will work like that?
[/quote]

nah it will work like that. it's in parallel with the output of the switch so it's fine 😊
```

---
## \#8 Posted by: Anubis Posted at: 2019-12-29T20:18:18.221Z Reads: 42

```
I personally wouldn't use an XT90 splitter like that. I have accessories that use the output, the cables for them are thin AF. A tiny ass cable is fine transmitting 50V as long as its at low amperage. 

I think you're better off having a 4 5.5mm or larger bullet connections on the positive line, then soldering the smaller wires onto the bullet edge (So there is basically a bullet connector extension, but on the extension you add your accessories) 
Unless you require a negative lead too... I think some of them do.
```

---
## \#9 Posted by: Rinze Posted at: 2019-12-29T21:02:21.811Z Reads: 39

```
[quote="PixelatedPolyeurthan, post:6, topic:104972"]
flipsky esc is pretty bad too
[/quote]

Thanks for the heads up

[quote="Anubis, post:8, topic:104972"]
I think you’re better off having a 4 5.5mm or larger bullet connections on the positive line, then soldering the smaller wires onto the bullet edge (So there is basically a bullet connector extension, but on the extension you add your accessories) Unless you require a negative lead too… I think some of them do.
[/quote]

all accessories also need the negative output, so then I need 2 bullet connectors. so I would have the same as the XT90 connectors I think.
I will use the 5.5mm bullet connectors for the motor to the FSESC, but I'm not 100% sure yet. this because I also use a enclosure from Eboosted under the deck.
I still have to look at this as soon as I start putting everything together.
```

---
## \#10 Posted by: flipskytech01 Posted at: 2020-01-06T08:16:39.503Z Reads: 19

```
Hello. Sorry for the late reply. Please connect the BMS with the battery and then connect it with the anti-spark switch (please pay attention to the input and output side), do not parrallel. Yeah. XT90 connector can hold higher current than XT60. If you need any more support, you can e-mail me directly flipskytech01@outlook.com or to our service e-mail: flipsky-service@outlook.com. I will reply you in time. Thanks.![vesc%20connection|353x500](upload://8rLPFRnkULRqwRo1LQHmBcswAaH.jpeg)
```

---
## \#11 Posted by: Rinze Posted at: 2020-01-06T15:29:09.377Z Reads: 15

```
[quote="flipskytech01, post:10, topic:104972"]
Please connect the BMS with the battery and then connect it with the anti-spark switch
[/quote]

Thanks for the tip, but I have a BMS bypass for safety reasons. Or is there a different reason?
The parallel connector is for the easy plug and play of the components.
should not cause a problem in theory, but maybe I overlook something.
Please let me know.
[quote="flipskytech01, post:10, topic:104972"]
please pay attention to the input and output side
[/quote]
Thanks I will pay attantion on this
```

---

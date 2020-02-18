# Smokey The VESC &ndash; Unsure cause

### Replies: 35 Views: 440

## \#1 Posted by: Lanik Posted at: 2018-08-30T18:34:40.958Z Reads: 164

```
I'm working on my first build:
Battery: 10S4P Lith-Ion
BMS: BesTech HCX-D223V1
Dual VESC: Torque ESC x2
Dual Motors: KEDA 6364 x2

I wanted to set up my ESC which seems to require the battery to be plugged in to do so because nothing lights up when using the micro usb. 

When I plugged my battery into a singular ESC, w/o the BMS or Motor, the positive terminal melted and started smoking. The rest of the ESC looks fine and w/o any burn marks, just the positive terminal on both my battery and ESC need to be replaced. 

Can anyone let me know what caused this? I don't really want to repeat it.

ESC:
![esc|281x500](upload://ny0ck0uRaqyKIwdJlCBVwjJik4w.jpg)

ESC Terminal:
![esc%20terminal|512x288](upload://pIasp3hf1Z5evBwwOVPbF5vvSZj.jpg)

Battery Terminal:
![battery%20terminal|512x288](upload://xOaFLny5CyGXiFTJTQuPSvLK2fq.jpg)
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-08-30T18:42:25.289Z Reads: 151

```
upclose pictures of the (vesc)board itsself?
```

---
## \#3 Posted by: NickTheDude Posted at: 2018-08-30T18:43:04.256Z Reads: 153

```
Perhapse the xt90 was soldered to the wrong wires? like + to - and - to +. I've done that before and it sparked a lot and blew my VESC... :sweat_smile:
```

---
## \#4 Posted by: longhairedboy Posted at: 2018-08-30T18:43:09.199Z Reads: 149

```
my first thought was reversed polarity but the connectors look good. yeah, like @Sn4pz said get some pics of the PCB
```

---
## \#5 Posted by: longhairedboy Posted at: 2018-08-30T18:44:53.320Z Reads: 144

```
one immediate thought for possibilities was that 1) the male connector prong was maybe pinched and/or had some kind of shipping oil or ooze on it or 2) there was something like that in the female socket and all of that lit up when it both made a bad connection and was interfered with by mystery material

that positive prong and socket both look slagged up now though, so hard to say
```

---
## \#6 Posted by: Lanik Posted at: 2018-08-30T18:47:40.786Z Reads: 139

```
Pictures of the board itself. I don't really want to remove the heat shrink, sorry.
![859065132884541390|281x500](upload://qdv0Lf8eDu97aHx52GXYhyDMWMM.jpg)
![8375025877482848890|281x500](upload://wkrXKWdjBgfBRkiYlx12qrVwqo1.jpg)
```

---
## \#7 Posted by: longhairedboy Posted at: 2018-08-30T18:48:38.954Z Reads: 129

```
polarity looks good on the board. Check to see if anything is shorting the big caps in any way, maybe a hair of a wire or something
```

---
## \#8 Posted by: Lanik Posted at: 2018-08-30T18:56:53.161Z Reads: 129

```
Everything looks good at the Caps. If there was a hair of wire, that should have burned up before the terminal or at least caused some smoke, but everything came from the terminal.
```

---
## \#9 Posted by: Sn4pz Posted at: 2018-08-30T19:05:39.455Z Reads: 122

```
i dont see anything wrong either.... but ive never seen that blonde part of the board looks different from what ive seen, im going to look at the saved pictures of my old torque vescs i have so i can compare... maybe your board is literally missing something?
```

---
## \#10 Posted by: Lanik Posted at: 2018-08-30T19:06:25.275Z Reads: 120

```
Do battery connections need to be made instantaneously via a switch? I haven't had a problem like this before with my past RC projects, but nothing has had this kind voltage or current numbers.
```

---
## \#11 Posted by: Sn4pz Posted at: 2018-08-30T19:09:04.717Z Reads: 117

```
no you can just plug and unplug a vesc normally from the battery pack, it will spark (hense antispark,) but nothing bad with happen. Maybe something is wrong with the battery?
```

---
## \#12 Posted by: Lanik Posted at: 2018-08-30T19:15:37.507Z Reads: 116

```
Just looking at the board the only thing I might be missing is a resistor that is most likely for the micro usb.

![2560202343075302822|443x288](upload://k9OR8GvZ2oE4cFvACnecRHdspK1.jpg)

I don't know if it is intentional, but I doubt it would cause my problem.
```

---
## \#13 Posted by: longhairedboy Posted at: 2018-08-30T19:19:00.168Z Reads: 115

```
you know what... i thikn you're just experiencing connection pop because you don't have an antispark and you're just jamming a couple of XT60s together. 

even without something in the socket or bent prongs to exacerbate it, its still going to pop and spark and light up and probably blacken the connector.
```

---
## \#14 Posted by: Lanik Posted at: 2018-08-30T19:22:03.515Z Reads: 108

```
I think you might be right. I'll get an antispark I haven't even looked into that. And now I'm out of XT90 connectors as well. So I'll be playing the ol' waiting game again.
```

---
## \#15 Posted by: Sn4pz Posted at: 2018-08-30T19:24:59.938Z Reads: 103

```
ah duh i overlooked that :thinking:

but wouldnt(shouldnt***) the pack come with a xt90? unless you made it yourself @Lanik
```

---
## \#16 Posted by: Lanik Posted at: 2018-08-30T19:26:33.764Z Reads: 102

```
It probably would, looking into an antispark now. I will need to replace those connectors that melted though. And I'm all out now.
```

---
## \#17 Posted by: RedEagle Posted at: 2018-08-30T19:30:09.683Z Reads: 99

```
i've got some connectors lying around but they are xt90.
```

---
## \#18 Posted by: taz Posted at: 2018-08-30T19:34:08.673Z Reads: 101

```
+1

This is one of the reasons I do not like XT connectors.
I have been using EC5 connectors on my 12S helis and never experienced something like that since both the male and female sides of the connectors are isolated.

![EFLAEC503_a0|690x383](upload://yKcLCr75pcLUHRm7T7PisKMQTuo.jpg)
```

---
## \#19 Posted by: b264 Posted at: 2018-08-30T19:41:51.448Z Reads: 101

```
XT90 ≠ XT90AS

Try an XT90AS or XT90 antispark as used in loopkeys.  Or, just use a loopkey made from an XT90AS.  Or use an antispark switch.

It's possible the melting happened because the empty capacitors on the VESC board were an effective short circuit for a very brief moment while they are charging-up.  You have to connect it *gently* (from an electrical perspective, not a physical perspective)
```

---
## \#20 Posted by: longhairedboy Posted at: 2018-08-30T19:44:11.311Z Reads: 98

```
The arcing that happens on connection... the spark.. isn't because of a lack of isolation. Its not caused by shorting. It happens as a result of the gap closing as the connector properly makes its connection. The potential is such that it arcs prior to making total contact.
```

---
## \#21 Posted by: taz Posted at: 2018-08-30T19:49:57.149Z Reads: 90

```
I know all that. The difference is that the spark is contained between the female and male sides of the connector but always on the same polarity.
On an XT the arc can also jump to the other polarity connector on the male side.
It does not cause any major problems but it can wear down the connectors a lot faster.
```

---
## \#22 Posted by: TowerCrisis Posted at: 2018-08-30T19:50:08.539Z Reads: 94

```
I'd be more suspicious about this rather than attribute it solely to a capacitor charging spark.

I had something very similar happen to an old vesc. Plugged it into a 6S battery once after a long time, big spark, I left it plugged in, and the thin alligator clips I used to connect it started smoking.

I hooked it up to a bench power supply and slowly turned the voltage up. It drew ~3 or 4 amps continuously at 5V. That was not the capacitors charging, something had been shorted.


@Lanik If you have a power supply I suggest hooking it up to that and seeing what kind of power it's drawing before you continue. Use low voltage and just read current. There's no use in frying more connectors (or even possibly an antispark switch) if the vesc is toast.

Idling a vesc shouldn't draw very much power once the caps are charged.
```

---
## \#23 Posted by: b264 Posted at: 2018-08-30T19:55:22.408Z Reads: 90

```
:arrow_up:

[quote="TowerCrisis, post:22, topic:66572"]
Idling a vesc shouldn’t draw very much power once the caps are charged.
[/quote]

Yes; the charging should happen in less than 1 second.  After that, you should have <100mA draw
```

---
## \#24 Posted by: TowerCrisis Posted at: 2018-08-30T19:58:12.424Z Reads: 85

```
Actually further inspecting the connector, those positive leads are seriously melted. You don't vaporize significant amounts of metal like that from charging up some measley caps.

The tip of the female positive is literally shorter now, this thing had to have pulled significant amps for a substantial amount of time.
```

---
## \#25 Posted by: dareno Posted at: 2018-08-31T02:50:24.273Z Reads: 75

```
That is a strange one even for me who has made every mistake imaginable.  It doesn’t look like a polarity issue as when I did it my VESC literally went snap crackle and pop and looked cooked as but it might pay to check the battery for a cross connection. Who built it?   
  It does look more like a short damage wise.  I did similar connector damage with my multi meter after my ten year old had been playing with the test leads.  Plugging them in different holes etc.  best way forward is to use a power supply and try to isolate the issue.  Check every connection as I’ve never had a connection spark do that much carnage.  Maybe a bit of wayward solder on the VESC xt?
```

---
## \#26 Posted by: Andy87 Posted at: 2018-08-31T04:47:25.005Z Reads: 72

```
Don’t think that it was a battery short, but just to be sure...did you check the polarity on your battery.
Yes we have seen the red and black wires right on the xt90, but we didn’t see the battery side.
If there + and - changed it non the less will short.
```

---
## \#27 Posted by: Lanik Posted at: 2018-08-31T05:08:07.231Z Reads: 74

```
Yup I double checked before I charged the battery. If it was wrong I'm guessing I would have found that out then.
```

---
## \#28 Posted by: Lanik Posted at: 2018-08-31T05:24:06.757Z Reads: 76

```
Bah. I went to check it again just to get it out of my head. Turns out my red and black leads on my multimeter got switched on me. That's what I get to lending it out and not paying attention. 

That would explain everything. The charger didn't fry it because I read the + and - with my compromised meter on the charger's output and matched it with my battery which I also got the + and - ends with my compromised meter.

I feel like a complete idiot.
```

---
## \#29 Posted by: taz Posted at: 2018-08-31T06:29:00.741Z Reads: 67

```
[quote="Lanik, post:28, topic:66572"]
That would explain everything.
[/quote]

No it does not.
If I understand correctly you are saying that the polarity on the battery side was reversed. 
When you connect the battery to the esc with the wrong polarity, you fry the esc not the connector.
I have seen my fair share of reverse polarity fried escs since I raced 1/10 electric touring cars and we used bullet connectors to save weight.
I will let you guess how many times I have seen this happen :stuck_out_tongue_winking_eye:

![20180831_092257|374x500](upload://3HNl7ImtvZlhTQtgn2JlWrlPAnS.jpg)
```

---
## \#30 Posted by: PatRocks Posted at: 2018-08-31T19:53:28.621Z Reads: 53

```
Lol I almost fried a focbox with reverse polarity! I use as150 connectors, and I heard the AS resistor burn up before the esc died, and that saved it!! Super lucky, I've since changed my connectors to idiot "resistant" the process
```

---
## \#31 Posted by: GrecoMan Posted at: 2018-08-31T20:12:29.018Z Reads: 53

```
i did exactly what he did (literally exactly the same thing with the meter wires swapped and everything) on my first tb vesc and it still worked fine after. i left it plugged for 2-3 seconds and burned the fuck outta my hands unplugging it
```

---
## \#32 Posted by: taz Posted at: 2018-08-31T21:16:05.268Z Reads: 51

```
I fail to see how the electronics on an esc can withstand more current than a properly sized connector when fed with the wrong polarity current.
That said I have been wrong before 😎
```

---
## \#33 Posted by: Spatt Posted at: 2018-08-31T22:05:45.142Z Reads: 49

```
Cool xray t3, I runned with xray nt1, these kind of beasts really make you understand basics of mechanics and electronics ![IMG_5098|375x500](upload://sN7fEu07CIjyDPCU36qGzYPpz83.JPG)
```

---
## \#34 Posted by: Lanik Posted at: 2018-09-08T19:24:38.113Z Reads: 34

```
Got new connectors and everything looks to be working fine.
```

---
## \#35 Posted by: Nordle Posted at: 2018-09-09T04:24:07.748Z Reads: 26

```
happened to me too, the connecter pushed itself apart in a big cloud of smoke. i assume it burn’t so fast that nothing got damaged on the vesc.
🍀 prob. just luck^^
```

---

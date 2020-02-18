# Think I just killed my Focbox 1.6 in less than 24 hours of owning it lol

### Replies: 66 Views: 832

## \#1 Posted by: legend27 Posted at: 2019-05-11T16:22:00.915Z Reads: 237

```
**TL;DR: Read from "The acutal issue"**

Hey everyone!

So yesterday I got a package. It was my brand new (used before, but brand new for me) **FocBox 1.6**.

I soldered new wires, bullet connectors and XT-90 and everything was working like it should. I did the setup with the following settings:
- Motor max: 70A
- Motor min: -60A
- Battery max: 45A
- Battery min: -15A

Today I went on the first test ride. Pumped up and ready to shred. Everything went fine the first kilometers. Temperature was maybe a bit high (60C at max). Then I came to this long long long road where I went nuts. Full throttle most of the time, 45 km/h most of the time and temperature eventually got higher. Temperature reached 70C (probably 80C but I had put my phone down in my pocket so I wouldn't crash doing 45 km/h.)

So I eventually reached a light signal and had to brake. I braked pretty hard and at some point I noticed I had lost my brakes completely (unfortunately at low speed...). I went on to the side walk to test my accelerator and nothing happend...

I had no choice. The time was now. I was the chosen one. It was time for

AN ANTI-PUSHER TO BECOME A PUSHER. THE WALK (ACTUALLY PUSH) OF SHAME
-

I eventually made it home after 5 km of hard pushing without dying or killing my board even more (accidentally pushed my board out in the middle of the road (no cars, unfortunately)).

Time had come, now I had to open my enclosure and focbox. This video speaks for it self...

https://www.youtube.com/watch?v=TrTvp9z_fM0

As the video showed, no damage on the pcb.

![image|666x500](upload://5jSDuKmoBxhuKQmdcc0jMbRijFc.jpeg) ![image|666x500](upload://zsQpBzTy7uH8WdXmOCjO6WNGmfJ.jpeg) 

Now to the actual issue:
-
- My FocBox doesn't turn on (No lights or anything)
- My PC doesn't recognize my FocBox when I plug it with USB in and give it power.
- I can read 39V power when measuring Focbox negative on PCB and battery positive.
- I can read 5V from the UART port when the focbox is getting power.
- Since I can't turn on my FocBox, I can't check the terminal for any error codes...

Setup:
- Single motor
- No can-bus used.

I would appreciate if someone had any suggestions on what happend. Like usual, any input is appreciated. Also the bad ones :kissing_heart:
```

---
## \#2 Posted by: rusins Posted at: 2019-05-11T16:32:49.832Z Reads: 219

```
Really strange. Have you tried charging your battery up? Hopefully the VESC is just set to turn off under a specific voltage, and you just ran your battery dry.
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-05-11T16:45:00.767Z Reads: 211

```
[quote="rusins, post:2, topic:93487"]
Hopefully the VESC is just set to turn off under a specific voltage, and you just ran your battery dry.
[/quote]

pretty sure he reconfigured it....
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-05-11T16:45:39.159Z Reads: 209

```
@JohnnyMeduse
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2019-05-11T16:47:31.895Z Reads: 208

```
[quote="legend27, post:1, topic:93487"]
My FocBox doesn’t turn on (No lights or anything)
[/quote]

sound like the 3,3V is dead... did you plug it can bus ? Or else it is probably a blown mcu.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-05-11T16:49:24.943Z Reads: 198

```
@Sn4pz guess what :rofl:
```

---
## \#7 Posted by: Creavenger Posted at: 2019-05-11T16:56:44.002Z Reads: 191

```
Another one bites the dust 🤔 good job on pushing 5km tho I feel ya xD
```

---
## \#8 Posted by: seaborder Posted at: 2019-05-11T16:59:07.199Z Reads: 187

```
Often you dont see a damage when its under or inside some of the chips. 
The gate resistor looks burned a bit but maybe its just the picture, I think your focbox was running at the limits and maybe sth wasnt configured right. With the hard brake it was just to much for some components, I would assume.

With my stuff, I always leave a certain buffer for safety. So I know even if something goes wrong, the components still have little room.

Was this in a single or dual config?
Does it still turn on?

EDIT: didnt see the text with the acutal issues under the pictures sorry

Greets!
```

---
## \#9 Posted by: legend27 Posted at: 2019-05-11T17:04:22.580Z Reads: 182

```
@rusins
I configured the Focbox voltage cut-off start to 34.5V and end to 33.5V. Battery is at 38.xV

@JohnnyMeduse
Can-bus was not connected. Only had UART + sensor + receiver connected. Could be the MCU.@AlanZhou also mentioned that. Would you be able to point out where the MCU is located? Also where is 3,3V? 

@seaborder
Think I pushed it to the limit :stuck_out_tongue: Could you please point out the gate resistor?
It was in a single setup. It doesn't turn on. No lights or sounds or anything. And power goes through my anti-spark so not because of that.

Thanks a lot for all of the inputs, guys! Really appreciate it!
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2019-05-11T17:06:08.088Z Reads: 182

```
Check if C25 is shorted. The Mcu is the big square chip on the same side as the DRV

![image|666x500](upload://vZvlNzxYO4lLGwzoSXYTJVHdeHL.jpeg)
```

---
## \#11 Posted by: seaborder Posted at: 2019-05-11T17:06:15.983Z Reads: 180

```
![easedfr|664x500](upload://fn5y5HQ3P4YwWrotf8OWnsD3OBK.png) 

This is the one. But Iam learning all that right now so not 100% sure.

Can you maybe make a closer picture of the part I marked?:)
```

---
## \#12 Posted by: seaborder Posted at: 2019-05-11T17:07:12.833Z Reads: 171

```
Okay Johnny knows much more about that, I think he can help you out more :)
```

---
## \#13 Posted by: Fatglottis Posted at: 2019-05-11T17:08:33.811Z Reads: 173

```
3,3V. Measure it! :slight_smile: 
![bild|441x405](upload://4D5PVcKTlm1zSi2TCor7cz46WzX.jpeg)
```

---
## \#14 Posted by: legend27 Posted at: 2019-05-11T17:25:00.496Z Reads: 171

```
Don't do like me guys. Just made my focbox get a little bit hot and think a saw very little smoke. All good (from my noob perspective)

Anyway. Got it measured. Don't measure the actual pins like an idiot (me) but connect a jst connector with some wires.

![image|666x500](upload://As15ShGypG0fjmtuGNGqD7PItvG.jpeg) 

@Fatglottis 
**The voltage for 3,3V is 150 mV. That's not normal, right?**

@seaborder
Here is the picture anyway.
![image|666x500](upload://o9mD3wfWBZprZe4GiG9Gof06Bub.jpeg) ![image|666x500](upload://pTECWfOuh07kGuGhFHG8h19zRYW.jpeg) 

@JohnnyMeduse
Doesn't look like it's shorted. Answer above is probably more helpful.
![image|666x500](upload://pSI8znoHK7FJY8RWOiRkh1EsVW1.jpeg) ![image|666x500](upload://wqZNOKL7F568W0AZwE44C8cTyPO.jpeg)
```

---
## \#15 Posted by: Fatglottis Posted at: 2019-05-11T17:35:42.209Z Reads: 163

```
You should have 3,3V, not 150mV. 
Could be this regulator..  Or the MCU is blown and it is now shorting the 3,3v rail somehow.

Is the MCU getting hot?

Btw this is a trick if you want to measure tiny stuff. Of course it’s safer the way you did it with wires 👌🏻
![image|375x500](upload://2zCliCgXkbinaPcDT9H1Kriadgv.jpeg)
```

---
## \#16 Posted by: legend27 Posted at: 2019-05-11T17:40:58.399Z Reads: 159

```
Just shocked myself lol. stupid.

The orange circled one is not getting hot.

The red circled one is a bit hotter than all the other parts. Not like untouchable but just noticeable.

![focbox|670x500](upload://sNeMmWEiUFGIiam9lVj7uQ5EVq1.jpeg)
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2019-05-11T17:43:04.512Z Reads: 154

```
If you don't have 3.3V on the 3.3V that not good. 

Using diode check on your multimeter check if the 3.3v is shorted to the gnd. If so it is most likely internal damage from the MCU
```

---
## \#18 Posted by: legend27 Posted at: 2019-05-11T17:46:43.212Z Reads: 153

```
wait what?

Diode?

Im sorry, but this is not my special. Can you please elaborate?
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2019-05-11T17:47:42.342Z Reads: 154

```
https://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse

That a similar procedure to check the 3.3V, but since you didn't use Can, the can chip is probably not defective
```

---
## \#20 Posted by: Fatglottis Posted at: 2019-05-11T17:53:04.774Z Reads: 151

```
Do as @JohnnyMeduse has explained above but on these pins. (FOCbox Powered off)
![bild|353x243](upload://9aJRZ2uQ9dnnws6xwrTjT1IRPgY.jpeg) 

Regarding if the MCU (STM32) got hot or not..
 Its the big chip to the right.
```

---
## \#21 Posted by: legend27 Posted at: 2019-05-11T17:55:10.827Z Reads: 149

```
Think I did it correct.

I got a beep when doing like this:


![|666x500](https://www.electric-skateboard.builders/uploads/db1493/optimized/2X/a/aad1723f09da6b393a64bd1c4b649897cb89e710_2_666x500.jpg)

Also got a beep when putting one probe on the C25 and the other on the Focbox battery negative line (shown in pictures below. Don't mind different colors.)

http://prntscr.com/nna5fs

http://prntscr.com/nna59r
```

---
## \#22 Posted by: legend27 Posted at: 2019-05-11T17:58:29.876Z Reads: 147

```
I got a beep when touching those two circled ones

http://prntscr.com/nna6pq

Thanks for clearing which one is the MCU. I thought it was the yellow one the whole time :stuck_out_tongue: It didn't get hot.
```

---
## \#23 Posted by: Fatglottis Posted at: 2019-05-11T18:10:38.014Z Reads: 142

```
3.3V is shorted to ground by either the 3v regulator or C25. Since they both are both connected to 3,3V and ground, its hard to say who is bad here. But since the MCU is not warm.. I believe its not broken.
You should remove one component at a time. 
Start with the C25. Beep 3v3 to GND. If it still beeps, remove the 3v regulator.
```

---
## \#24 Posted by: legend27 Posted at: 2019-05-11T18:13:18.952Z Reads: 142

```
What excatly do you mean by "remove"? Like un-solder and remove it?
```

---
## \#25 Posted by: Fatglottis Posted at: 2019-05-11T18:15:54.347Z Reads: 139

```
yes :wink:..  first SMD thingy I soldered was a DRV.  Get the tools.. its not that hard if you do it right. Also you will be able to fix other things later :)
```

---
## \#27 Posted by: KaramQ Posted at: 2019-05-11T18:18:44.527Z Reads: 137

```
I literally have the same problem with a focbox I have
```

---
## \#28 Posted by: legend27 Posted at: 2019-05-11T18:20:52.607Z Reads: 139

```
Oh okay. No way around it? Can’t use something like this instead?

![image|666x500](upload://oNsSQuDt5DdUGBuY0in8bE1hJN5.jpeg) ![image|666x500](upload://8CGPyAoVwpTPIynDe4JxqszBmgd.jpeg)
```

---
## \#29 Posted by: Fatglottis Posted at: 2019-05-11T18:28:32.708Z Reads: 133

```
Since the component is connected to ground plane.. the solder on this side will harden quite fast when you release the tip to work on the other side. Also it will take some time to heaten it up if you do it the other way around.  Maybe if you jump back and forth on each side.
```

---
## \#30 Posted by: KaramQ Posted at: 2019-05-11T18:29:49.550Z Reads: 136

```
Do any of you have aomething on r43 on your focbox? I seem to be missing it![image|375x500](upload://weNMSwPh6600agG4NId1Q32hKIg.jpeg)
```

---
## \#31 Posted by: legend27 Posted at: 2019-05-11T18:31:29.833Z Reads: 135

```
Yes I do.

![image|666x500](upload://w52yca1pw0f8FUENvk5XxeWGI2m.jpeg)
```

---
## \#32 Posted by: Fatglottis Posted at: 2019-05-11T18:33:14.744Z Reads: 129

```
![bild|522x500](upload://A9eT0d3XrEBWhJyZ5MPEhYuP1IP.jpeg)

you are missing a motor wire btw... that one I cant find :grin:
```

---
## \#33 Posted by: legend27 Posted at: 2019-05-11T18:33:35.147Z Reads: 129

```
LOL :rofl:
```

---
## \#34 Posted by: KaramQ Posted at: 2019-05-11T18:34:03.749Z Reads: 128

```
Hahahah, I just noticed that, I got it from a friend a while back and he gave it to me like this
```

---
## \#35 Posted by: KaramQ Posted at: 2019-05-11T18:34:25.637Z Reads: 130

```
I know, shitty soldering job by my friend, I’ll fix it up
```

---
## \#36 Posted by: legend27 Posted at: 2019-05-11T18:34:28.037Z Reads: 128

```
Mine says 4R7 on the top.
```

---
## \#37 Posted by: KaramQ Posted at: 2019-05-11T18:35:42.815Z Reads: 126

```
You think that will fix my problem?
```

---
## \#38 Posted by: Fatglottis Posted at: 2019-05-11T18:37:50.734Z Reads: 127

```
If your focbox wont turn on, moving the resistor to its proper place wont help this. (it still must be done though)..  (not sure if was clear or not but the resistor is sitting there on the edge) :)
```

---
## \#39 Posted by: KaramQ Posted at: 2019-05-11T18:42:53.734Z Reads: 125

```
Yeah I took it off, it’s so small!
```

---
## \#40 Posted by: AlanZhou Posted at: 2019-05-11T18:43:56.188Z Reads: 124

```
4R7 is a resistor, and its mandatory, but your vesc will turn on without any issues but might fail detection
```

---
## \#41 Posted by: KaramQ Posted at: 2019-05-11T18:45:55.909Z Reads: 123

```
Who can fix this, maybe @JohnnyMeduse, I just lost the resistor🤦🏻‍♂️
```

---
## \#42 Posted by: AlanZhou Posted at: 2019-05-11T18:50:44.519Z Reads: 118

```
its super easy to resolder
```

---
## \#43 Posted by: KaramQ Posted at: 2019-05-11T18:52:09.248Z Reads: 121

```
How tf am I supposed to do that with this piece of shit![image|375x500](upload://jCXPEnI0J6bR6mg2uV8qssZCxzY.jpeg)
```

---
## \#44 Posted by: legend27 Posted at: 2019-05-11T18:53:14.107Z Reads: 118

```
Hey! I got the same!

Must admit, it is pretty shitty. Currently trying to unsolder the C25 and the solder is not even melting...
```

---
## \#45 Posted by: AlanZhou Posted at: 2019-05-11T18:53:34.088Z Reads: 119

```
i did it on a 2$ trisonic iron....
```

---
## \#46 Posted by: KaramQ Posted at: 2019-05-11T18:54:23.717Z Reads: 119

```
I found the resistor but it seems way to small to even solder and i don’t have a good tip
```

---
## \#47 Posted by: Sn4pz Posted at: 2019-05-11T19:04:48.263Z Reads: 116

```
What 😭

Char

I'll look at this later I can't be on my phone at work
```

---
## \#48 Posted by: AlanZhou Posted at: 2019-05-11T19:05:15.278Z Reads: 111

```
flux :wink:
```

---
## \#49 Posted by: KaramQ Posted at: 2019-05-11T19:10:04.088Z Reads: 111

```
This is the hardest thing I’ve ever run into, someone please do this for me!!!
```

---
## \#50 Posted by: Fatglottis Posted at: 2019-05-11T19:13:15.760Z Reads: 116

```
@legend27
If you don't succeed with the repair and you don't mind sending it to sweden, I can do this repair for you. (and the STM32 change if its fried). Send a PM in that case.
```

---
## \#51 Posted by: legend27 Posted at: 2019-05-11T19:35:43.446Z Reads: 112

```
Geez... It is literally impossible to make the solder wet. Would a solder heat gun be faster & better?
```

---
## \#52 Posted by: AlanZhou Posted at: 2019-05-11T19:40:36.420Z Reads: 112

```
It does not work like that.
```

---
## \#53 Posted by: legend27 Posted at: 2019-05-11T19:53:22.616Z Reads: 113

```
@Fatglottis 

FINALLY GOT C25 OFF!

![image|666x500](upload://eLhijqi0FuqqdAZzXUa9HhhLj4u.jpeg) 

But it still beeps when I touch 3v3 and GND...

Next step is to unsolder this one, right?

![unsold|652x490](upload://yvp3LLmbET6qBOKWod6w4H68dvE.png)
```

---
## \#54 Posted by: Fatglottis Posted at: 2019-05-11T20:13:05.149Z Reads: 110

```
Nice! :slight_smile:
Now when you have removed the capacitor from the circuit you can try and beep it. hopefully it doesn't beep.

Yes now we want to remove the 3v3 regulator. This is tricky since it has 4 legs. Not sure how I would have started here if I did not have my hot air station :thinking:

EDIT: I would put a big solder blob covering all three legs and then do as you did with the capacitor! :cowboy_hat_face:

What you DON'T want to do is damaging the foot print on the PCB during this process.

Maybe start de-solder the larger leg first and GENTLY bend the component up a bit so that the pad comes free. But maybe there is to much solder on the pad for this :roll_eyes:

Or...If it is possible you could cut the three legs off with a cutting tool tingy, and afterwads remove the big pad.. or maybe the space is not enough for that?

Or..De-solder one small leg at a time, bending the leg upwards when it comes loose.
```

---
## \#55 Posted by: legend27 Posted at: 2019-05-11T20:24:00.831Z Reads: 105

```
Thanks for all the tricks!

I tried measuring again and it is still beeping when I touch GND and 3V3.

Really appreciate your help!
```

---
## \#56 Posted by: Fatglottis Posted at: 2019-05-11T20:49:16.530Z Reads: 105

```
Ok.. that was less good :confused:

Can you beep the 3v3 regulator now when its removed ?
(just too make sure that it was not part of the problem)

The things remaining that sits across 3v3 and gnd should only be the STM32 and the CAN transceiver I believe (Or are there capacitors on the 3v3 rail other than C25? @JohnnyMeduse  )

Now a hot air gun would really be useful. Without it, the only thing you could do is to remove the CANtranceiver using the solder blob method. And cross your fingers this is the issue.
If you still have a short between 3.3v and Gnd.. the STM32 must be replaced and you would need a new CANtransceiver if you want to utilize the CAN feature (unless you can clean up the chip with some solder wick)
```

---
## \#58 Posted by: JohnnyMeduse Posted at: 2019-05-11T21:14:41.431Z Reads: 102

```
Guys come on!!!

I have said it 5 time already!!! THE MCU IS DEAD... 

[quote="JohnnyMeduse, post:5, topic:93487"]
sound like the 3,3V is dead… did you plug it can bus ? Or else it is probably a blown mcu.
[/quote]


I have dealt with this issue numerous of time...
```

---
## \#59 Posted by: Fatglottis Posted at: 2019-05-11T22:47:04.720Z Reads: 97

```
Well, now that we scientifically have ruled out C25 and 3v3 (which would give the same symptom)...and we assume the CANchip is fine since it was never used, then yes I also vote MCU is dead.... 

I don't see why spending some time checking the simpler components first is wrong before replacing the much more complicated MCU.
This @legend27 have done by himself this now and probably gave him some experience points :+1::grinning:

Until now Legend27 had a fair chance to fix this himself without sending it for repairs.

I mean absolutely no offence to you Mr Meduse. I know you are involved a lot with VESC repairs. You definitely have more statistics of root causes than I do. I have learnt from you.
I just want make clear for others what was going on here.

For me this is simple fault tracing.. do one bit at a time. Start with the simple things. MCU was never ruled out and here is were we end up. :)

I have blown them myself and I rather change a 3v3 :sweat:
```

---
## \#60 Posted by: banjaxxed Posted at: 2019-05-12T07:11:23.212Z Reads: 96

```
Sadly you blew its mind
```

---
## \#61 Posted by: Gamer43 Posted at: 2019-05-12T08:51:00.702Z Reads: 93

```
If you opt to attempt to replace the MCU, I would recommend using chip quik if you dont have a high quality hot air station.
```

---
## \#62 Posted by: legend27 Posted at: 2019-05-14T10:08:40.733Z Reads: 79

```
Hey everyone!

Haven't actually tried any of the other solutions yet, but it just kinda hit me now why it probably broke. 

Running 40A battery on a single focbox with stock heat sink in a completely closed enclosure and pushing it a lot doesn't sound like a great idea. 

The reason I had those settings was because, I had ran them on my focbox unity, but now when I think about it, it was probably just 20A for each side of the unity...

Looking forward to try all the solutions when next paycheck arrives :slight_smile:
-Thanks guys! 

Last words;
Learn by others mistakes.
```

---
## \#63 Posted by: banjaxxed Posted at: 2019-05-14T10:36:22.464Z Reads: 68

```
3DServisas had single focbox cases in the past, that would probably do it but unless they go into production again...
```

---
## \#64 Posted by: AlanZhou Posted at: 2019-05-14T11:49:11.947Z Reads: 64

```
[quote="legend27, post:62, topic:93487"]
Running 40A battery on a single focbox with stock heat sink in a completely closed enclosure and pushing it a lot doesn’t sound like a great idea.
[/quote]

That's not really a valid reason.... The vesc should prevent itself from dying...

Even though the most I've done is 30 batt amps.
```

---
## \#65 Posted by: Sn4pz Posted at: 2019-05-14T11:57:16.366Z Reads: 62

```
If you get the kug3 single focbox case, you should be safe to run it at 40/45amps even inside an enclosure with no airflow 

I ran 45a and the highest temp I ever saw was somewhere in the 70c range (for a ~7 mile ride)👍
```

---
## \#66 Posted by: legend27 Posted at: 2019-06-02T17:29:39.300Z Reads: 49

```
Hey everyone!

Finally got some cash to spend :money_mouth_face:

Now it's time to find a hot  air gun. I've been looking on the cheapest ones and they seem to do the job. I've specifically been looking on this

https://www.aliexpress.com/item/110V-220V-700W-YOUYUE-858D-Soldering-Station-LED-Digital-Solder-Iron-Desoldering-Station-BGA-Rework-Solder/32714681480.html?spm=a2g0o.cart.0.0.9fbb3c00QUwxZw

Before I buy it, I would appreciate if someone have any experience with it, or knows whether it's go or no-go.

I've also found some solder paste

https://www.aliexpress.com/item/2pcs-10CC-Mechanic-Tin-XG-z40-Solder-Paste-Flux-Sn63-Pb37-25-45um-Syringe-For-PCB/32899594756.html?spm=a2g0o.cart.0.0.9fbb3c00QUwxZw

Thanks a lot for all of your help so far guys!
```

---
## \#67 Posted by: deucesdown Posted at: 2019-06-02T18:26:29.061Z Reads: 45

```
There are a LOT of vendors labelling their hot air station as 858D. Some have mains voltage on the wand!

https://www.youtube.com/watch?v=WPy9XYGDmWQ

I think the Yihua or Atten branded ones are usually good.

Solder paste, I believe you have to store refrigerated and it has a shelf life? I think instead, if you're just doing a few components and not a whole board, you can get away with lots of flux and good quality solder.
```

---
## \#68 Posted by: Gamer43 Posted at: 2019-06-02T20:01:20.280Z Reads: 35

```
Actually, you're better off using chip quik.

I replaced three MCUs in quick succession using the leaded chip quik set from adafruit. 
https://www.adafruit.com/product/2660?gclid=EAIaIQobChMIio20qsvL4gIVqRitBh3XpARFEAQYAyABEgL0yvD_BwE

You will need a suction cup tool or blu tack (or similar putty substance) to remove the MCU.

https://www.youtube.com/watch?v=UmD7F0--7Lc

This is the only resource I used going into the repair.
```

---

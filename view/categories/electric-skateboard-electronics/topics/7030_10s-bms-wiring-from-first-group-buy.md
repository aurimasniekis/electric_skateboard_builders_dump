# 10s BMS wiring? (from first group buy)

### Replies: 25 Views: 2397

## \#1 Posted by: cmatson Posted at: 2016-08-02T21:35:56.227Z Reads: 362

```
I haven't touched this project in a while and have not only misplaced my manual, but also the picture @longhairedboy sent me.

Long story short, I need to wire up this BMS and am not sure what goes where. 
-the e switch is the two prersoldered wires 
-the balance leads are already hooked up because I did that when I had a manual..
 
here's the link to the BMS: http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

<img src="/uploads/db1493/original/2X/0/03615b9b7c1fd0c04971dd69f8e171f00501b647.png" width="690" height="449">
```

---
## \#2 Posted by: barajabali Posted at: 2016-08-02T21:38:32.127Z Reads: 348

```
I've been wanting to buy that bms to try it out but I hear there was a bad batch going around and they were burning up. 

I'm sure it's the same as any other bms but I don't want to be wrong and confuse you further
```

---
## \#3 Posted by: Namasaki Posted at: 2016-08-02T21:49:28.619Z Reads: 343

```
P- is for negative wire to Esc's
C- is for negative wire to charge port
B- is for negative wire from battery
The positive wire from battery goes directly to Esc's positive wire and charge port positive wire.
I just hooked mine up a few days ago and so far it works like a dream.
Note: it won't even turn on unless you have the balance wires connected
```

---
## \#4 Posted by: barajabali Posted at: 2016-08-02T22:34:57.708Z Reads: 322

```
Balance ports are the same as lipo except no lead for main negative terminal.
```

---
## \#5 Posted by: treenutter Posted at: 2016-08-03T00:22:13.276Z Reads: 310

```
[quote="cmatson, post:1, topic:7030"]
the balance leads are already hooked up because I did that when I had a manual
[/quote]

You got a manual? Did you have to pay extra for it? :slight_smile:

@cmatson I've still got the data sheet from the group buy if you want to me send it to you.
```

---
## \#6 Posted by: cmatson Posted at: 2016-08-03T01:20:38.719Z Reads: 302

```
Nope, I just got one with the bms that told me what terminals were what, and all about the cutoffs etc. 

Didn't really pay much attention to it, and when I needed it, I had already lost it
```

---
## \#7 Posted by: longhairedboy Posted at: 2016-08-03T12:16:21.425Z Reads: 285

```
if i had seen this last night i would have posted another pic of the chart mine came with. 

This BMS is great, i've got one in a customer build and its working really well.
```

---
## \#8 Posted by: tim_felbinger Posted at: 2016-11-13T06:17:43.854Z Reads: 224

```
Where were you able to buy the BesTech BMS from?

I want to upgrade from my current $15 BMS (which I am bypassing for discharge) as I want to feel safer when leaving it on the charger over night
```

---
## \#9 Posted by: cmatson Posted at: 2016-11-13T17:12:43.889Z Reads: 206

```
use the link above, and contact Bestech about purchasing the BMS. 

I think they had a minimum order quantity of two.. but I may be mistaken.
```

---
## \#10 Posted by: tim_felbinger Posted at: 2016-11-13T17:31:56.937Z Reads: 203

```
Thanks. I just sent them an email. 

If the minimum order quantity is above 2 I might start a group buy for them.

Also, what does the 'E-Switch' thing mean? Is it an ON OFF button?

Thanks
```

---
## \#11 Posted by: cmatson Posted at: 2016-11-13T18:17:18.986Z Reads: 199

```
Yep, on off switch
```

---
## \#12 Posted by: Lionpuncher Posted at: 2017-09-10T22:47:27.936Z Reads: 130

```
 So if just for fun i plugged in the balance wires before i wired the main wiring in the bms, could i expect it to heat up? Not that i did that....
```

---
## \#13 Posted by: Namasaki Posted at: 2017-09-11T05:08:02.798Z Reads: 125

```
I don't think it matters which you connect first. Just have all the wires connected correctly when you turn the bms on.
If you have the balance wires connected in the wrong order, That will damage the bms.

On my very first build with Li-ions and bms, I connected the main wires first and tried to turn the bms on without connecting the balance wires. ( How Dumb Was That)
The bms would not turn on. ( obviously because it saw zero voltage from all cells) So I connected the balance wires and then it turned on and the whole episode did not damage the bms.
```

---
## \#14 Posted by: Lionpuncher Posted at: 2017-09-11T13:35:55.261Z Reads: 116

```
<img src="/uploads/db1493/original/3X/5/8/58fbe84441132ea9edead71f39012f1faf18982a.jpg" width="690" height="303">
Does that look about right? @Namasaki ?
```

---
## \#15 Posted by: Namasaki Posted at: 2017-09-11T19:05:53.375Z Reads: 112

```
Looks good to me.
```

---
## \#16 Posted by: Lambjr088 Posted at: 2017-11-03T00:35:50.726Z Reads: 99

```
@Namasaki still have this bms? If so how is it holding up?
```

---
## \#17 Posted by: Namasaki Posted at: 2017-11-03T02:18:54.325Z Reads: 92

```
Been running them on 2 builds for long time. 
Never a problem yet
```

---
## \#18 Posted by: Lambjr088 Posted at: 2017-11-03T02:28:07.922Z Reads: 89

```
Awesome thanks I'm definitely gona get a set
```

---
## \#19 Posted by: Quiles Posted at: 2017-11-08T14:11:41.271Z Reads: 85

```
@Namasaki what's preferable if i want to use BMS for charge and discharge (no bypass!)...to have a BMS with the same port for charge/discharge or with different ports?
What's the difference and impact on the the design to have one or another (if any)?
```

---
## \#20 Posted by: Namasaki Posted at: 2017-11-08T22:10:44.340Z Reads: 84

```
I don't know if it makes much difference whether there is a separate charge port or not.
I'm not an electronic engineer though so I can't really say for sure.

I prefer the Bestech bms mainly because of other reasons.
1. It's ability to handle high peak amperage.
2. The heat sinks
3. Twice the balancing current of other bms's
4. And most of all, the built in E-switch which saves you from spending an additional $40-$60 for an external E-switch that would likely fail.
```

---
## \#21 Posted by: clvnng Posted at: 2017-12-12T17:57:07.132Z Reads: 65

```
Apologies for bringing this back from the dead

@Namasaki

How does this BMS handle regen breaking? 
and does the E Switch have to be ON when charging?  so the vesc and the motors will have to sit idle?
```

---
## \#22 Posted by: Namasaki Posted at: 2017-12-12T18:38:31.875Z Reads: 66

```
The e-switch has to be on while charging. 

From the tests that I did with regen braking downhill on a full battery. 
It appears that the bms prevents charging past the over charge detection voltage. 4.28v
So my 10s pack would not go past 42.8 even when I continued braking. When I reached the bottom of the hill and released the brakes, the bms trimmed the voltage back down to 42v
I can’t say for sure but I think it is safe to assume that the bms is dissipating the excess current as heat.
```

---
## \#23 Posted by: clvnng Posted at: 2017-12-12T18:55:45.404Z Reads: 64

```
@Namasaki very interesting! thank you very much for your replying so quickly.
```

---
## \#24 Posted by: Acido Posted at: 2017-12-12T19:09:39.585Z Reads: 60

```
Someone should test this, find out where the energy goes, someone needs to make disc breaks for eskates controllable by remote
```

---
## \#25 Posted by: Namasaki Posted at: 2017-12-13T00:04:33.972Z Reads: 57

```
Disc brakes would be nice!
```

---

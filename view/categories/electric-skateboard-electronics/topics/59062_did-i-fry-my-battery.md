# Did I fry my battery?

### Replies: 18 Views: 451

## \#1 Posted by: JasperM Posted at: 2018-06-15T23:04:55.914Z Reads: 178

```
Hi guys,

The other day I setup my photon remote for my board, to do this I had to update my Focbox FW to 3.38. When I got it all working I went for a quick test ride and thats where the problem started.

The first problem was the brakes stopped working and they felt like they were trying to engage every second or so, then a few minutes later they worked.

Then the board stopped working at all, the remote was sending and receiving a signal. My remote said the temp was 57 degrees and I could smell a bit of a burning smell.

When I got home and the board cooled down the motor was spinning on my workbench under no load. When I stripped it all down I checked the Focbox and it looks fine but the battery has a burn mark on the corner of the wrapping.

So my two questions are.
What could cause this to happen in the settings?
How do I check if it is still usable?



![20180616_090341|452x500](upload://ixx65vkwkNBCTKPvJHobrsKRLbE.jpg)
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-16T01:08:22.351Z Reads: 155

```
can't really tell from the picture but looks like it short with the Can of the battery?
```

---
## \#3 Posted by: E1Allen Posted at: 2018-06-16T03:57:40.328Z Reads: 133

```
Where is the battery from
```

---
## \#4 Posted by: DougM Posted at: 2018-06-16T04:23:46.301Z Reads: 132

```
I had a lot of trouble with the metal strips between the cells overheating and eventually burning apart.  In my case it was because I used the cheap crappy strips that came with the battery welder.  Once I went to good strips all was well.

But without seeing what's under the paper I'll jump to the conclusion that it's a a burned strip.
```

---
## \#5 Posted by: JasperM Posted at: 2018-06-16T04:35:36.138Z Reads: 125

```
Its a 10S3P from DIYeboard.

How can I tell if its still usable though?
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2018-06-16T04:40:27.736Z Reads: 120

```
I would strip the pack down and inspect all the groups with a multimeter, that's how I found my problem with my pack
```

---
## \#7 Posted by: pat.speed Posted at: 2018-06-16T04:55:03.794Z Reads: 119

```
By the way you said “focboxs” I guess you have two right? And I kinda doubt you were running them at less than 15amps each, which means you would likely have drawn more current than the cells and nickel could handle, resulting in burn marks. 

The cells might be ok, but you will need to open the pack and check the wiring and possible beef it up a bit. I would even recommend getting a second pack in parallel for more current draw, or getting a 30q/25r pack made
```

---
## \#8 Posted by: JasperM Posted at: 2018-06-16T05:15:45.379Z Reads: 115

```
Ill strip it back and check with a multimeter, Ill also put some more photos up.

One Focbox, I was saying the focbox's settings.

I'm new to this stuff, what settings would you guys recommend for this battery, a Focbox and a Tunigy 6374 SK3?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-06-16T05:19:20.147Z Reads: 109

```
Ahh ok all good then, make sure no more than 30amps battery, I would recommend 25 just for precaution
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-06-16T05:53:25.177Z Reads: 111

```
Yes 30amp IS the total max. And even 25 amp will Stress the battery....i don't understand why you bought that crap battery. You Spend Money on dual focbox and Photon remote, 100$ more and you could have a Premium battery. Maybe a Bit smaller one but one that handles 40amps easily
```

---
## \#11 Posted by: JasperM Posted at: 2018-06-16T08:25:47.671Z Reads: 98

```
I didn't realise at the time that they were average.

So let say 
Motor current max 20-25A
Motor current max brake -20A
Battery current max 20-25A
Battery current max regen -20A

Would that work?
```

---
## \#12 Posted by: Jumpman Posted at: 2018-06-16T08:56:28.634Z Reads: 90

```
Your battery current max regen looks way to much.  Probably -6A max, depending on what cells are in your pack.
```

---
## \#13 Posted by: oyta Posted at: 2018-06-16T09:11:02.536Z Reads: 89

```
I cannot really say what's gone wrong. Do you have any warranty against DIY or is this because of overloading the battery pack? Need more pictures if you are going to open it up.

[quote="JasperM, post:11, topic:59062"]
Motor current max 20-25A
Motor current max brake -20A
Battery current max 20-25A
Battery current max regen -20A
[/quote]

Are these batteries Samsung 30Q? If so each battery in series are 15 A max continuous discharge, standard charge is at 1.5 A and max charge is at 4 A. That means total for the pack it is 45A max continuous discharge which could be enough depending on your set up, totalt weight, ride style and topography. For charge it has a max of 12 A. You also have two ESCs, and you need to divide these numbers by two. That means that each ESC can have settings like:

* Battery current max:  20 A (total 5A margin to not strain the battery)
* Battery current max regen:  -5A (total of 2A margin on charging)

Some say and experience that doing burst of higher currents for discharge is ok, and does not destroy the battery pack. However - this is simply according to the batteries data sheet.

EDIT:
Motor limits can be higher due to the duty cycle. I do not know what motors you have, but they can probably be raised quite a lot. For example:

* Motor current max 80A
* Motor current max brake -60A
```

---
## \#14 Posted by: JasperM Posted at: 2018-06-16T09:18:53.193Z Reads: 83

```
I've only got one Focbox so would that still mean
Battery current max 20A
Battery current max regen -5A

Or would one Focbox change the settings?

I have a Turnigy 6374 SK3 so the 80A and -60A would work?
```

---
## \#15 Posted by: oyta Posted at: 2018-06-16T09:57:08.395Z Reads: 79

```
Oh, I misread. With one focbox and motor you can have battery Max = 40A, Battery max regen = 10A. That is if the batteries are Samsung 30Q in 10s3p config.

Motor settings as put above is Ok for your motor.
```

---
## \#16 Posted by: JasperM Posted at: 2018-06-16T10:12:08.309Z Reads: 72

```
Im not sure what cells DIY use but there not 30Q.

If my battery is Ok I might try 25 and 5 to be safe.
```

---
## \#17 Posted by: pat.speed Posted at: 2018-06-16T13:24:35.834Z Reads: 59

```
I would do 25,-8 battery amps and 60, -60 motor amps. That would be a starting point, if you need more power up the motor amps but definitely not battery amps, those cells are rated at 10a max each, you have a 3p so 30a max.

First you need to check the battery, you do not want the whole board to catch fire, then even more money will be lost
```

---
## \#18 Posted by: Benjamin899 Posted at: 2018-06-16T14:32:29.289Z Reads: 53

```
Jason from DIY said they use  LG MF1, HG2 , SAMSUNG 22P , i think for the 3p pack they used the 22p/MF1 since they have exactly 10A discharge and 2,2AH capacity, both battery can take 1C charge current. So the pack has 6Ah-ish Capacity. like @pat.speed said -8 for regen looks solid.
```

---

# \[Share\] Dual 6374 + Vesc settings for comparison

### Replies: 20 Views: 1585

## \#1 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:25:41.138Z Reads: 180

```
Hey guys, I just finished my re-build and wanted to cross check my settings. If someone has a similar setup can you share your current settings

Dual 6374
2x focboxes
10s4p
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-10-08T03:27:16.450Z Reads: 179

```
I think you are asking for current settings
```

---
## \#3 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:28:09.863Z Reads: 176

```
Yes sorry, wrote it on the go. But yes you are correct.
```

---
## \#4 Posted by: BigBoyToys Posted at: 2017-10-08T03:31:14.323Z Reads: 174

```
Tell us about your battery and what you are trying to accomplish. Are u lookomg for per mellow and efficient settings, the most power amd torque possible, or somewhere in between?
```

---
## \#5 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:33:44.750Z Reads: 173

```
It's a Spacecells 4 10s4p Samsung 25r cells

Was looking for somewhere between that all out and mellow. Something like a evolve GT so I don't chew through battery
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-10-08T03:38:45.769Z Reads: 172

```
Id recommend

Motor max: 60A
Motor min: -60A

Batt max 30A
Batt min (regen): -12A
```

---
## \#7 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:40:19.964Z Reads: 167

```
So that would be 30A for each Vesc on max and min
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-10-08T03:41:10.049Z Reads: 165

```
Correct, your board has much bigger motors than an evolve GT btw 😉
```

---
## \#9 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:42:51.428Z Reads: 165

```
So each vesc would read

Motor max: 30A
Motor min: -30A

Batt max 30A
Batt min (regen): -12A. <- not sure if this should be split across so -6a each?
```

---
## \#10 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:49:31.770Z Reads: 166

```
My current setup per vesc is:

Motor max: 35A
Motor min: -35A

Batt max 60A
Batt min (regen): -7A
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-10-08T03:51:55.629Z Reads: 159

```
I think you'll need about -12A on each esc to get effective braking at speed. Many would recommend -8A Max on each tbough.
```

---
## \#12 Posted by: Enigmacpl03 Posted at: 2017-10-08T03:53:38.683Z Reads: 154

```
Why is that?

And is my Battery max current set to 60a per vesc okay or should I divide that as well
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-10-08T03:59:15.891Z Reads: 152

```
You could do 40A max on each vesc  from the battery, but no higher.  Your battery is only capable of 80 total. If you want more acceleration you can increase motor max A's.
```

---
## \#14 Posted by: Enigmacpl03 Posted at: 2017-10-08T04:01:31.269Z Reads: 148

```
Okay perfect, and just for my notebook. What settings would you use per vesc if you wanted to go balls to the wall.?

Thanks for all your help @BigBoyToys
```

---
## \#15 Posted by: BigBoyToys Posted at: 2017-10-08T04:06:28.606Z Reads: 143

```
Increase motor max A's but leave batt max at 40A.  I run a motor max of 100A on my builds but most will tell you thats too high so at your own risk 😉
```

---
## \#16 Posted by: Enigmacpl03 Posted at: 2017-10-08T04:09:31.334Z Reads: 147

```
100A? That's per vesc? Jesus 

So what's a fun range for motor max 40-60A per vesc?
```

---
## \#17 Posted by: Eboosted Posted at: 2017-10-08T04:40:21.875Z Reads: 141

```
I see you have big current numbers always, are you runing only hubs on those settings or belts as well?
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-08T05:08:05.282Z Reads: 136

```
I run My belt drive Trampa 50A battery 100A motor 😉
```

---
## \#19 Posted by: cwazy1 Posted at: 2017-10-08T05:13:08.674Z Reads: 137

```
Keep in mind, OP, that this depends heavily on your weight, setup as well as preferences. If you're a big dude, with a low gearing ratio, and like heavy torque, you're going to need more current. 

I'm 160#, 13:36 ratio, 12s4p pack, and I like +60/-50 for motor, and +20/-7 for battery on each vesc. I also ride in the inner downtown city on sidewalks, bikelanes and I need to have as minimal of jerkiness as possible.
```

---
## \#20 Posted by: Enigmacpl03 Posted at: 2017-10-08T13:57:08.844Z Reads: 125

```
Great thank you guys, I will go back and adjust and test.

@BigBoyToys @cwazy1 thank you for your time and knowledge. It's been awhile for me, so super rusty.
```

---

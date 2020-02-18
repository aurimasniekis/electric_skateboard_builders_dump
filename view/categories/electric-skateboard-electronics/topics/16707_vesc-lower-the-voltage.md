# VESC Lower The Voltage?

### Replies: 20 Views: 1201

## \#1 Posted by: Sander Posted at: 2017-01-26T15:26:44.274Z Reads: 129

```
Hi I am wondering if its possible to change the output voltage of the VESC?
Because I am soon finished with making my carbon board and the carvon v3 will not ship until april. 
That means I can't really use my board until that date. 

I will have a 12S battery(44.4V).
My motors I currently have only tolerate max 25V.

Motor information:
Model: N5065
Voltage: 18~25.2V
Power: 1800W
RPM: 270KV ( RPM / V )
Max current: 100A

So is it possible to lower the voltage in the VESC settings?
12S to 6S?

Thanks.
```

---
## \#2 Posted by: Blasto Posted at: 2017-01-26T15:36:59.771Z Reads: 123

```
Interesting question, I don't have a definitive answer (never tested for myself), but I have a few settings to suggest limiting.

you can limit your maximum duty cycle to 50% (0.5)

<img src="/uploads/db1493/original/3X/3/0/3040e95c0d378e3d8b8cff10b4778920aa35378f.png" width="690" height="358">

You can limit your ERPM also... 25V * Kv * 7 = maxERPM

Post your results! Very interested to know
```

---
## \#3 Posted by: Sander Posted at: 2017-01-26T15:41:19.519Z Reads: 112

```
[quote="Blasto, post:2, topic:16707"]
Interesting question, I don't have a definitive answer (never tested for myself), but I have a few settings to suggest limiting.

you can limit your maximum duty cycle to 50% (0.5)
[/quote]

Smart! Thanks, will do some testing with the voltage meter thing.
But I can't really test it before I get my battery pack ;)
```

---
## \#4 Posted by: devin Posted at: 2017-01-26T16:12:11.590Z Reads: 101

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#5 Posted by: Sander Posted at: 2017-01-26T16:19:19.289Z Reads: 86

```
[quote="devin, post:4, topic:16707"]
the VESC changes "effective voltage" by chopping up the current with pulse width modulation. how it does this is determined by your batt/motor/absolute max amp limit settings.

for more info on how it does this, see related thread:
[/quote]

I did not ask why my voltage is changed, I asked is it possible to lower it with the VESC...
But I think the answer I already got will work just fine ;)
```

---
## \#6 Posted by: devin Posted at: 2017-01-26T16:21:26.370Z Reads: 83

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#7 Posted by: Maxid Posted at: 2017-01-26T16:46:23.690Z Reads: 75

```
I somehow doubt that the motors only tolerate 25V.
As long as you limit the motor current to a healthy limit this should be fine with the VESC. 
Only with Car ESC that push whatever current they can deliver through your motor you could have problems.
```

---
## \#8 Posted by: NickTheDude Posted at: 2017-01-26T17:47:54.738Z Reads: 71

```
Maybe you could limit ERPM? Would that essentially reduce voltage?
```

---
## \#9 Posted by: Hummie Posted at: 2017-01-26T19:07:16.266Z Reads: 68

```
It's very likely the same enamel on this motor as others with higher rating and it will stop much higher voltage.  The voltage limit stated is likely just related to the acceptable amps as was said.  They assume if u do higher voltage ull have too many amps but with vesc u can control the amps.  
Most often with small motors the volt limit is related to what the bearings can spin. 
U must limit the max erpm if u want to use that battery with that motor.  Think it's 8600 erpm limit on vesc and what u have is kv x volts x 7.  Lots of this has been said.  

Lowering the voltage limits in the bldc tool (connected to pc) will just be setting the cutoffs and it will shut u down. Not what u want
```

---
## \#10 Posted by: Sander Posted at: 2017-01-26T23:00:29.220Z Reads: 64

```
[quote="Maxid, post:7, topic:16707"]
I somehow doubt that the motors only tolerate 25V.
[/quote]

I contacted the seller a few months ago and I asked him can it go faster?
He said something like, "Yes you can use 10S then you will reach 50km/h".

So I could actually have the 44.4V Input with 100A limit with no problem?

[quote="NickTheDude, post:8, topic:16707, full:true"]
Maybe you could limit ERPM? Would that essentially reduce voltage?
[/quote]

Good, idea! But I think the motor can handle 44.4V with no problem if I limit the amp to 100? Because voltage has nothing to do with what the motor can handle? Because its the Amp that matters, if the amp is very high the magnetic copper will be destroyed. 

So I should just be fine with 44.4V input and limit the amp.

[quote="Hummie, post:9, topic:16707"]
The voltage limit stated is likely just related to the acceptable amps as was said.  They assume if u do higher voltage ull have too many amps but with vesc u can control the amps.
[/quote]

Technically the motor should be fine if the voltage is 44.4V and max ampere is 100?
```

---
## \#11 Posted by: Maxid Posted at: 2017-01-26T23:13:16.681Z Reads: 56

```
100A is too much usually. Just look around in build threads with VESCs and see what people are using.
```

---
## \#12 Posted by: Sander Posted at: 2017-01-26T23:23:51.293Z Reads: 54

```
[quote="Maxid, post:11, topic:16707, full:true"]
100A is too much usually. Just look around in build threads with VESCs and see what people are using.
[/quote]

I think I will stick with 60A
```

---
## \#13 Posted by: Hummie Posted at: 2017-01-27T05:03:30.206Z Reads: 54

```
The vesc has temp shut offs for safety so u don't have to worry. just the amps make it hot.  If u have the battery for it you can do higher amps.  The motor amp limit is seeming not a risk and I've ridden at 200 for awhile. The battery amps I've had up to 70.  Worth knowing what temp ur motor can get up to before it will damage the magnets as that's the limit. Standard niodimium mags in hobbyKing motors they don't say but I wouldn't do over 180f. Infrared thermo is 10$
```

---
## \#14 Posted by: devin Posted at: 2017-01-27T05:19:35.049Z Reads: 50

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: Sander Posted at: 2017-01-27T18:25:52.822Z Reads: 40

```
[quote="devin, post:14, topic:16707"]
...very dangerous if both of these settings were combined as they are not the proper ratio..
[/quote]

I dont get it? Why dangerous?
Do you mean if Battmax == Motormax = Dangerous?
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-01-27T18:33:13.569Z Reads: 38

```
This is all good info to know. I have a set of NTM 270's i'd like to experiment with at 12S and i was wondering all of this as well.
```

---
## \#17 Posted by: Hummie Posted at: 2017-01-27T18:43:22.176Z Reads: 38

```
With chosing the settings on a whim you could have inconsistent acceleration at different speeds, think riding a stick shift car and sticking in just that one gear, as apposed to a straight even acceleration.  If you ride a board and experience the different curves you'll get used to it quickly whatever it is and I wouldn't call it dangerous.  70/70 equals more power at higher speeds while about 200/45 is more even yet less overall power.  Motor amp number gives more low speed power and batt amp gives more overall power.  There's a bunch of math if ur interested in the details you can search just about any post with devin
```

---
## \#18 Posted by: PXSS Posted at: 2017-01-27T18:53:30.657Z Reads: 40

```
As stated numerous times by several members, even power throughout speed curve is NOT the same as even acceleration.
```

---
## \#19 Posted by: Hummie Posted at: 2017-01-27T19:55:16.760Z Reads: 38

```
Yea, we got to the bottom, so u could set it up for even power or even acceleration depending on how u set those
```

---
## \#20 Posted by: devin Posted at: 2017-01-27T21:36:23.543Z Reads: 35

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---

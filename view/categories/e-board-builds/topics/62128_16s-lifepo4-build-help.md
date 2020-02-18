# 16S LiFePO4 build help

### Replies: 16 Views: 738

## \#1 Posted by: iBenRollen Posted at: 2018-07-17T19:38:27.050Z Reads: 175

```
Hey All,

I've slowly been building my esk8 over the last few months, and finally, have all the parts wired up. I'm using a custom 16S LiFePO4 pack I was lucky enough to source for free from my workplace. I'm using a smart BMS that has Bluetooth capability. The VESC was purchased from . And motor was sourced from Hobbyking and is the Turnigy D5035-125KV Sensored Brushless Motor. With everything wired and connected to the computer using the Torque ESC BLDC tool, I cannot get the motor to spin. I have tried quite a few different settings in the motor wizard and the motor will make noises, but nothing else. Are there good tutorials on this tool? Most tutorials are outdated using old software.
```

---
## \#2 Posted by: b264 Posted at: 2018-07-17T20:16:46.833Z Reads: 165

```
You should not run a TB VESC over 45 - 50V.  What voltage is your battery?
```

---
## \#3 Posted by: iBenRollen Posted at: 2018-07-17T20:55:08.905Z Reads: 151

```
Fully charged 58.5v but drops down to ~52v within the first few % used

I thought I read somewhere they can handle up to 60v, but I may be mistaken. What does TB stand for?
```

---
## \#4 Posted by: b264 Posted at: 2018-07-17T21:04:53.183Z Reads: 143

```
TB is Torqueboards or 

You are running that at too high a voltage.  Even if you get it to work and it's not already cooked, (probably not yet) it might malfunction and/or break while you're riding it and injure you
```

---
## \#5 Posted by: iBenRollen Posted at: 2018-07-17T21:38:45.128Z Reads: 135

```
According the their website, it is rated for up to 60v

"Voltage: 8V to 60V (Up to 14S LiPo Voltage)"
```

---
## \#6 Posted by: Battosaii Posted at: 2018-07-17T21:45:05.529Z Reads: 129

```
14s is pushing a vesc hard 16s is too much voltage. Remember while riding there are voltage spikes from the motors so it can easily go over 60v if you are already at 58v
```

---
## \#7 Posted by: iBenRollen Posted at: 2018-07-17T21:50:03.112Z Reads: 125

```
Keep in mind 16S LiFePO4 is almost the same votlage as 14S LiPO, correct?
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2018-07-17T22:06:25.661Z Reads: 119

```
LiFePO4 has a nominal voltage of about 3.2v/cell while lipo/li-ion is 3.7

lipo 12s = 44.4 V
LiFePO4 16s = 51.2 V
lipo 14s = 51.8 V

yeah, it might be too much, but it might just be possible
```

---
## \#9 Posted by: b264 Posted at: 2018-07-17T22:48:19.207Z Reads: 117

```
[quote="faithfulpuppy, post:8, topic:62128"]
LiFePO4 has a nominal voltage of about 3.2v/cell while lipo/li-ion is 3.7
[/quote]

Nominal voltage is not what matters.

The peak charge voltage will be much higher.  Also, when dealing with reactive loads like motor windings the voltage will constantly be spiking higher than the supply voltage.  Plus, when streeting your face is the failure mode, you don't want to ever run at 100% capacity.  Consumer products are generally ran at 60% maximum of their components rated voltages, which, in this case, is 60V and 63V.  So if this was a consumer product using that hardware it'd probably have an 8S li-ion (33.6V) battery.  You're fine with a 10S li-ion (42V) and a 12S li-ion (50.4V) is pushing it to the max.

You're talking about a 57.6V battery which is beyond the limits of the hardware chosen.

lipo 6S = 25.2V
lipo 8S = 33.6V
**lipo 10S = 42V**
**LiFePO4 12S = 43.2V**
lipo 12S = 50.4V
LiFePO4 16S = 57.6V
lipo 14S = 58.8V
```

---
## \#10 Posted by: deucesdown Posted at: 2018-07-17T23:53:29.689Z Reads: 105

```
Arguing the other side. Some people are very successfully running focbox at 13s aka 54.6v max.

Tb vesc is not focbox and 52v after a few % is not 54v, but with some foolishness, cleverness and courage it's aaaalmost there.

Imo if you go focbox and mod the pack to 15s you'll be in much better shape.
```

---
## \#11 Posted by: iBenRollen Posted at: 2018-07-17T23:56:25.272Z Reads: 103

```
Thanks for the good info. Are there any users here who can rework already built packs? I have quite a few of these LiFePO4 16S packs that have one dead cell, due to a defective BMS.
```

---
## \#12 Posted by: Holyman92 Posted at: 2018-07-18T02:00:27.743Z Reads: 93

```
If you're dead set on 16s I would honestly wait for @Kug3lis' esc

https://www.electric-skateboard.builders/t/fatboy-hv-esc-18s-150a-electric-speed-controller/60463
```

---
## \#13 Posted by: iBenRollen Posted at: 2018-07-18T02:01:54.045Z Reads: 86

```
Link to thread?
```

---
## \#14 Posted by: Holyman92 Posted at: 2018-07-18T02:02:13.197Z Reads: 85

```
I was editing Lol
```

---
## \#15 Posted by: deucesdown Posted at: 2018-07-18T04:00:35.250Z Reads: 75

```
[quote="iBenRollen, post:11, topic:62128"]
Are there any users here who can rework already built packs?
[/quote]

Pictures.... And how much to sell? :slight_smile:

[quote="Holyman92, post:12, topic:62128"]
dead set on 16s
[/quote]
```

---
## \#16 Posted by: hillsk8ger Posted at: 2018-10-12T13:07:29.240Z Reads: 42

```
Hi,


I would be super interested im buying one of those packs. Could rework some for you too but I am located in germany
```

---

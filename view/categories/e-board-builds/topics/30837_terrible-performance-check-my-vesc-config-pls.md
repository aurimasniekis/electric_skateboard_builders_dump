# Terrible performance - check my VESC config pls

### Replies: 19 Views: 1517

## \#1 Posted by: RiGo Posted at: 2017-08-16T23:55:35.976Z Reads: 139

```
I just finished my first build and got to configuring the VESCs (actually FOCBOX).

Took my board for a test ride and the performance was terrible. Really underpowered. Slow acceleration and poor braking. Also, couldn't even get up a 10% incline. I didn't test the max speed.

This is what I'm running:

* Dual 6355 190kV motors
* Dual FOCBOX over CAN
* 10S3P with 25R cells
* Battery supports BMS with 60A max discharge

Is there a problem with the way I've configured it or could it be something else?

Thanks!

Here's my config for each FOCBOX:


**MASTER**
<img src="/uploads/db1493/original/3X/5/b/5bb8af540127df9a068369ee13c388fb7c2ae43f.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/a/9/a9dfd859638ca3bd8ab6691b2fcfaf3b6d6d701f.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/c/b/cb14fb790576777fc8782e22882e4feb8e36e4a7.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/0/c/0c3d7ddf303c3c25d0318e4a11a39e0305315b3b.png" width="690" height="385">


**SLAVE**

<img src="/uploads/db1493/original/3X/f/0/f083723be72bf8aec3a6ce2fd9836f725dc28fb0.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/a/5/a54a248c1dffd8ddadb806ff37cfc577a8e20173.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/4/8/486574b218c47c07b45189643563046ffb40bdda.png" width="690" height="385">

<img src="/uploads/db1493/original/3X/1/a/1a396f5ed36ea144c76d74316d445e9599ce0f15.png" width="690" height="385">
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-16T23:59:20.289Z Reads: 123

```
motor max is too low. I'd up battery max to 30A each VESC and motor max 60A each VESC as a starting point. You can adjust motor max as needed but don't go higher than 30A/Vesc on battery max.

You can also raise battery min to -6A/Vesc for better braking at speed.

PS. no you won't burn out your motor/battery with these settings.
```

---
## \#3 Posted by: RiGo Posted at: 2017-08-17T00:03:09.235Z Reads: 120

```
The pack and BMS both have a max continuous output of 60A. I don't wanna be running it right at the limit. I should be getting good performance at 40A, right?

Also would rather keep regen braking at 7.5A for the pack. That's 1C recharge.

I really thought I had head room to not have to run at the pack's limits. Was I wrong?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-17T00:05:49.133Z Reads: 129

```
Motor max does not determine the current being pulled from the battery, only battery max does this. You'll be safe at 60a continuous and probably even more. Just as with fuses theres a bit of leeway until it triggers overcurrent breaks.

You won't really be regening much at all and it's worth upping the battery min for more responsive (i.e. safer) braking. 

The motor max is the most important thing to change if you want more power. If you change nothing else, just change motor max and you'll see better performance right off the bat.
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-08-17T00:08:15.812Z Reads: 123

```
Why did you set the FOC switching frequency to 40000?

Set Battery cutoff start to 30V and battery cutoff end to 28V.
Absolute max should be at 130A

then set battery min to -6 for each vesc. You can even go higher if you want (like -9A) but there are different theory's about that. I prefer having stronger brakes to save my live instead of battery life.

Motor max can be raised to for example 40A up to like 80A. But start with 40A to get used to the power.

Battery max can be raised to 30A which will be fine for the battery. Maybe the BMS struggles with it but it's not a good advice to have the BMS in the discharge cycle.  
And that gives you roughly 1000 Watts for each motor which is enough for the most people to be happy.

Motor min can be raised to -50A or higher. Just try it till it suites you. The higher the stronger is the brake.

Adjust your minimum and maximum pulsewidth. looks a bit standard to me. Maybe you adjusted it already.

Set the app configuration for the slave VESC to "No app" in the general tab.
```

---
## \#6 Posted by: RiGo Posted at: 2017-08-17T00:08:27.655Z Reads: 120

```
Sweet, thanks!

What's the relationship between battery current and motor current?

Continuously pulling 60A from the battery pack will surely kill the cells really quickly though?
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-17T00:10:22.895Z Reads: 118

```
You wont' be continually pulling 60A. It's simply the max the VESC is allowed to pull from the battery. Giving it this headroom will help with power and acceleration, but when you're at speed you'll likely be pulling 20A~ or so.

The voltage going into your pack is a constant voltage, but since your motor runs from 0-42v, it'll need more current to push the same amount of wattage coming from the battery.
```

---
## \#8 Posted by: RiGo Posted at: 2017-08-17T00:20:14.530Z Reads: 118

```
[quote="Ackmaniac, post:5, topic:30837"]
Why did you set the FOC switching frequency to 40000?
[/quote]

To make the motors quieter. Should I set it back to 20000?

[quote="Ackmaniac, post:5, topic:30837"]
Set Battery cutoff start to 30V and battery cutoff end to 28V.
[/quote]

Isn't this dangerously low voltage for lithium cells? Won't this kill them more quickly?

[quote="Ackmaniac, post:5, topic:30837"]
Motor max can be raised to for example 40A up to like 80A. But start with 40A to get used to the power.
[/quote]

[These are the motors I have](https://www.unikboards.com/en/boutique/moteur/). I think they might be Maytech but not sure. How could I find out what's their max current?

[quote="Ackmaniac, post:5, topic:30837"]
Motor min can be raised to -50A or higher. Just try it till it suites you. The higher the stronger is the brake.
[/quote]

Same with this. I'm guessing I'll have to keep it under the motor's max rated current, right?
```

---
## \#9 Posted by: RiGo Posted at: 2017-08-17T00:21:07.291Z Reads: 110

```
[quote="Jinra, post:7, topic:30837"]
You wont' be continually pulling 60A. It's simply the max the VESC is allowed to pull from the battery. Giving it this headroom will help with power and acceleration, but when you're at speed you'll likely be pulling 20A~ or so.
[/quote]

What about going up long hills? I have lots of hills where I live.
```

---
## \#10 Posted by: Jinra Posted at: 2017-08-17T00:22:52.259Z Reads: 109

```
Unless you're going up mountains, you still probably won't be pulling 60A continuous, and even if you do, your system is rated for it. In regards to voltage, your cells are lab tested to go from 4.2 to 2.5v for 250 cycles. so a 30/28 cutoff is not dangerous for the cell. Sure, it'll reduce cycle life if you hit those low voltages, but at the same time you don't want the cutoff to happen during heavy sag or when you're far away from home.
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-08-17T00:45:17.276Z Reads: 104

```
[quote="RiGo, post:8, topic:30837"]
To make the motors quieter. Should I set it back to 20000?
[/quote]

Set it to 30000 with your motors. interesting that somebody tried.

[quote="RiGo, post:8, topic:30837"]
Isn't this dangerously low voltage for lithium cells? Won't this kill them more quickly?
[/quote]

if you use your cells at the absolute max the manufacturer mentions in his specification the cells still would be good for roughly 10000 km. No chance to use the cells like this on a electric longboard for the street.
But feel free to prove me wrong if you didn't achieve 10000 km.
Worst you can do to the cells is charging them with high currents contentiously (braking doesn't count because that isn't a continuous charge), overcharging and store them for long time fully charged. 
Your cells will get more damage by aging before you can damage them by hard usage.

[quote="RiGo, post:8, topic:30837"]
These are the motors I have. I think they might be Maytech but not sure. How could I find out what's their max current?
[/quote]

These are oriiginally the Enertion R-Spec. 80A isn't a problem for them. Just try it by riding them. When they are too hot to touch them then you maybe reached the limit. If you still can touch them for at least like 3 seconds with your bare hand then shame on you and ride harder because your motors are bored.

[quote="RiGo, post:8, topic:30837"]
Same with this. I'm guessing I'll have to keep it under the motor's max rated current, right?
[/quote]

If you are ever be able to overheat your motors by braking then let me know. 

Long story short the max amp rating of the motors mostly means that you can use that amps contentious. But on a longboard you will only use that during short bursts.

When people killed their motors on a longboard they mostly tried stupid stuff. Like towing cars, burnouts or locking the motor and giving full throttle.
```

---
## \#12 Posted by: RiGo Posted at: 2017-08-17T01:09:29.831Z Reads: 96

```
Great advice. Thanks for all the help guys.

A couple more questions.

* Do I set the absolute max at 130A for each FOCBOX? So 260A total?
* What are the dangers of setting an incorrect switching frequency when using FOC?
```

---
## \#13 Posted by: lrdesigns Posted at: 2017-08-17T03:53:41.085Z Reads: 94

```
yes 130a for both. Its a saftey feature to protect the vesc for large spikes of current but is not usually effected by normal use. Kinda a software fuse. If abs max is reached the vesc will re-boot. And so long as your battery amps are reasonable your system will never draw that many amps.  

By having this at a low setting you risk the vesc re-booting when going up a steep hill. 130a is the defult and works good for most users.

Battery amps will limit total system power and is the most important setting in regards to keeping everything safe.
```

---
## \#14 Posted by: RiGo Posted at: 2017-08-17T04:15:50.669Z Reads: 89

```
Holy shit! Changed the settings to this and nearly killed myself lol

<img src="/uploads/db1493/original/3X/b/a/bac50bd388936b0da9ee91419571aba673436f6a.png" width="575" height="183">

Bottom end power is too crazy. It's worse than my Evolve on GT mode. Any way to tweak the throttle to give it an exponential curve?
```

---
## \#16 Posted by: lrdesigns Posted at: 2017-08-17T04:26:35.392Z Reads: 86

```
I would turn down battery amps but leave motor amps at 50A.

Try 20. If too much try 18. 

Keeping the motor at 50 will still give you power a slow speeds.

Edit: if you want throttle curves you need to install Ackmaniac's watt mode firmware.
```

---
## \#17 Posted by: SeanHacker Posted at: 2017-08-17T04:44:03.571Z Reads: 84

```
Yes there is. Use this firmware. https://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286
```

---
## \#18 Posted by: RiGo Posted at: 2017-08-17T05:05:02.966Z Reads: 85

```
Ok, will try Ackmaniac's firmware. Need to find a Windows PC :frowning:

Also, one last question I haven't had answered:  What are the dangers of setting an incorrect switching frequency when using FOC?
```

---
## \#19 Posted by: Jinra Posted at: 2017-08-17T05:31:31.548Z Reads: 82

```
What remote are you using
```

---
## \#20 Posted by: RiGo Posted at: 2017-08-17T05:44:16.252Z Reads: 82

```
I've used two - Benchwheel DIY remote and also a remote from another board I don't use anymore. Don't know the brand.
```

---

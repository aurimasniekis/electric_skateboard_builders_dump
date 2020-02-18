# MASSIVE voltage sag with 10s2p Samsung 30Q lithium ion pack

### Replies: 36 Views: 1226

## \#1 Posted by: Michaelj1 Posted at: 2018-05-29T13:48:20.566Z Reads: 209

```
So a while back I got a battery from @vishal_tejwani, and I’ve only been using it for a few weeks. It’s started sagging like crazy and I’m worried that it’s damaged or something. When it’s fully charged and I accelerate really hard, the battery indicator I have goes all the way from 100% to 50%. It was a pretty expensive battery, but I was wondering if anyone had any ideas? I’ve tried talking to the guy I bought the battery from, as I was wondering where it was from but he won’t answer. (Maybe he’s on vacation or something lol) if the battery is bad, could anyone point me towards a new one (over 6000mah if possible) that can fit in @Eboosted ‘s boosted style enclosure? Preferably under $300.
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-05-29T13:58:03.617Z Reads: 199

```
well 2p is kinda small, but where do you ride? Is it steep? How much do you weigh`? What is your Gearreduction and wheelsize also you vesc setting. Many things are to be considered.
```

---
## \#3 Posted by: Michaelj1 Posted at: 2018-05-29T14:00:05.579Z Reads: 197

```
My gearing is 16/36, and I know sag gets worse uphill but this is happening on level ground. I have dual 6355 170kv sensored motors
```

---
## \#4 Posted by: Michaelj1 Posted at: 2018-05-29T14:00:52.532Z Reads: 194

```
I’m pretty light, and this has been steadily getting worse. I used the battery cutoff settings @vishal_tejwani recommended for the battery
```

---
## \#5 Posted by: Michaelj1 Posted at: 2018-05-29T14:02:24.254Z Reads: 184

```
Like my friend has a boosted v2 dual with extended range, and I used to be able to run laps around his battery, but now we’re about the same
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-05-29T14:06:17.556Z Reads: 175

```
mmh weird. did you inspect the battery for any visible damages?
```

---
## \#7 Posted by: Michaelj1 Posted at: 2018-05-29T14:07:00.945Z Reads: 174

```
They’re all wrapped up so I can’t really see them
```

---
## \#8 Posted by: Ishayc Posted at: 2018-05-29T14:08:45.585Z Reads: 170

```
What is your battery max setting on each vesc?
```

---
## \#9 Posted by: Michaelj1 Posted at: 2018-05-29T14:09:15.817Z Reads: 170

```
Just to clarify, I didn’t try to talk to @vishal_tejwani about the battery until now so I’ll let u know if he and I can figure it out
```

---
## \#10 Posted by: Michaelj1 Posted at: 2018-05-29T14:09:32.008Z Reads: 167

```
Max is 57v the default
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-05-29T14:09:47.812Z Reads: 159

```
no he means the amps i guess
```

---
## \#12 Posted by: Ishayc Posted at: 2018-05-29T14:10:12.545Z Reads: 156

```
How many amps are you allowing your vesc to draw?
```

---
## \#13 Posted by: Michaelj1 Posted at: 2018-05-29T14:10:13.033Z Reads: 153

```
Ohh 20 per vesc. The max for the battery is 40a total
```

---
## \#14 Posted by: Ishayc Posted at: 2018-05-29T14:10:39.801Z Reads: 155

```
You are pushing the battery to it's maximum.
So 50% under heavy load sounds right.
```

---
## \#15 Posted by: Ackmaniac Posted at: 2018-05-29T14:10:45.971Z Reads: 154

```
Does it go to 50% under heavy acceleration and then back to like 95% or above. If yes then it is normal for the small battery.
```

---
## \#16 Posted by: Michaelj1 Posted at: 2018-05-29T14:11:13.648Z Reads: 153

```
Yeah that’s what it does. That normal? But I feel like the battery life is also getting shorter
```

---
## \#17 Posted by: Benjamin899 Posted at: 2018-05-29T14:11:57.644Z Reads: 153

```
well he did mention that he used to outperform his mate and now they are even.
```

---
## \#18 Posted by: Ackmaniac Posted at: 2018-05-29T14:12:20.402Z Reads: 155

```
How do you feel that? A voltage meter is made to show you roughly the capacity when there is no load on the battery. When you accelerate you have load. And load let's the voltage sag a bit. And when you have 42V and draw 20A a cell then it will go somewhere at like 36V or 37V and that is at no load 50% capacity.

But a 2P battery isn't really a made for performance. 10S4P or 12S4P works nice for most people.
```

---
## \#19 Posted by: Michaelj1 Posted at: 2018-05-29T14:14:07.610Z Reads: 152

```
My friend has a boosted v2 dual with extended range and I used to get way better battery life than him but it seems we’re starting to become more even. Idk, maybe it’s just placebo
```

---
## \#20 Posted by: Ackmaniac Posted at: 2018-05-29T14:17:18.766Z Reads: 146

```
Mostly when people think the battery life becomes worse is when they compare their range to the range they had at the beginning when they were not used to ride electric boards.
But the more you get used to it the harder you ride it and the more power you draw at the same distance. Huge difference especially at the beginning.
```

---
## \#21 Posted by: Michaelj1 Posted at: 2018-05-29T14:17:48.636Z Reads: 143

```
Honestly you’re probably right because I have been riding it harder haha
```

---
## \#22 Posted by: Ackmaniac Posted at: 2018-05-29T14:18:39.006Z Reads: 138

```
What are your settiings? Battery max, min and Motor max, min?
```

---
## \#23 Posted by: Michaelj1 Posted at: 2018-05-29T14:20:34.671Z Reads: 137

```
Motor max per motor is 60a, min is -60 battery max per vesc is 20 amp, and battery min per vesc is like 10a
```

---
## \#24 Posted by: Michaelj1 Posted at: 2018-05-29T14:21:10.375Z Reads: 134

```
Or -10a I forgot how battery min works i don’t have my computer right in front of me atm
```

---
## \#25 Posted by: Acido Posted at: 2018-05-29T14:22:22.910Z Reads: 134

```
Thats a weak battery for 2 motors, it can supply max 40A for your motors which could pull a LOT more than 20 if you had the battery for it

Have you considered a bigger battery?
```

---
## \#26 Posted by: Michaelj1 Posted at: 2018-05-29T14:22:46.414Z Reads: 131

```
Yeah I’m talking with they guy, I think I’m gonna get a 10s4p
```

---
## \#27 Posted by: Michaelj1 Posted at: 2018-05-29T14:23:04.903Z Reads: 133

```
He said it’s better for dual motor setups
```

---
## \#28 Posted by: Acido Posted at: 2018-05-29T14:23:08.404Z Reads: 132

```
Just add one more in paralel
```

---
## \#29 Posted by: Michaelj1 Posted at: 2018-05-29T14:23:49.431Z Reads: 125

```
My enclosure won’t fit that unfortunately, it’s gotta be put together custom so I’ll just get a new battery. It’s all good. Thanks for the help guys!
```

---
## \#30 Posted by: Benjamin899 Posted at: 2018-05-29T14:24:39.386Z Reads: 123

```
i would always build the battery bigger, less strain on the cells and longer cell life, cooler temp ect ect.
Maybe lipo fit inside the enclosure. People demonize them, but i use them in my build and love it.
```

---
## \#31 Posted by: Ackmaniac Posted at: 2018-05-29T14:25:20.912Z Reads: 119

```
-10 is a little high, in theory by the specs you can only go -4. But i always go 50% higher which would be -6 in your case. But it is also possible that the battery doesn't really care about these short bursts. Maybe it does.

If you want a new battery anyway just give it a try. Best would be if you have some self discipline and brake gently when you go fast so that you still have the good brake performance when you need it in times of crisis.

And motor max doesn't matter for the battery, he can even go to 80A. Battery max is the one that counts when it comes to the maximum amps the battery can handle.
```

---
## \#32 Posted by: Michaelj1 Posted at: 2018-05-29T16:32:24.845Z Reads: 96

```
Does anyone know someone who could make a custom 10s4p for this enclosure? Something like this?![DSC01376|690x459](upload://mohDcdpqBAHmGYMj6WjC7IJZhWi.jpg)
```

---
## \#33 Posted by: Michaelj1 Posted at: 2018-05-29T16:32:43.039Z Reads: 93

```
I’d like to keep it under $300 if possible
```

---
## \#34 Posted by: Ackmaniac Posted at: 2018-05-29T16:50:42.782Z Reads: 90

```
Extend your battery yourself. Buy 20 cells more (nkon 80€) and solder them.
I know soldering might be bad etc etc. Even if you loose 5% capacity by soldering you still gain 95%. 

(Now all battery nerds can stone me to death.)
```

---
## \#35 Posted by: Michaelj1 Posted at: 2018-05-29T16:51:34.461Z Reads: 90

```
Yeah I’d rather just buy it from someone, I’m pretty bad at soldering and I don’t want to spend money on new equipment
```

---
## \#36 Posted by: Eboosted Posted at: 2018-05-29T17:32:25.256Z Reads: 86

```
@Michaelj1

Michael would you like me to build a battery for you? I have an vanguard battery enclosure with me so I can do a perfect battery layout for it.

Hit me up via pm
```

---

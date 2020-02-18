# Vesc over_temp_fet

### Replies: 32 Views: 2977

## \#1 Posted by: boardthebuilder Posted at: 2016-09-07T11:01:54.049Z Reads: 217

```
I have 2 4.12 VESCs both on 2.18. i changed the maximum input voltage on BLDC tool to 22V because that's what my batteries are rated for. but both my VESCs shat themselves. I reset all settings but i cannot start the detection of the motor, because all the temp readings are between 300-400 degrees. HELP!!
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-09-07T11:11:31.446Z Reads: 216

```
First increase the maximum input voltage. Try it with 50V. Shouldn't be a problem. Even if your batterie has less. Because if your batterie which is most likely a 6S is fully charged it will have 4,2 V * 6 = 25,2V. So it could be that the vesc shut's down before it can detect the temperature.
So give it a try.
```

---
## \#3 Posted by: boardthebuilder Posted at: 2016-09-07T11:26:18.679Z Reads: 212

```
yeah i have 2 LiPo in 6s. the default max voltage is 57 and i get a OVER_TEMP_FET error
```

---
## \#4 Posted by: Blasto Posted at: 2016-09-07T12:41:33.283Z Reads: 199

```
Leave the max input voltage at 57V.

did you change the temperature settings?
```

---
## \#5 Posted by: Ackmaniac Posted at: 2016-09-07T13:05:32.531Z Reads: 185

```
Please post a screenshot of your actual motor configuration. That would help.
```

---
## \#6 Posted by: boardthebuilder Posted at: 2016-09-07T23:16:03.397Z Reads: 172

```
I've left the voltage at 57V and the min temp is at 80 max 100
```

---
## \#7 Posted by: boardthebuilder Posted at: 2016-09-07T23:18:54.587Z Reads: 180

```
<img src="/uploads/db1493/original/3X/1/3/1351ecf7124d0f48766b8cf100b68086fd050b7c.png" width="690" height="355"><img src="/uploads/db1493/original/3X/9/8/984e9522bf58a19a298af68767d6b8cf609dbdf4.png" width="690" height="345">
```

---
## \#8 Posted by: Blasto Posted at: 2016-09-07T23:21:59.627Z Reads: 165

```
Get a close up picture of R1, it's near the fets
```

---
## \#9 Posted by: Ackmaniac Posted at: 2016-09-07T23:37:23.140Z Reads: 164

```
You said in you first post that you have a 6s battery. 
That means at 3,7V * 6 = 22,2V,

But you set the Battery cutoff start to 33V and the cutoff end to 30V. That means the Vesc drecreases the power at 33V and stops working at 30V to prevent you to destroy your battery. And a fully charged 6S battery can only provide 4,2 * 6 = 25,2V. So you should set the correct values for a 6s batterie.
For example cutoff start at 3,6V * 6 = 21,6 V and cutoff end at 3,4 * 6 = 20,4V.

So at the moment your Vesc thinks that the battery is completely discharged.

And what motor do you have. Because 40A max motor current seems a bit low.
```

---
## \#10 Posted by: boardthebuilder Posted at: 2016-09-07T23:45:46.541Z Reads: 156

```
its for a school project, and its at school right now. ill try to get a photo when i can
```

---
## \#11 Posted by: boardthebuilder Posted at: 2016-09-07T23:57:22.118Z Reads: 156

```
I've tried reducing the voltage limits, but that's what made the VESC fail in the first place. they used to work on the default setting that I've shown there, but i know id have to change the min and the max voltage, but now after changing the settings the VESCs don't output power to the motors

As for the motors they are 85A. So if i change the amps it might work. but as I said, the VESCs aren't even outputting power in the first place, so I don't know if it would make a difference
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-09-08T00:01:15.776Z Reads: 150

```
you should not play with the max voltage limits always leave it to 57V, it will only create problem.
```

---
## \#13 Posted by: boardthebuilder Posted at: 2016-09-08T00:04:58.908Z Reads: 149

```
i learnt that the hard way. is there any way to fix it if you do change it? I don't know if I've fried the VESC
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-09-08T02:09:52.110Z Reads: 152

```
Take picture of R1 (that the Temps sensor) like @Blasto said, to see if the problem is coming from a broken sensors, are the blue light still lighting...
```

---
## \#15 Posted by: elkick Posted at: 2016-09-08T15:13:50.175Z Reads: 134

```
You will never get it to work with 6S and those battery cutoff values of 33V/30V.
```

---
## \#16 Posted by: boardthebuilder Posted at: 2016-09-08T15:26:02.736Z Reads: 133

```
What cutoff do you recommend?
```

---
## \#17 Posted by: boardthebuilder Posted at: 2016-09-08T15:27:34.289Z Reads: 133

```
The light is still lit yeah
```

---
## \#18 Posted by: Blasto Posted at: 2016-09-08T15:45:17.884Z Reads: 135

```
[quote="Ackmaniac, post:9, topic:9134"]
or example cutoff start at 3,6V * 6 = 21,6 V and cutoff end at 3,4 * 6 = 20,4V.
[/quote]

Change your settings to this for 6S
```

---
## \#19 Posted by: elkick Posted at: 2016-09-08T15:50:17.445Z Reads: 140

```
Since I don know the chemistry of you battery I can't answer this, but that table might give you an indication. It's generally for LiPo cells. 

But with 18650 for example you can go closer to the limits (means cutoff start at 3.2V and cutoff end at 3.0V since they are capable of going much lower). Still, it's better to stay on the safe side. 

<img src="/uploads/db1493/original/3X/b/a/bab2040f18ca6220daf5ae5aee3e78cd1f7fd88e.png" width="586" height="196">
```

---
## \#20 Posted by: Jebe Posted at: 2016-10-01T21:08:10.227Z Reads: 125

```
:/ got this same problem...... Was running fine on a 170kv 3kw then I hooked up the enertion 6355 - reflashed firmware and mosfet temps all reading 300 - 400 degrees
```

---
## \#21 Posted by: boardthebuilder Posted at: 2016-10-29T05:11:12.752Z Reads: 114

```
after a few months of waiting i finally got the board back from school. hooked it all up and im getting the same issue. the temps on all MOSFETs and PCB are 400oC. i changed the battery cut off and start to what you recommended and nothing changed??
```

---
## \#22 Posted by: Blasto Posted at: 2016-10-29T05:19:39.411Z Reads: 112

```
Take a pic of your vesc, your temp sensor maybe damaged
```

---
## \#23 Posted by: Jebe Posted at: 2016-10-31T07:24:21.060Z Reads: 106

```
Which is the temp sensor ?
```

---
## \#24 Posted by: Blasto Posted at: 2016-10-31T12:32:28.859Z Reads: 104

```
[quote="Blasto, post:8, topic:9134, full:true"]
Get a close up picture of R1, it's near the fets
[/quote]

R1 is the temp sensor
```

---
## \#25 Posted by: boardthebuilder Posted at: 2017-03-25T08:29:12.397Z Reads: 92

```
<img src="/uploads/db1493/original/3X/1/a/1aaec98f65a4c17de898d0dae1fa802f7bf9f4df.jpg" width="666" height="500">
```

---
## \#26 Posted by: boardthebuilder Posted at: 2017-03-25T08:35:15.938Z Reads: 92

```
<img src="/uploads/db1493/original/3X/9/2/92aedba6be43dfa0b27317384e35c0435a447bac.jpg" width="375" height="500">
```

---
## \#27 Posted by: torqueboards Posted at: 2017-03-26T07:31:26.033Z Reads: 87

```
R1 is here.

<img src="/uploads/db1493/original/3X/c/7/c7c81b04faefd8c079afcf87986c96d3a67e978f.png" width="351" height="500">
```

---
## \#28 Posted by: Jebe Posted at: 2017-03-29T03:03:55.584Z Reads: 82

```
So if the vesc fets are reading 370 degrees will it be this resistor?
I removed mine and it reads 6500ohms which seemed in range to me. 6500 ohms - approx 35 degrees celcius.
It's horrible in my shed in summer.
```

---
## \#29 Posted by: torqueboards Posted at: 2017-03-29T03:32:14.369Z Reads: 81

```
@Jebe - Yeah, correct. 20-30 Celsius is about average.
```

---
## \#30 Posted by: Jebe Posted at: 2017-03-29T04:08:19.164Z Reads: 80

```
So R1 looks ok - what else can cause this??? BTW - extended caliber hanger please !
```

---
## \#31 Posted by: xachmo Posted at: 2018-03-28T23:38:10.605Z Reads: 47

```
Anyone figure this out? Also having the same issue after upgrading firmware
```

---
## \#32 Posted by: xachmo Posted at: 2018-03-29T00:23:32.231Z Reads: 45

```
Ah got it - Had the wrong HW version checked when i uploaded the firmware. Maybe this answer will be helpful to someone else
```

---

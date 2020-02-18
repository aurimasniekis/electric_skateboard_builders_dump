# Vesc problem red flashing light

### Replies: 63 Views: 4159

## \#1 Posted by: mnelson3690 Posted at: 2017-03-13T18:33:40.647Z Reads: 280

```
So I just got my vesc and configured all the settings. Whenever I pull the throttle all the way, the power slowly decreases until it stops. Then a red light flashes 5 times. I can get it to work again if i turn off the power but it eventually will do it again. Any idea on what this is and can be solved?
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-13T18:34:55.404Z Reads: 274

```
Post your settings and pictures of your setup
```

---
## \#3 Posted by: mnelson3690 Posted at: 2017-03-13T18:37:16.887Z Reads: 265

```
<img src="/uploads/db1493/original/3X/0/7/07f28038d6f6af79f677db256a0e13751ff2f4db.png" width="690" height="380">
```

---
## \#4 Posted by: mnelson3690 Posted at: 2017-03-13T18:37:49.374Z Reads: 250

```
<img src="/uploads/db1493/original/3X/9/2/92919c93b5accc6c2f9f1ea01b13de85ab79b568.png" width="690" height="422"><img src="/uploads/db1493/original/3X/2/2/228b7cc24ea5190b3fcbe8251d0da3cc615d17ca.png" width="690" height="389">
```

---
## \#5 Posted by: mnelson3690 Posted at: 2017-03-13T18:41:52.288Z Reads: 245

```
<img src="/uploads/db1493/original/3X/a/5/a5ee1ec698ddf18fb75778b8ebc09914e7f74f26.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/e/d/ed2a26b1f40426f4458c56e5d85262128eecf418.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/d/bd8c9db87a0f0b29083942c64738af60fd8fc841.jpg" width="375" height="500">
```

---
## \#6 Posted by: mnelson3690 Posted at: 2017-03-13T18:43:05.861Z Reads: 237

```
There is all the pics. I have a 10s3p battery pack, 6374 torque motor, and VESC
```

---
## \#7 Posted by: mnelson3690 Posted at: 2017-03-13T18:52:36.826Z Reads: 235

```
I just noticed that I got an error sign that read OVER_TEMP_FET
```

---
## \#8 Posted by: mnelson3690 Posted at: 2017-03-13T18:52:47.951Z Reads: 234

```
how do i fix this
```

---
## \#9 Posted by: Blasto Posted at: 2017-03-13T19:06:26.428Z Reads: 230

```
Your cutoff start and end are way to high, set the cutoff start at 33V and end 29V
```

---
## \#10 Posted by: mnelson3690 Posted at: 2017-03-13T19:09:58.533Z Reads: 226

```
should i leave the max input voltage the same?
```

---
## \#11 Posted by: Blasto Posted at: 2017-03-13T19:10:35.021Z Reads: 216

```
Yes leave it at 57V

Your batt max is a little high in my opinion, i would set it to 30A

And set your abolute max at 130A
```

---
## \#12 Posted by: mnelson3690 Posted at: 2017-03-13T19:21:30.331Z Reads: 205

```
so i changed all of those settings but still doing the same thing
```

---
## \#13 Posted by: Blasto Posted at: 2017-03-13T19:22:23.611Z Reads: 192

```
Is the vesc getting hot to the touch?
```

---
## \#14 Posted by: mnelson3690 Posted at: 2017-03-13T19:22:55.913Z Reads: 189

```
no 
not at all.
```

---
## \#15 Posted by: mnelson3690 Posted at: 2017-03-13T19:24:01.733Z Reads: 189

```
i dont have the sensor wire plugged in. Could that be the issue?
```

---
## \#16 Posted by: Blasto Posted at: 2017-03-13T19:24:36.190Z Reads: 191

```
No you have it set as sensorless in the bldc tool
```

---
## \#17 Posted by: mnelson3690 Posted at: 2017-03-13T19:25:16.655Z Reads: 193

```
okay. I talked to somebody at enertion and they said to go buy a new cord. I dont get how that could be the problem
```

---
## \#18 Posted by: Blasto Posted at: 2017-03-13T19:26:03.272Z Reads: 195

```
New cord?? It's a tb vesc....
```

---
## \#19 Posted by: mnelson3690 Posted at: 2017-03-13T19:26:49.845Z Reads: 190

```
tb? what does that mean
```

---
## \#20 Posted by: mnelson3690 Posted at: 2017-03-13T19:27:06.070Z Reads: 189

```
I just got it today from diyelectricskateboard
```

---
## \#21 Posted by: Blasto Posted at: 2017-03-13T19:27:19.690Z Reads: 179

```
Torqueboard vesc, from diyelectricskateboard
```

---
## \#22 Posted by: mnelson3690 Posted at: 2017-03-13T19:27:38.204Z Reads: 178

```
yeah that is it
```

---
## \#23 Posted by: Blasto Posted at: 2017-03-13T19:29:16.174Z Reads: 178

```
To me it sounds you have a small manufacturing issue, the temperature sensor is R1, but that doesnt mean the issue is there
```

---
## \#24 Posted by: mnelson3690 Posted at: 2017-03-13T19:29:38.323Z Reads: 176

```
Im still getting this issue
```

---
## \#25 Posted by: mnelson3690 Posted at: 2017-03-13T19:30:22.808Z Reads: 177

```
<img src="/uploads/db1493/original/3X/7/5/75dd55fee7520431c52fd230e38ee2663a0e797f.png" width="690" height="448">
```

---
## \#26 Posted by: JohnnyMeduse Posted at: 2017-03-13T19:31:24.341Z Reads: 170

```
As @Blasto said R1 is probably defect 😧
```

---
## \#27 Posted by: mnelson3690 Posted at: 2017-03-13T19:32:50.054Z Reads: 166

```
so i should get a new vesc?
```

---
## \#28 Posted by: Blasto Posted at: 2017-03-13T19:33:04.558Z Reads: 165

```
Ya something is up with your temperature reading... your at 100degC, stuff would start to burn. Take this up w diyelectricskateboard

98% sure this is a manufacturing defect, no bad settings would cause this to happen
```

---
## \#29 Posted by: mnelson3690 Posted at: 2017-03-13T19:34:48.639Z Reads: 164

```
there isn't any setting that can be changed to fix this?
```

---
## \#30 Posted by: mnelson3690 Posted at: 2017-03-13T19:36:58.438Z Reads: 165

```
okay thanks guys. This is just so frustrating as ive waited 4moths
```

---
## \#31 Posted by: Blasto Posted at: 2017-03-13T19:37:10.215Z Reads: 165

```
Could offset the mosfet temperature start & end by 70 degrees... but that's the bowboy way of doing it
```

---
## \#32 Posted by: mnelson3690 Posted at: 2017-03-13T19:38:09.248Z Reads: 161

```
what would the exact numbers be?
```

---
## \#33 Posted by: Blasto Posted at: 2017-03-13T19:39:22.195Z Reads: 160

```
Well i dont recommend doing it, but mosfet start 150 end 170
```

---
## \#34 Posted by: mnelson3690 Posted at: 2017-03-13T19:39:48.821Z Reads: 155

```
I mean if it's already broken why not
```

---
## \#35 Posted by: Blasto Posted at: 2017-03-13T19:40:31.275Z Reads: 152

```
Because you're covered from a manufacturing defect?
```

---
## \#36 Posted by: mnelson3690 Posted at: 2017-03-13T19:41:12.227Z Reads: 153

```
ohh okay. What is wrong with setting the temp higher?
```

---
## \#37 Posted by: Blasto Posted at: 2017-03-13T19:42:52.021Z Reads: 155

```
Well you would be shutting off the temperature protection... and im not entirely sure that the reading is good or not

Maybe one of your mosfets is actually shorted out and is getting hot

Hard for me to tell, there's a forum in the way
```

---
## \#38 Posted by: mnelson3690 Posted at: 2017-03-13T19:56:42.933Z Reads: 150

```
Well i just rode it and it works totally fine now
```

---
## \#39 Posted by: Blasto Posted at: 2017-03-13T19:58:48.135Z Reads: 148

```
Keep in mind thats a cowboy fix, could lead to permanent damage if there's an actual temperature issue

[spoiler]and you're welcome[/spoiler]
```

---
## \#40 Posted by: mnelson3690 Posted at: 2017-03-13T20:05:03.943Z Reads: 145

```
thank you very much
```

---
## \#41 Posted by: mnelson3690 Posted at: 2017-03-13T20:05:15.792Z Reads: 139

```
would running it with the sensor wire help
```

---
## \#42 Posted by: Blasto Posted at: 2017-03-13T20:15:01.485Z Reads: 135

```
Sensors will help the startup torque, you need to do a motor detection so the vesc knows the hall table, after that just tick the sensor mode
```

---
## \#43 Posted by: Namasaki Posted at: 2017-03-13T20:30:09.952Z Reads: 137

```
You also have to connect the motor wires a certain way to run sensors or you will fry something. 
Do not attempt sensor operation until you've done your homework on it.
```

---
## \#44 Posted by: Blasto Posted at: 2017-03-13T21:19:24.280Z Reads: 131

```
[quote="Namasaki, post:43, topic:19018, full:true"]
You also have to connect the motor wires a certain way to run sensors or you will fry something. Do not attempt sensor operation until you've done your homework on it.
[/quote]

Not sure what you mean here, he has tb motors with sensors, he just needs to plug them in the sensor port of the vesc and run a motor detection so the vesc can know the position of the sensors
```

---
## \#45 Posted by: Namasaki Posted at: 2017-03-13T22:24:05.492Z Reads: 122

```
When you run motors sensored, you have to match the phase wires between the Esc and motor. 
Unless the Vesc is different than all other Esc's concerning this.
```

---
## \#46 Posted by: Blasto Posted at: 2017-03-13T22:27:39.115Z Reads: 122

```
[quote="Namasaki, post:45, topic:19018"]
Unless the Vesc is different than all other Esc's concerning this.
[/quote]

Yes the vesc is able to detect the position of the hall sensors, you can put them in any order
```

---
## \#47 Posted by: Namasaki Posted at: 2017-03-13T22:32:44.808Z Reads: 123

```
Well, that sure is good news. 
Does that work in bldc mode or just foc?
```

---
## \#48 Posted by: Blasto Posted at: 2017-03-13T22:33:59.387Z Reads: 121

```
[quote="Namasaki, post:47, topic:19018"]
Does that work in bldc mode or just foc?
[/quote]

In both modes you can detect the hall sensor position, but you need to it in it's respective tab
```

---
## \#49 Posted by: hannesr Posted at: 2017-03-18T15:39:56.862Z Reads: 107

```
I have the same problem, starts out around 100-107, also the pins for the rc receiver was completely loose. I waited several months too, super frustrating... since I can't test it with my receiver, I can't see what the temperature effect would be after running for a while either...
```

---
## \#50 Posted by: LordSnow Posted at: 2017-03-19T23:28:38.140Z Reads: 104

```
I have the exact same issues (110+ C FET temps) and fault showing up on my VESC that I just received from  this week. I thought it was an issue with my settings and have been double- and triple-checking everything.

To me, this just confirms that they have a bad batch.
```

---
## \#51 Posted by: PXSS Posted at: 2017-03-20T05:13:48.123Z Reads: 101

```
Send it back. Not worth the money.
```

---
## \#52 Posted by: basselope Posted at: 2017-03-20T19:34:57.688Z Reads: 96

```
Having the same exact issue with my new VESC from DIY. Reading mosfet temp of 100+°C on startup.
```

---
## \#53 Posted by: Blasto Posted at: 2017-03-20T19:53:45.747Z Reads: 98

```
@basselope @LordSnow @hannesr @mnelson3690

  Is anybody able to read the resistor code of **R2**, should be a 3 digit code

I have a feeling you all have a common problem

<img src="/uploads/db1493/original/3X/2/8/28b329a66ddda2987ce4c0bc6a0064d738c76900.jpg" width="690" height="476">
```

---
## \#54 Posted by: basselope Posted at: 2017-03-20T23:36:16.123Z Reads: 94

```
01C? Not sure if O/0 or I/1 since it's so small, but that's what I can see
```

---
## \#55 Posted by: Blasto Posted at: 2017-03-20T23:44:27.605Z Reads: 96

```
Thanks, yes that is the right code (01C = 10k ohm resistor). So thats not the problem
```

---
## \#56 Posted by: JohnnyMeduse Posted at: 2017-03-20T23:54:17.702Z Reads: 97

```
Could you check if R1 space is populate.

<img src="/uploads/db1493/original/3X/8/c/8c02e135d40602ad35a281699e3895a988b4d442.JPG" width="690" height="476">
```

---
## \#57 Posted by: basselope Posted at: 2017-03-21T00:35:49.175Z Reads: 91

```
It's there. If there any markings on it, I can't see them because I still have the shrink wrap on
```

---
## \#58 Posted by: JohnnyMeduse Posted at: 2017-03-21T00:44:55.280Z Reads: 91

```
no there no marking on it, better contact @torqueboards look like it might be a manufacturing error :cry:
```

---
## \#59 Posted by: hannesr Posted at: 2017-03-21T07:28:57.611Z Reads: 97

```
Yeah @torqueboards what should we do? The best I got from you was to send it back (didn't get any response on what to do with shipping, shipping here alone was $40)... I'm also not eager to wait another two months ore more like I did with this one. Now you went into non responsive mode. I would've been a loyal customer if you only treated with respect, and not cheated me with my money... Oh and it was also delayed a month from estimated delivery...
```

---
## \#60 Posted by: torqueboards Posted at: 2017-03-21T07:54:00.065Z Reads: 98

```
Hey guys.. Sorry didn't see this info until I got tagged.

There actually seems to be an issue with a bad R1 component. We've tested it and R1 fixed the issue. So it's just a bad temp sensor component. You would have to replace it.

We'll be happy to replace it for you. It would require you to ship back your current VESC. We can give you credit for the shipping costs and send you a new VESC as a replacement.

I'll send a direct PM to each of you who mentioned as we should have a new batch with the R1 issue fixed.

@mnelson3690
@hannesr
@lordsnow
@basselope

For anyone else who has an issue please contact me via email dexter@ and/or Live Chat. It's not too often we check the forums. 

@hannesr - Contact us on live chat and we can help you. If your looking for immediate help I'd refer to Live Chat. We can ship it out to you soon and/or put it aside. Unfortunately, you are overseas so this isn't as easy. Typically, we recommend overseas customers to purchase a bigger order for free shipping.
```

---
## \#61 Posted by: FinnishSnowmobiler Posted at: 2017-04-20T21:34:59.105Z Reads: 89

```
@torqueboards

I also have the exact same problems that were mentioned in a previous post (loose remote-pins and mosfet temp. readings starting from 110C). The pins were easy to solder back but I've got no idea of the mosfet temps. How dangerous would it be for the VESC to just run the board without those sensors? 

The riding season is starting soon so is there some intelligent solution to my problem? And by that I mean like shipping VESC back to you. The VESC hasn't been ridden yet but the powering wires are shortened.

Greeting from Finland, by sending it back there could be some problems with customs but I guess it can be managed.
```

---
## \#62 Posted by: torqueboards Posted at: 2017-04-21T02:00:10.080Z Reads: 82

```
We'll it's better to switch them out. They're actually in a convenient place on the VESC and isn't as difficult as other things. You can ship them back and we'll send you new ones. Up to you. Let us know :)
```

---
## \#63 Posted by: Salo_munki Posted at: 2017-09-12T12:33:42.058Z Reads: 49

```
hi. i was reading your chat with @mnelson3690 and i have a similar problem where my motor hasn't run at all. the red light flashed when i accelerate and the BDLC tool says "detection failed" when i need to detect the motors parameters. i have no idea what to do
```

---

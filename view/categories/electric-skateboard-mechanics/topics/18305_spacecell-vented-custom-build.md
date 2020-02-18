# SpaceCell Vented - Custom Build

### Replies: 63 Views: 4121

## \#1 Posted by: Jwiz Posted at: 2017-02-27T06:11:08.189Z Reads: 230

```
My build
Turnigy SK3 192 Kv motor
39"x10" 7  ply hard rock maple board
Enertion vesc-x
Enertion Space cell 10s3p pro3 battery
Alien power system remote
83 enertion wheels
Abec 9 bearings

I weigh 180
And I get about 23mph at top speed with this build, I get about 16 miles on a full charge and the board doesn't take Hills too great. I feel like I'm not getting what I can out of it.
Can anyone help me out. I'm semi new to e-skating.
```

---
## \#2 Posted by: Alextech Posted at: 2017-02-27T07:11:11.493Z Reads: 222

```
What's your gearing? And size of motor.
```

---
## \#3 Posted by: Jwiz Posted at: 2017-02-27T07:45:13.976Z Reads: 208

```
I'm not sure my gearing I'm using whatever it came stock as, I don't know how to know that. It's 6374 motor
```

---
## \#4 Posted by: Luke Posted at: 2017-02-27T09:36:55.206Z Reads: 196

```
What are your vesc motor settings?
```

---
## \#5 Posted by: Jwiz Posted at: 2017-02-27T22:31:35.885Z Reads: 184

```
<img src="/uploads/db1493/original/3X/d/1/d126c80d4ca04dd8b1899b3860f4fbf9cc267746.JPG" width="666" height="500">
```

---
## \#6 Posted by: Jwiz Posted at: 2017-02-27T22:32:31.770Z Reads: 175

```
These are my current settings
Do you know what would be the best for this build?
```

---
## \#7 Posted by: Jwiz Posted at: 2017-02-27T22:33:15.402Z Reads: 170

```
15t/36t 12mm wide
```

---
## \#8 Posted by: Namasaki Posted at: 2017-02-27T22:40:18.046Z Reads: 171

```
I'm running a dual setup with 190kv motors, 10s voltage and 15/36 gearing and 83mm wheels.
All I'm getting is 23mph as well. 
By changing your vesc settings, you can increase performance in terms of acceleration and torque for climbing hills but if you want to increase top speed, you'll need higher gearing or larger wheels which will in turn reduce your ability to climb hills.
```

---
## \#9 Posted by: mccloed Posted at: 2017-02-27T22:40:51.183Z Reads: 168

```
My suggestion would be to bump up the motor max to, at least, 50. I run all my 10s boards at 60amp max, but I would say to start at 50 and see how it goes. That should be a decent set-up with the 192kv motor. BTW I do not own a VESC-X, only VESC 4.12.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-02-27T22:44:11.716Z Reads: 167

```
You can up your motor max to 80a and your battery max to 40a.
Those settings will be perfectly safe for your motor, vesc and space cell battery and will give you a noticeable boost in power for climbing hills however it will not increase top speed.
```

---
## \#11 Posted by: Jwiz Posted at: 2017-02-27T23:24:30.855Z Reads: 168

```
Is there any way to increase range?
```

---
## \#12 Posted by: Namasaki Posted at: 2017-02-27T23:57:05.103Z Reads: 168

```
Your already getting 16 miles from a 10s3p. I'd say thats pretty good mileage especially if your climbing any hills.
BTW, if you increase your motor and battery max amps in bldc tool to improve power, you might see a little loss in mileage because the more amps you pull the faster your battery will deplete. So it's a trade off.
```

---
## \#13 Posted by: Jwiz Posted at: 2017-02-28T16:28:22.993Z Reads: 160

```
Thanks man for the settings, my board just blew up and now I'm out 800$, whole thing caught on fire
```

---
## \#14 Posted by: Alextech Posted at: 2017-02-28T16:43:50.981Z Reads: 154

```
What? No that's crazy!
```

---
## \#15 Posted by: saul Posted at: 2017-02-28T17:59:11.862Z Reads: 156

```
wow really? I would think you'd trip the battery fuse. guess that is useless.... :thinking:

did it happen at full charge or empty? because the cutoff at 30v is too low for 10s...
```

---
## \#16 Posted by: Jwiz Posted at: 2017-02-28T18:12:27.291Z Reads: 154

```
98% battery was on it
Didn't even fully push the throttle.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-02-28T18:40:22.635Z Reads: 158

```
The settings didn't cause that. Something else happened. If your battery blew up it's because a cell got shorted or went into thermal runaway. The spacecell is designed to handle 40a
That's because it has a 40a fuse. 
The cells in that battery are rated for 20a ea. 
20a x 3p is 60a total load capacity.
```

---
## \#18 Posted by: Jwiz Posted at: 2017-02-28T18:53:04.201Z Reads: 160

```
Do you think it was my error or the company error?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-02-28T19:03:06.046Z Reads: 160

```
Hard to say. You would have to open the battery pack to see what happened. I'm guessing either a cell got shorted on its self or against another cell in its group or maybe a bad cell that over heated.
```

---
## \#20 Posted by: Jwiz Posted at: 2017-02-28T19:09:59.700Z Reads: 164

```
Considering there is nothing left of my battery, I can't really show you or see anything.
```

---
## \#21 Posted by: Namasaki Posted at: 2017-02-28T20:04:18.616Z Reads: 177

```
Very sorry for your loss
```

---
## \#22 Posted by: Malibujv Posted at: 2017-02-28T20:47:01.711Z Reads: 203

```
Not sure if it can help but could you please take a picture?
Sorry for your loss!
```

---
## \#23 Posted by: Jwiz Posted at: 2017-03-01T01:10:46.771Z Reads: 201

```
<img src="/uploads/db1493/original/3X/6/c/6c1058fb58e3581ae84d771aae2a299493c7d4fa.PNG" width="281" height="500">
```

---
## \#24 Posted by: Namasaki Posted at: 2017-03-01T01:35:56.715Z Reads: 199

```
Gotta be a battery failure. Where you able to salvage anything?
```

---
## \#25 Posted by: Jwiz Posted at: 2017-03-01T04:37:19.043Z Reads: 197

```
Salvaged nothing. Everything went.
```

---
## \#26 Posted by: mmaner Posted at: 2017-03-01T04:40:58.872Z Reads: 194

```
Good lord, that sucks man.  So sorry for you.
```

---
## \#27 Posted by: PXSS Posted at: 2017-03-01T06:11:35.780Z Reads: 189

```
What about the fuse? It should have prevented this.  Was it removed?

IMO if you didn't tamper with the space cell at all it's enertions fault. The battery is supposed to have a BMS and fuse in place to prevent this sort of thing. 
If your battery caught fire then the short must have been internal since the BMS and fuse did nothing. 

Was your battery damaged beforehand? What was your enclosure like? Did you run over anything that could have pierced it?
```

---
## \#28 Posted by: Jwiz Posted at: 2017-03-01T06:23:07.243Z Reads: 177

```
That's why I'm so confused that this happened. the fuse was never tampered with.
```

---
## \#29 Posted by: Jwiz Posted at: 2017-03-01T06:24:36.986Z Reads: 179

```
No that was the very first time I had ever taken it out on the street. The first time was at my schools rubber track.
```

---
## \#30 Posted by: Jwiz Posted at: 2017-03-01T06:25:19.678Z Reads: 177

```
Was extremely careful not to messed with anything or have anything mess with the battery
```

---
## \#31 Posted by: PXSS Posted at: 2017-03-01T06:25:58.363Z Reads: 177

```
What about the enclosure? What was it like? Do you have any pictures before the fire? I looked at all your settings and they look good.
```

---
## \#32 Posted by: Namasaki Posted at: 2017-03-01T06:27:00.638Z Reads: 172

```
There could have been one or more faulty cells in the pack that just overheated and ignited. Thermal runaway.
```

---
## \#33 Posted by: Namasaki Posted at: 2017-03-01T06:27:41.856Z Reads: 171

```
How long have you had the space cell?
Maybe you should send an email with that pic to Enertion
```

---
## \#34 Posted by: Jwiz Posted at: 2017-03-01T06:31:38.853Z Reads: 166

```
I literally received the space cell about 1 week ago, made sure the enclosure was safe. Nothing could have pierced it and messed with anything internally.
```

---
## \#35 Posted by: Jwiz Posted at: 2017-03-01T06:32:30.392Z Reads: 164

```
I don't have a picture but I know that the enclosure was under no stress and was fully water proofed.
```

---
## \#36 Posted by: Jwiz Posted at: 2017-03-01T06:33:55.253Z Reads: 165

```
My board was about as new as it can get
```

---
## \#37 Posted by: PXSS Posted at: 2017-03-01T06:37:11.167Z Reads: 162

```
Yep. I'm trying to rule out external sources of error. If his enclosure was clean and safe then it's absolutely the manufacturing. If it was a bad cell, the BMS should have helped to keep it in check while charging. I'm assuming he has no way of knowing individual voltages for the series packs. 

Whether it was a bad cell or a bad weld, I think this one is on Enertion. Hopefully they will do right by him
```

---
## \#38 Posted by: PXSS Posted at: 2017-03-01T06:39:10.718Z Reads: 160

```
I'd hit up @onloop and enertion support. I think you got a good case to get it covered under warranty (if it has any)
```

---
## \#39 Posted by: Jwiz Posted at: 2017-03-01T06:53:51.779Z Reads: 159

```
Thank you all for the help. I have the upmost respect for all of you taking the time to help me. Sorry about my rude attitude earlier,  I was just hit with huge emotion, because so much has been saved up for my board to be made and it literally went up in flames within days.
```

---
## \#40 Posted by: Jwiz Posted at: 2017-03-01T07:05:31.093Z Reads: 160

```
I love enertion and couldn't get enough of watching videos of enertion's products. I have contacted enertion support. I hope @onloop and Enertion can find a way to help me out.
```

---
## \#41 Posted by: PXSS Posted at: 2017-03-01T07:09:11.239Z Reads: 159

```
I'd be pretty pissed too... specially since it looks like you did everything you could to keep it safe!
It looks like you were almost exclusively using enertion parts too which is good I guess since it'll be easier to claim that you weren't using any shady components.
```

---
## \#42 Posted by: Jwiz Posted at: 2017-03-01T07:18:22.215Z Reads: 164

```
Everything electronic was enertion except for the motor. The motor mount and pulley were also enertion, along with the trucks and wheels. Remote was from torqueboards website
```

---
## \#43 Posted by: onloop Posted at: 2017-03-01T13:04:45.178Z Reads: 163

```
Hey mate. This totally sux. Sorry for your loss.

Please share some pre-fire photos with our customer service team. We need to see your install.

With the info we have now its hard to diagnose the issues. 

At this stage there are two likely possibilities.

1. The products were somehow faultly and we cover everything and get you running again.

2. The install was somehow bad. Specifically, the deck was too flexy. The cells (welds) got damaged and got over discharged or short circuited.

Please talk with support and provide all the details. We'vr never seen this happen with a space cell before so we are taking this matter very seriously.

Regards
Jason.
```

---
## \#44 Posted by: Jwiz Posted at: 2017-03-01T16:04:11.877Z Reads: 154

```
@onloop,
Thank you for being a very awesome company, I sent over the pictures I had of it beforehand. I hope it can help.
```

---
## \#45 Posted by: SeanHacker Posted at: 2017-03-01T16:28:49.242Z Reads: 152

```
@onloop is really good about getting things replaced when a defect is present. Sorry that happened to your board dude. That's gotta be such a shitty feeling. I'm really curious to what actually happened to it.
```

---
## \#46 Posted by: SirDiff Posted at: 2017-03-01T16:43:58.285Z Reads: 149

```
I think everybody is curious, this could happen to anybody :frowning: I'm sorry for you mate
```

---
## \#47 Posted by: Surfer Posted at: 2017-03-01T17:28:01.198Z Reads: 142

```
Omg!!! Sorry for your loss mate.
```

---
## \#48 Posted by: okp Posted at: 2017-03-01T19:13:55.041Z Reads: 139

```
wow ! that's how most of the dinosaurs disappeared !

:slight_smile:
```

---
## \#49 Posted by: JohnnyMeduse Posted at: 2017-03-01T19:32:57.010Z Reads: 139

```
[quote="unik, post:48, topic:18305"]
that's how most of the dinosaurs
[/quote]

Most... does that mean there is still some around 😧
```

---
## \#50 Posted by: barajabali Posted at: 2017-03-01T19:46:38.869Z Reads: 132

```
Yes, alligators
```

---
## \#51 Posted by: okp Posted at: 2017-03-01T19:49:57.395Z Reads: 134

```
ahh you saved me !
```

---
## \#52 Posted by: scottkellum Posted at: 2017-03-01T20:20:41.377Z Reads: 131

```
That’s not a carbon fibre deck is it? Enertion didn’t wrap that line of batteries (mine wasn’t anyway) so it could potentially short on the deck itself or something in the deck shorting the battery itself.
```

---
## \#53 Posted by: Jwiz Posted at: 2017-03-02T00:47:13.431Z Reads: 122

```
No it's not carbon fiber
```

---
## \#54 Posted by: JdogAwesome Posted at: 2017-03-03T16:19:34.700Z Reads: 102

```
Wow this is crazy! But I gotta say, it must have been pretty cool when it went up in flames ey?! Obviously I'm kidding idk what I would if my board died, I've put so much time and effort into it. Anyways it sounds like what @onloop said about the board being to flexible could be a problem, but how flexy was your board? Like I could see a problem with a boosted deck and having the space cell in the middle lol, but just a bit of flexibility would be fine.
```

---
## \#55 Posted by: Namasaki Posted at: 2017-03-03T16:33:55.749Z Reads: 104

```
Would you mind posting your pre-fire pics here for us to see?
```

---
## \#56 Posted by: Namasaki Posted at: 2017-03-03T16:37:03.153Z Reads: 107

```
In the beginning of the thread he mentioned a 39x10
7 ply hard rock maple deck. 
That shouldn't be too flexible for a 180 lb rider
```

---
## \#57 Posted by: Jwiz Posted at: 2017-03-03T17:05:09.722Z Reads: 105

```
<img src="/uploads/db1493/original/3X/2/0/204a42ee7a1cbff7ba6afded8970a6c917e7faae.JPG" width="241" height="500">
This is all I have of it before
```

---
## \#58 Posted by: sl33py Posted at: 2017-03-03T19:34:46.108Z Reads: 102

```
That SUCKS!  So sorry to see this...

Do you have a link to the deck used?  it looks like a downhill style board w/ a profile/raised edges which should stiffen it from flexing... and at *only* 180 - this shouldn't be flexy i think.  But link and we can confirm?

Great to see @onloop jump in here.  I've had exceptional customer service from him and his team the few times i needed it.  Fingers crossed they are able to help you out!

best of luck.
```

---
## \#59 Posted by: Jwiz Posted at: 2017-03-04T00:49:04.214Z Reads: 100

```
 Yeah here is the link to the longboard deck, I got it from this company based out of Huntington beach in California where I live. They are family owned and make beautiful longboard decks. 

http://www.customskateboards.com/Blank-Longboards/Blank-Laying-It-Down-Longboard
```

---
## \#60 Posted by: Mrmoonlight Posted at: 2017-03-04T04:54:51.960Z Reads: 102

```
Damn!

Glad you got out of that okay. 

Enertion is a pretty standup company. If it turns out to be a faulty space cell, I'm sure onloop will make sure you're taken care of. 

What was the condition of your enclosure? Flexy decks and batteries don't usually mix well, but if your deck was flexing too much, It's very likely that your enclosure would have cracked before your battery pack blew. [quote="Jwiz, post:23, topic:18305, full:true"]
<img src="/uploads/db1493/original/3X/6/c/6c1058fb58e3581ae84d771aae2a299493c7d4fa.PNG" width="281" height="500">
[/quote]
```

---
## \#61 Posted by: Jwiz Posted at: 2017-03-04T06:15:54.540Z Reads: 94

```
No, my deck was definitely not too flexible. That was one of the biggest things I made sure of when bought this deck. That was probably the most common thing I was warned about before making it.
```

---
## \#62 Posted by: Iceni Posted at: 2017-03-04T10:38:13.314Z Reads: 91

```
Damn man, sorry for your loss.
I had the same thing happen to my space cell a while ago, I was lucky enough it didn't catch fire though.

After an inspection I saw that the nickel strip had broken between the cells in one parallel group leaving one group with only one cell to take the full load, which made it go thermal.

And I had it mounted in a solid aluminium case with padding on the inside and rubber standoffs between the board.
```

---
## \#63 Posted by: 3d-guy Posted at: 2017-03-04T11:16:29.895Z Reads: 89

```
love the title (spacecell vented) more like spacecell went nuclear lol.
```

---

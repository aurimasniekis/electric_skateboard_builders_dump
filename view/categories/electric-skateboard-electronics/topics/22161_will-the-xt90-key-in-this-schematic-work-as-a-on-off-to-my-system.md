# Will the XT90 key in this schematic work as a on/off to my system?

### Replies: 28 Views: 1126

## \#1 Posted by: marcus Posted at: 2017-05-01T19:08:49.246Z Reads: 149

```
Hey guys, quick question. So I am intending on constructing a 10s1p (2x 5s1p in series) board in the coming weeks. At the moment, I intend on charging each lipo separately on my charger (I understand this will be a bitch). Using this diagram for inspiration from a forum post by DeathCookies, I believe this should work out perfectly!

Yet, I was wondering it the XT90 loopkey, while although I have to unplug it to charge my batteries (it disconnects the bridge of the series), can I also use this key as my on/off switch in the system? As in, when I pull out the key my system will technically be "off". I want to make sure that I dont damage my other components etc. 
<img src="/uploads/db1493/original/3X/6/a/6ae1e31b9a79ed366c2c01cda85c9358eecba1c7.jpg" width="479" height="500">

Thanks so much for your help,

Marcus
```

---
## \#2 Posted by: Hummie Posted at: 2017-05-01T19:20:51.838Z Reads: 121

```
Looks good to me
```

---
## \#3 Posted by: JohnA Posted at: 2017-05-01T19:48:55.782Z Reads: 118

```
Looks like it will work
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-01T21:00:18.876Z Reads: 112

```
Looks good to me
Unplug the loop key when charging.
But you probably new that. 
Nice diagram btw.
```

---
## \#5 Posted by: mmaner Posted at: 2017-05-01T21:27:58.632Z Reads: 103

```
TO be safe, you need to isolate the electronics from the battery(s).  I woul dput an XT-90S loop key here...
<img src="/uploads/db1493/original/3X/a/b/abe58fe714c5b0e9b98abab3c5c0a6a768d5c587.jpg" width="465" height="500">
```

---
## \#6 Posted by: marcus Posted at: 2017-05-01T21:36:03.780Z Reads: 92

```
I was thinking the same thing...However, just to play devils advocate and learn, wouldn't the first xt90 loop key totally stop any electrical pulse to the VESC in the first place as the series bridge is disconnected? Therefore a second loop key would be redundant right?..
```

---
## \#7 Posted by: mmaner Posted at: 2017-05-01T21:38:57.749Z Reads: 87

```
Im not sure...You NEG leg will still be connected to battery 2 and the POS leg to battery 1, so technically if the series bridge is broken so should the flow of current, but batteries do weird spooky shit mate :).
```

---
## \#8 Posted by: marcus Posted at: 2017-05-01T21:44:49.077Z Reads: 83

```
that much is true....I was also wondering how charging might somehow affect the VESC but there is not finished circuit if the loop key were to be unplugged, so theoretically safe....idk why risk it thought on a expensive piece of hardware...im want simplicity yet safety.....
```

---
## \#9 Posted by: mmaner Posted at: 2017-05-01T22:55:14.810Z Reads: 73

```
[quote="marcus, post:8, topic:22161"]
want simplicity yet safety
[/quote]

I'm with you there.  I would use 2 keys just to be safe.
```

---
## \#10 Posted by: TheImmortalJew Posted at: 2017-05-01T23:15:12.584Z Reads: 69

```
I did exactly as your diagram describes. When my XT90S is in, board turns on and connects my batteries in series for 12s. When I unplug it, it turns the board off and separates the battery into 2 6S that I charge with 2 iMax B6 chargers. To make charging simpler, I wired my main + and - and the balance leads to a 15 pin VGA port. That leaves me with a 2 plug charging setup instead of 4 like in your diagram. I thought I might need a second XT90S before the VESC, but it's been working fine with only one between the 6S batteries.
```

---
## \#11 Posted by: Challlsss Posted at: 2017-05-02T19:39:29.502Z Reads: 64

```
Your diagram is fine. It will work. I would move the XT90 closer to the VESC this won't change anything about the circut _**but**_ when you are trying to solder and organize all your wires it will likely be easier if you connect your loop key near the VESC. 

Do you need to change anything? - NO
Can you optimize design by moving XT90? - YES
```

---
## \#12 Posted by: Maxid Posted at: 2017-05-02T20:52:41.419Z Reads: 60

```
how can he move the XT90? In this diagram the benefit is that charging as 5S becomes possible. That is why the loop key actualy connects the batteries in series and closes the circuit this way. Moving it closer to the VESC would mean that the batteries are permanently connected and can not be charged separately.

@marcus the diagram is a proven schematic and will work flawlessly. As usual though: You are playing with lithium batteries so be careful with what you do!
```

---
## \#13 Posted by: Challlsss Posted at: 2017-05-02T21:09:50.344Z Reads: 56

```
@Maxid It doesn't matter where the XT90 is because it will break the circuit either way. Near the VESC and where it is right now both achieve this.

<img src="/uploads/db1493/original/3X/9/b/9bd9b10daed90cfcb1ed4d9e39ea11b682f0bdae.png" width="477" height="500">'

Here is my diagram. It is a little easier to tell because I don't have the parallel batteries But the way that Marcus has his diagram is essentially the same (Ignoring the balance wires) as where I have circled in **red** and the way that is near the VESC is circled in **black**. Either way the loop key will break the cicut
```

---
## \#14 Posted by: Maxid Posted at: 2017-05-02T21:39:34.233Z Reads: 49

```
The loop key connects the batteries in series. If you leave them permanently connected and charge them in parallel on a dual charger guess what will happen...

Don't give advice like this to people with little experience. He found the right schematic for his use case.
```

---
## \#15 Posted by: Challlsss Posted at: 2017-05-03T13:01:27.796Z Reads: 41

```
Moving the loop key wouldn't permanently connect them though....
```

---
## \#16 Posted by: Smorto Posted at: 2017-05-03T13:02:27.445Z Reads: 41

```
No but it would make it so he can't discharge in series and then with the unplugging of one loop key charge the two batteries separately.
```

---
## \#17 Posted by: Challlsss Posted at: 2017-05-03T13:03:42.022Z Reads: 42

```
Based on my understanding of circuts that does not make sense to me. Can you elaborate further _why_ this would not allow for separate charging?
```

---
## \#18 Posted by: Maxid Posted at: 2017-05-03T13:06:08.002Z Reads: 43

```
the ground of the second pack is at the voltage level of the first pack's positive. the charger's ground is at 0V though. now guess what will happen if you connect the two grounds together.
```

---
## \#19 Posted by: Maxid Posted at: 2017-05-03T13:08:48.709Z Reads: 45

```
[quote="Challlsss, post:13, topic:22161, full:true"]

<img src="/uploads/db1493/original/3X/7/9/79fcca0646cb8900a805b70e088cdfa3586fdbe0.jpg" width="536" height="461">

If the loop key was moved to anywhere where I've circled in red it **would not break the circut** and would be useless.
[/quote]

that is wrong though
```

---
## \#20 Posted by: Challlsss Posted at: 2017-05-03T13:09:54.032Z Reads: 41

```
If I moved the loop key to any of those spots the circuit would not be broken, I would just take one battery out.
```

---
## \#21 Posted by: Maxid Posted at: 2017-05-03T13:10:30.235Z Reads: 33

```
what? no the batteries are in series!
```

---
## \#22 Posted by: Challlsss Posted at: 2017-05-03T13:11:25.578Z Reads: 36

```
not at those spots those are parallel connections between the 6s Batteries. Look closely at the image and where I've circled
```

---
## \#23 Posted by: Maxid Posted at: 2017-05-03T13:12:19.435Z Reads: 35

```
 the batteries are connected in series - that is the whole point of this setup.
```

---
## \#24 Posted by: Challlsss Posted at: 2017-05-03T13:16:30.501Z Reads: 36

```
aaaaaaaand the light has shined down and blessed @Challlsss With a lesson in READING SKILLS.
My stupid head has been looking at the 6S charger squares in the diagram and interpreting it as another 6s battery. IE I've been thinking about this as a 12S2P system this whole time.  My bad man, I can now understand why you thought I had a serious lack of understanding haha.
```

---
## \#25 Posted by: Challlsss Posted at: 2017-05-03T13:16:49.044Z Reads: 36

```
I will update my posts to remove incorrect info
```

---
## \#26 Posted by: Hummie Posted at: 2017-05-03T14:39:28.705Z Reads: 34

```
But if two seperate Chargers were used I don't think he would even need to remove the key and could leave it connected while charging. It would all still be in series but the chargers are only dealing with 6s still. No?
```

---
## \#27 Posted by: Challlsss Posted at: 2017-05-03T14:41:41.967Z Reads: 36

```
but then the VESC would have power running through it and the motor too so if you bumped your controller your board would fly across the room
```

---
## \#28 Posted by: Hummie Posted at: 2017-05-03T14:43:17.794Z Reads: 38

```
Yea if u use the transmitter. But assuming u don't do that I'd think charging would be fine.  Stylez?
```

---

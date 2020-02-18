# Mini Cruiser (Penny) 22&rdquo; &#124; TORQUE 75kv Hub &#124; Unknown Battery Config &#124; 18mph goal &#124; Ultra portable

### Replies: 8 Views: 1572

## \#1 Posted by: Atticus Posted at: 2016-10-04T23:18:58.429Z Reads: 252

```
My primary goal behind this board is for it to be travel safe (airplane), ultra portable (attached to my back on a motorcycle), 

**Airplane Concerns**
First off, I'm aware of the battery issues with airplanes. My goal there is to have my battery setup modular so I can easily separate it into distinct "batteries" that are under the 99Wh limit and be stored in lipo bags. So batteries like Zippy 6s 8000mAh are out.

**Speed & Range**
I do not need high speeds nor huge range. I'd be happy with 18mph max speed and 3-6 miles of range. I am going with hub motors because from what I've read it seems those are best if you plan on manually pushing the board on occasion, which I do intend to do. I want the powered mostly aspect for hills, both up and down (braking). But it would be nice to have a couple of miles of juice in there still.

**Budget**
My budget isn't a huge concern. I don't think I really need to spend over $1000 to achieve my end goal, but I'm willing to go up to that. I want the best solution to my needs possible, whether that's building a custom battery or buying pre-created packs. Though I probably won't be machining any parts, so I'm stuck with off the shelf there.

**Self**
5'11" & 165lbs

**Rough Build**
All of that being said, my current build looks something like:

* 22" Mini Cruiser Board (off brand penny) - 27cm x ~12cm usable space between the trucks.

* Longboard trucks for added stability at speed (current trucks get wobbly at ~16mph)

* TORQUE 75kv Hub motor (Not sure if 1 or 2 yet)

* VESC

* Unknown battery configuration (details below)

**Battery Details**
I'm not perfectly clear on exactly what battery specifications I'll need to reach my goal. Based on things I've seen around here, it seems like I need to be delivering 20-30C to each motor. If that is true then I most likely need to be doing 2p with 20C discharge batteries (if I do 2 motors). But then how much in series I need is unknown for me. I haven't been able to determine how to translate series quantity into speed, etc.

**Questions**
My 2 biggest questions right now are:

1. One motor or two? From other posts I've gathered that one motor usually tops out around ~12mph on average it seems, although that's been for geared, not hub. If that's true, I would want to do two, but I don't need all of that speed they are capable of.
2. What is the minimum battery configuration I can get away with? Is something like 8s2p, 16000mAh total, 40C discharge adequate? Will 8s give me enough? Do I need to go to 10 or 12? Alternatively, if I am using 1 motor, can I get away with 12s1p with a 20C discharge? I just haven't been able to get definitive answers on this. Is there some simple calculation I'm missing that would tell me exactly what I need based on my desires?

Thank you in advance for any/all assistance you can provide. I'm ultimately trying to get this board completely built in the next 3 weeks.

**Photos:**
Board:
https://images-na.ssl-images-amazon.com/images/I/61Mr3MFjCCL._SL1001_.jpg
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-04T23:23:35.275Z Reads: 232

```
I run single Sk3 192kv with 6s and i can do much more than 12mph. Im fairly lightweight (65kg) so i can go uphills and everything just fine too.
```

---
## \#3 Posted by: Spek Posted at: 2016-10-05T00:30:49.399Z Reads: 226

```
1 vs 2 motors **shouldn't** _(typo corrected)_ add speed. 2 motors is more torque, better breaks and less work/effort for motors. I've only ridden my dual and can say the torque is great at my 215lbs. 1 is probably fine for your weight depending get on the hills. I personally only ever had interest in dual. I've never read of anyone using 70kv motors. Also I'm fairly new to this and almost done with my first build so I'm sure others will have more knowledgeable answers

http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1
```

---
## \#4 Posted by: TarzanHBK Posted at: 2016-10-05T09:45:42.545Z Reads: 190

```
you mentioned you want to stay in that 99Wh limit. So with 6s: 
99Wh : 22,2V = 4,459AH
-> so you could use a 4500mah 6s battery maximum.

10s lipo: about 2600mah max
12s lipo: about 2200mah max
```

---
## \#5 Posted by: chinzw Posted at: 2016-10-05T17:23:41.505Z Reads: 164

```
[quote="Spek, post:3, topic:10650"]
1 vs 2 motors should add speed.
[/quote]

Nope, without accounting for efficiency and loses. 2x 200kv motors at 10s would give you 8400 RPM, which is the exact same as 1x 200kv
```

---
## \#6 Posted by: Spek Posted at: 2016-10-05T17:35:12.920Z Reads: 158

```
Stupid cell phone autocorrect. I meant to say "shouldn't"! Thank you for correcting me
```

---
## \#7 Posted by: Wubbalubbadubdub Posted at: 2017-04-24T20:59:04.549Z Reads: 108

```
How did this build work out? While I'm waiting for my new deck to arrive, I bolted my calipers onto my 22" penny and put my battery/bms/VESC/Bluetooth receiver in a duffel just to see if it would work.

I went two feet all of three times and thought I was about to die. maybe if I didn't have to hold the bag so close to the board on account of the short wires. Anyways I am curious how this worked out for you!
```

---
## \#8 Posted by: taity Posted at: 2017-05-16T01:50:12.883Z Reads: 84

```
I've done this build. Used a 260kv outrunner (single).vesc. 2 x zippy 5000mah batteries, just use connectors and separate them when you travel. I get 6-10mi range and cruise at about 18mph. Have had it up to 26 on a long flat run but anything over 20 is terrifying. Travelled with it to aus and the uk (living in NYC) and have over 200mi total on it so far. I'm heavier than you too
```

---

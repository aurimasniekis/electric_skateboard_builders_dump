# Upgrading my first build

### Replies: 18 Views: 367

## \#1 Posted by: TiMMaTTie Posted at: 2018-07-03T16:17:19.313Z Reads: 128

```
Hi there,

I have completed my first build. It was defintely meant as a first exploration, using an old skateboard and trying to keep costs down as much as possible. Furthermore I wanted to expirement a bit with 3D printing and electronics by making my own remote and battery enclosure. The board uses a Maytech vesc and 5065 236kv motor rated for 10s 60a max, powered by two 4s 5000mah lipos (25-35c) in series. I travel by train a lot and want to keep my board portable, so no need for crazy range and speed. I have done no exact measurements but range should be a little over 10km now, and due to the small board I have not actually reached top speed yet (one ebiker followed me once and told me he measured 30km/h but not too sure about that).

Time for upgrades! I plan to make a longboard with a few cm more length and carying handle. But more importantly I received a "broken" ebike battery and scavenged the cells (supposedly something wrong with electronics and hardly used yet). I am not a big fan of opening my enclosure every time and charging the lipos seperately, and want to build a proper pack with a BMS. I am still a poor student so trying to stay cheap!

TLDR: My questions:
1) The cells I have at hand are Panasonic NCR18650PF 2900mAh - 10A. I have 40 of these. Is it possible to find a cell arangement that achieves similar results to the lipo batteries without becoming more bulky and heavy? Or would it then be better to stick with lipo and add a BMS?
2) Would it be bad to get a cheap BMS and avoid discharging through the BMS? And can the charger be a cheap chinese 2A?

Please let me know if I left out information that should be taken into account for this decision!

![IMG-20180701-WA0017|690x345](upload://oZ7iJc6PH0ZYAdbMtTt5krVIPqN.jpeg)![IMG-20180701-WA0014|690x345](upload://9su1EwYw48aocOSa3tw9OOcTCTq.jpeg)![IMG-20180701-WA0012|250x500](upload://7OqIHePx6fqaToXn6G0ZZxDAQNV.jpeg)![IMG_20180703_174156|375x500](upload://uEsCmRPL9f7vxu6OebgFuqqmzhm.jpg)![IMG_20180703_174051|375x500](upload://lAtGWNk9K1Hs7GSECV5Y1H2LS7A.jpg)
```

---
## \#2 Posted by: Silent_bob52637 Posted at: 2018-07-04T09:05:05.960Z Reads: 88

```
A 10s4p would give you 11.6ah at 36v nominal
But as for space and actual layout i got no idea
```

---
## \#3 Posted by: TiMMaTTie Posted at: 2018-07-04T09:46:55.100Z Reads: 84

```
Yeah I am mostly worried at the discharge capacity of these cells, but I suppose I should measure what I'm actually drawing with my current setup
```

---
## \#4 Posted by: Silent_bob52637 Posted at: 2018-07-04T12:19:37.834Z Reads: 73

```
4p at 10a per cell would be 40a continous i believe maybe @longhairedboy or someone else with more knowledge than me  could chime in cuz im still learning
```

---
## \#5 Posted by: Silent_bob52637 Posted at: 2018-07-04T12:20:34.472Z Reads: 67

```
Also i quite like your remote do you have a guide or build log for the remote itself
```

---
## \#6 Posted by: Sn4pz Posted at: 2018-07-04T13:05:47.488Z Reads: 62

```
40a is plenty for a single motor setup, maybe program your vesc to output 35 batt max so you dont strain them too hard? Make sure all your welds are solid, and that youve either got thick or multiple (pure) nickel strips

lipos would almost certainly deliver more power though, as well as being a more compact and "simple" solution, but if youre looking at the total lifespan, the 18650 cells you have are the better bet. Make sure your lipos arent swelling, you dont want a fire x.x
```

---
## \#7 Posted by: bartroosen12 Posted at: 2018-07-04T13:14:25.969Z Reads: 59

```
Like sn4pz said, 40A is really enough for 1 motor.
And you will get a great range.
I have dual hubmotors and they only use 20A max and they are powerfull enough for me.
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-07-04T13:19:17.305Z Reads: 56

```
10s4p takes 130cm³ volume. 4p for a portable build seems big.
```

---
## \#9 Posted by: TiMMaTTie Posted at: 2018-07-04T13:23:22.131Z Reads: 56

```
Thanks, there is actually a lot to improve, I will share once I finish the second version. It will probably be similar to the other printed remotes though, just trying to make it as small as possible
```

---
## \#10 Posted by: TiMMaTTie Posted at: 2018-07-04T13:24:31.168Z Reads: 56

```
Thanks for the advice! Still have to find an actual welder but I will keep it in mind
```

---
## \#11 Posted by: TiMMaTTie Posted at: 2018-07-04T13:26:04.775Z Reads: 57

```
This is something I am worried about as well... I kind of need a few in parallel to up the current, but I don't care about long range too much and want to keep it light and small
```

---
## \#12 Posted by: TiMMaTTie Posted at: 2018-07-04T18:45:02.868Z Reads: 42

```
I'm considering the easy solution of adding a BMS to my current lipo setup, skip the discharging and set limits in the vesc. I realize that the charger needs cc/cv features, but how can you tell if a charger has those? Does this one have that?
https://www.banggood.com/33_6V-2A-Smart-Battery-Charger-For-8S-28_8V-29_6V-Li-ion-Li-Po-Battery-p-1111782.html?rmmds=search&cur_warehouse=CN
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-07-04T20:16:52.044Z Reads: 30

```
if you look for a li ion charger its what you get, just get the one with the right voltage. yeah lipo is just ez to do for small commuter. I mean there are small capacity 18650 which pack quite a punch.
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-07-04T20:17:38.541Z Reads: 28

```
that is an 8s charger. you need 10s charger.
```

---
## \#15 Posted by: sunnyD Posted at: 2018-07-04T20:44:49.551Z Reads: 21

```
I am a big fan of that remote. it combines the smaller size of a thumb wheel remote with the great trigger of the index or classic RC remote. my only question is how do you brake?
```

---
## \#16 Posted by: TiMMaTTie Posted at: 2018-07-04T21:09:22.048Z Reads: 21

```
Thanks for all the advice!
```

---
## \#17 Posted by: TiMMaTTie Posted at: 2018-07-04T21:12:11.821Z Reads: 22

```
Basically brakes are on by default with the trigger all the way forward by the spring. I have never used the thumb stuff but I suppose in "resting" position it doesn't brake nor accelerate? Could be a nice addition for the next version
```

---
## \#18 Posted by: sunnyD Posted at: 2018-07-04T21:13:34.854Z Reads: 20

```
Ah ok cool. Please keep me posted on this as I do like the design very much.
```

---

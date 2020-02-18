# BMS wiring correct?

### Replies: 23 Views: 490

## \#1 Posted by: seaborder Posted at: 2019-03-05T13:45:20.489Z Reads: 129

```
Hello guys :slight_smile:

ive got a  charge/discharge bms 12s 80a (http://www.batterysupports.com/44v-48v-504v-12s-80a-12x-36v-lithium-ion-lipolymer-battery-bms-p-392.html) so I am right now into connecting that whole thing. The balance wires are no problem. I watched a ton of videos and read much but I am still not quite sure. Ive made a photo of  like I think its correct but the cables which go to nothing are confusing me somehow. Maybe someone could help me a bit I would be more than thankful!!  No worries its just sticked together to show.
![bms|666x500](upload://vSLFVauolqF77XkngMa0ba95xuN.jpeg)
```

---
## \#2 Posted by: seaborder Posted at: 2019-03-05T14:27:32.751Z Reads: 115

```
@Andy87 helped me a bit now it looks like this :slight_smile:

So there is the negative and postive from the balance plug where they go? I think i have to skip the second postive of the second battery and the negative goes to b-? 

I will ad a switch before the vesc

![BMS21|375x500](upload://8lydiKzAOKGY10r6jrAt9TRLsQW.jpeg)
```

---
## \#3 Posted by: seaborder Posted at: 2019-03-05T22:59:25.055Z Reads: 83

```
![15518267409759026483451045700285|374x500](upload://7EqiZq9xLG8colaNUSaOvvpf9BN.jpeg)

Ok so the balance wires I ordered like this, i started measuring the pins and startet with pin 12 - into small positive balance plug at the postive side of the “positive” battery - 44v. Then I went through all and on the other battery “the minus one” which is in series I skipped the first and last pin because I assume they are conected anyways with the big wire. The rest I left like in my last photo.

I think I did it correct? :smiley:
```

---
## \#4 Posted by: b264 Posted at: 2019-03-05T23:06:37.080Z Reads: 73

```
Put a fuse on the charge port

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#5 Posted by: ryansinatra Posted at: 2019-03-05T23:11:24.754Z Reads: 71

```
I always see you mentioning the importance of putting a fuse on the charge port and I totally understand why, but how do you do it? Never wired a fuse before I'm sure it's simple but I'm a visual learner. Do you have a photo?
```

---
## \#6 Posted by: b264 Posted at: 2019-03-05T23:12:47.426Z Reads: 68

```
There are photos on my new build thread
```

---
## \#7 Posted by: ryansinatra Posted at: 2019-03-05T23:20:51.229Z Reads: 67

```
Cool! I'll check it out, thanks.
```

---
## \#8 Posted by: seaborder Posted at: 2019-03-06T00:14:51.970Z Reads: 63

```
![AASD|622x500](upload://ef4wRGhTRALVdp5mWdd9sJs2j1N.png)

 ![IMG_20190306_011822|374x500](upload://1wTHIMt6HfZOxORvW7ffAA2EpKo.jpeg) 

Thats how I would connect it. Hope you can see everything. Also a photo of the top of the bms (not connected to anything). 
I drawed no xt90 connections or sth like that.
I think its correct. But not sure
```

---
## \#9 Posted by: b264 Posted at: 2019-03-06T00:24:30.562Z Reads: 56

```
This doesn't have a B0 so you want B1 to be around 4V (relative to B-) and B2 to be around 8V etc all the way to B12 around 48V

B12 should be the same voltage as B+ and B1 should NOT be that same as B-

Make sure that's how it's wired up

I don't see any issues except no fuse on the charge port
```

---
## \#11 Posted by: seaborder Posted at: 2019-03-06T01:20:17.384Z Reads: 53

```
how do I check the voltages correct with the mulitmeter if the battery is in series :/ noob question but never used a multimeter before and I think i measered wrong
```

---
## \#12 Posted by: seaborder Posted at: 2019-03-06T09:55:10.988Z Reads: 48

```
https://www.electric-skateboard.builders/t/noob-question-thread-ask-your-questions-here/9559/4945?u=seaborder
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-03-06T10:16:28.714Z Reads: 45

```
http://i1098.photobucket.com/albums/g378/lilianleung/LOGO%20Connecting%20Chart.jpg

You have two 6s batteries, let's call them 1 and 2. Let's say all your cells are exactly at storage charge, 3.7v. Let's also say that your pack negative (ground, 0v) is the negative on 1. The positive on 1 goes to the negative on 2, and then the positive on 2 is your pack positive (+44.4v.)

 Each of your 6s batteries has 7 balance wires. One connected to negative, one to positive, and one in between each pair of cells. Since you have two of these in series, then the middle wires are redundant (the positive-most balance wire on 1 is the same as the negative-most wire on 2.) 

After you take this into account, you have a total of 13 balance wires for the pack. One to negative (ground, 0v), and one to positive (44.4v), and one between each pair of cells.

With that BMS, the wire that goes to the spot marked 1 on the connector is the **second** balance wire (measuring from ground, 0v, it will be 3.7v.) position 2 gets the **third** wire (measuring from ground, it will show 8.4v.) 

Repeat this until you get to the end, where the 12th position gets the **thirteenth** balance wire (44.4v measuring from ground).
```

---
## \#14 Posted by: seaborder Posted at: 2019-03-06T10:29:18.810Z Reads: 40

```
this helped a lot thanks man ♥️♥️
```

---
## \#15 Posted by: seaborder Posted at: 2019-03-06T10:31:47.753Z Reads: 43

```
for the fuse @b264 said. Just put it at the p or n at the wire of the charging port ? doesent matter, does it?
```

---
## \#16 Posted by: seaborder Posted at: 2019-03-06T12:26:19.488Z Reads: 39

```
Ok I still dont get sth.

The side where B- goes into the battery at the outside is supposed to start with 3.8v at the balance plug according to the plan. But I already have the 44v up there. On the other battery where the outside is positive I have on the 2nd pin of the balance plug after the red cable 3.8v. But according to the plan should be 3.8v where the negative b- come in. Or does it really matter as long as I measure? I hope Iam not annoying already. But really want to learn that and not connect anything what blows at the end.

![48|666x500](upload://iaTDE9ZQbEJPxQumSFitDA9YSG8.jpeg)
```

---
## \#17 Posted by: Jumpman Posted at: 2019-03-06T12:38:45.417Z Reads: 36

```
I think you are measuring backwards.  The black probe should be on B- and you should measure by moving the other probe.

B- is your “zero”, and each balance lead should read progressively higher from there.
```

---
## \#18 Posted by: seaborder Posted at: 2019-03-06T12:40:07.185Z Reads: 38

```
Jeah @Andy87 told me too. Now it makes sence 😅😅
```

---
## \#19 Posted by: b264 Posted at: 2019-03-06T21:01:12.464Z Reads: 35

```
Yes, either one.  I put it on the negative so it's easy.  If you put everything on the negative then you know all the positives for everything just connect together.  Less complicated.
```

---
## \#20 Posted by: seaborder Posted at: 2019-03-07T21:06:40.243Z Reads: 25

```
![IMG_20190307_210918|374x500](upload://fdLLRNiyXy1TCn3pBICWD3nU6CL.jpeg)

charge port is not soldered but the big wires are ok so, arent they? Watched the schematic and everything should be correct I think. Maybe someone can take a look

lipo conects at the right xt90, vesc at the left one
```

---
## \#21 Posted by: b264 Posted at: 2019-03-07T22:28:40.489Z Reads: 24

```
You'll need another small red wire coming off that big one for the charge port.  I can't see the "B-" and "P-" labels so I can't confirm that is correct

Make sure B1 is about 4V more than B- and B2 is about 4V more than B1 and B3 is about 4V more than B2... etc
```

---
## \#22 Posted by: seaborder Posted at: 2019-03-07T22:36:32.286Z Reads: 23

```
yeah charge plug is not connected ill do it now. Thats no problem. P- is the left b- the right. Iam pretty sure it should be alright. :) Thanks for taking look
```

---
## \#23 Posted by: b264 Posted at: 2019-03-07T22:37:49.158Z Reads: 23

```
I don't see any issues then :slight_smile:
```

---
## \#24 Posted by: seaborder Posted at: 2019-03-08T12:40:46.890Z Reads: 18

```
I just connected everything an man Good News, everything is working. YEAHHHHH. Thanks to you guys for helping me and somehow Iam a little bit proud to myself I dont know why but yeahhh man!!

bye bye Imax balance charger hahqhq 

♥️♥️🤘😀😀
```

---

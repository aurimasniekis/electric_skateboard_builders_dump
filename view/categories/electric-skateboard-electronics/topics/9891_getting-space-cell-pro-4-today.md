# Getting Space Cell Pro 4 today!

### Replies: 17 Views: 1497

## \#1 Posted by: jesser722 Posted at: 2016-09-20T15:33:25.106Z Reads: 186

```
The Space Cell Pro 4 arrived today and I was wondering what are the settings I need to have on my vesc? I am planning on doing a comprehensive review along with unboxing. I haven't seen like any videos about it online so look forward to that!

Thanks,
Jesse
```

---
## \#2 Posted by: Jinra Posted at: 2016-09-20T15:35:22.565Z Reads: 187

```
I use 33v/30v battery cutoff start/end and 40A (per VESC) battery max for 80A total. Other settings depends on your other parts.
```

---
## \#3 Posted by: jesser722 Posted at: 2016-09-20T15:36:43.772Z Reads: 181

```
Any other tips when setting it up/ putting it on the board?
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-20T15:37:31.981Z Reads: 176

```
[quote="Jinra, post:2, topic:9891, full:true"]
I use 33v/30v battery cutoff start/end and 40A (per VESC) battery max for 80A total. Other settings depends on your other parts.
[/quote]
Doesn't the SP4 come with a 40a fuse?
```

---
## \#5 Posted by: Jinra Posted at: 2016-09-20T15:40:43.830Z Reads: 165

```
It does, but it's nice to have the power on demand. A 40A fuse wont necessary blow at 40A or even higher than 40A, depends on time/temperature as well as current. Some people say 40A is sufficient for a pack like this, but I disagree and have the wounds to prove it. I'd personally replace it with a bigger 60-80A fuse, but there's barely any space in the enclosure as it is, or remove the fuse altogether if you want to risk it, which is what I've done.

That said, I was using this setting for weeks without ever blowing the fuse. It was only when I pushed the board hard, by 0-100 acceleration that it blew.
```

---
## \#6 Posted by: Tarzan Posted at: 2016-09-20T21:18:15.926Z Reads: 128

```
I read in another thread that the new space cells come with a bypassed bms for discharging.
I'm sure Jason proved it, but it was a pro3.
Will look if I can find it.
```

---
## \#7 Posted by: jesser722 Posted at: 2016-09-20T22:13:51.441Z Reads: 116

```
What settings do I use if I want to use my winning remote?
```

---
## \#8 Posted by: lospollos Posted at: 2016-09-20T22:17:44.334Z Reads: 114

```
Check this out https://www.youtube.com/watch?v=OtuofrQr3F8
```

---
## \#9 Posted by: Jinra Posted at: 2016-09-20T22:49:29.145Z Reads: 110

```
it does, but has a 40a fuse.
```

---
## \#10 Posted by: jesser722 Posted at: 2016-09-21T18:42:25.586Z Reads: 94

```
I have a mono drive and I am having trouble going up hills that I could go up easy with my hobby king esc. I didn't change the battery max because it is already set at 40A. Any ideas on what could be the problem?

Thanks,
```

---
## \#11 Posted by: Kaden56 Posted at: 2016-10-27T06:00:40.742Z Reads: 77

```
I'm contemplating getting a space cell 4. Is the fuse easy to replace if I blow it? Are you happy with the pack? I feel like it's the biggest bang for your buck for a battery pack from what I've seen.
```

---
## \#12 Posted by: E-Boarding Posted at: 2016-10-27T07:14:11.619Z Reads: 77

```
yes, you can easily replace the fuse, I got 2 spare ones as well.

I had only one problem so far: the cable on the xt60 came lose and I had to resolder it, not a big deal
```

---
## \#13 Posted by: Jinra Posted at: 2016-10-27T14:20:09.387Z Reads: 71

```
I like it so far. The fuse is easy to replace, but I decided to cut mine off since the amperage is so low. The fuse blew on my while riding normally. I may throw a bigger fuse on there if i find one suitable enough.
```

---
## \#14 Posted by: Kaden56 Posted at: 2016-10-28T16:29:32.774Z Reads: 58

```
So the power switch and bms must be rated higher than 40amps if you have been fine without using the fuse. That's one thing I was worried about. Do you know how hard you have pushed the amps on your board? Would you suggest a 60amp fuse if I was to replace it?
```

---
## \#15 Posted by: Jinra Posted at: 2016-10-28T16:33:09.825Z Reads: 59

```
yea, you should be fine with a 60A fuse, though, if it's the same size, 80 would be safe. It's very hard to find a small fuse rated for 60+ amps though. Power switch doesn't have to be rated for any current if you're using an e-switch like on the SCP3/4. I've climbed very steep hills with the stock 40A fuse without blowing. It was only when I did a drag race with a fellow esk8er that it blew.
```

---
## \#16 Posted by: Kaden56 Posted at: 2016-10-29T06:14:31.011Z Reads: 54

```
That's good to hear! The more and more I thought about doing a 10s1p set up with two 10000mah lipos the more of a head ache I got with how much care goes into it. And after the switch, bms, lipos, charger, charging port, etc. it adds up to the point that I was within $100 of the space pro 4 and I reasoned that $100 is certainly worth a plug and play option that will certainly last longer than a couple cheap lipos. Plus it comes with a good looking enclosure for my first build. Almost feel like I'm cheating in the DIY aspect of things! haha but it's so worth it. I think the only reason to go with a cheaper lipo option is if you are just doing a 6s set up with on 5000mah battery and you get a cheap balance charger. But as soon as you go up to around 10s or 12s and you also want range, it seems like your lipo setup gets a little hairy. Thanks for the feedback on the pack I appreciate your expertise.
```

---
## \#17 Posted by: Jinra Posted at: 2016-10-29T06:31:03.153Z Reads: 51

```
Yea, I definitely recommend the space cell. Having a pre-made battery built into an enclosure definitely makes everything a lot easier. I built my own battery on my 2nd built and got an empty enclosure. It was 100% more work than my first build with the SCP4.
```

---

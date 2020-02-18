# Can someone help me set up this bms?

### Replies: 18 Views: 787

## \#1 Posted by: abenny Posted at: 2018-07-18T18:41:23.539Z Reads: 107

```
hey guys; so i bought this BMS from aliexpress; it was  listed as a 10s bms and i inquired to the seller about if they had an 8s bms. they told me they could modify the board and make it 8s for me. so i ordered it 3-4 weeks ago and it came in today and im wanting to get it set up. only thing is the instructions are all in chinese and i've only set up a bms once before (with the help of a very detailed thread), so im not sure how to install it. It is 60A charge and discharge, so id like to install it for both. if anyone could help me it'd be great;y appreciated.
![20180718_143806|243x500](upload://cceVWlvYANyXtJe03btWyQnjZHu.jpg)![20180718_143759|243x500](upload://ijQNyWsW7Tfs9oqAlGbGxe279TH.jpg)![20180718_143749|243x500](upload://d8ObNknVDwQTqYdET7R2y1XfVI6.jpg)
```

---
## \#2 Posted by: abenny Posted at: 2018-07-18T21:09:33.829Z Reads: 93

```
okay so ive found this on their seller page; this should apply to mine since charge/discharge is common port. can someone verify that im interpreting this correctly? ![image|690x310](upload://48dXYaBxgmtgKa6UoUkzH7nB3qA.jpg)

i think i need to connect the balance leads from the right battery in order of ground first, then the 4 positive wires; and for the left battery i need to omit the ground and just put the 4 positive on the balance connector. and then B- gets connected to the main ground on the right battery, and P- and the positive lead from the left battery go to make my main + and - .  and from there i can just wire in my 2.1x5.5 DC jack into the main + and - leads?
can someone please verify this for me? id be very appreciative.

![20180718_170503|243x500](upload://8WnL4iDjRwhNMS4n2ct496RXJ2D.jpg)![20180718_170509|243x500](upload://h7Q3rcgUny8buTwpr8ZkLLkDPpA.jpg)![20180718_170512|243x500](upload://A3v7uhLTbQfNNY1LPI965hmbpkm.jpg)
```

---
## \#3 Posted by: Silverline Posted at: 2018-07-18T21:28:38.095Z Reads: 72

```
Before you do anything. Do you have a multimeter ? This is very essential, when DIY
```

---
## \#4 Posted by: abenny Posted at: 2018-07-18T21:32:41.786Z Reads: 72

```
i do have a multimeter
```

---
## \#5 Posted by: laurnts Posted at: 2018-07-18T21:33:06.324Z Reads: 73

```
You need to join the balance lead of the positive (the last red cable of the group) into the negative of the other balance lead.
```

---
## \#6 Posted by: abenny Posted at: 2018-07-18T21:34:53.480Z Reads: 72

```
can you explain further? im not 100% sure what you mean
```

---
## \#7 Posted by: laurnts Posted at: 2018-07-18T21:37:55.790Z Reads: 71

```
You need to series the balance lead as well, in your first picture you still didn't complete them yet. This BMS works quite similar to other BMS'es including the Bestech ones.
```

---
## \#8 Posted by: abenny Posted at: 2018-07-18T21:40:13.275Z Reads: 71

```
how certain of this are you? i was roughly following this thread https://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122
which is the exact same BMS i used previously so i basically followed it step for step and i dont think i ever connected the balance leads in series too
```

---
## \#9 Posted by: Silverline Posted at: 2018-07-18T21:43:43.101Z Reads: 68

```
Maybe this video can help you out...

https://youtu.be/_yrYG5skwvs
```

---
## \#10 Posted by: laurnts Posted at: 2018-07-18T21:48:42.053Z Reads: 67

```
Yes I am certain 100%. You already connected the main in series, connecting the balance leads won't short it. If you want to be sure 100%, check it with multimeter. You technically don't have to connect them either, it still will work, just abit weird to have 1 balance lead cable dangling around.

The theory of BMS is like this. You run 8S, so there will be 9 channels in the port. 8 Positives, 1 negative. 1s (or channel 1), should be roughly 3.6v - 4.2v. This value should increase for the next s channels up to the end voltage of the 8s. At least thats the basic.
```

---
## \#11 Posted by: abenny Posted at: 2018-07-18T21:48:54.069Z Reads: 64

```
im not sure this is applicable to my bms; his 10s bms has 10 leads where my 8s bms has 9 leads; is that video for a bypass discharge bms?
```

---
## \#12 Posted by: laurnts Posted at: 2018-07-18T21:53:53.633Z Reads: 62

```
![3eaae6eea54c416a5e206f85c0afc5b10f5aeb4f_1_243x500|243x500](upload://z4DSM2cI9o5fJK5NyZBKZoPNPbZ.jpg)

Sorry, its not P- but B-
```

---
## \#13 Posted by: Silverline Posted at: 2018-07-18T21:56:44.584Z Reads: 53

```
It's because yours also need the main minus (B-) together with All the ballance leads from the cell groups
```

---
## \#14 Posted by: abenny Posted at: 2018-07-18T22:06:58.629Z Reads: 55

```
this is what ive done based on what i interpreted from the diagram...
![20180718_180439|243x500](upload://A8CwxvoU9PgkKJaAWZOMlpnVsz9.jpg)
i connected the main cell negative first, then the first cells with the first lipo pack, and then the second one i connected the 4 positive cells.. the one loose wire is the negative from the second lipo which i believe i dont need  so i can snip that? essentially all the red balance leads on the BMS connector are positive while the one black is the main negative lead.
then  B- connects to the main negative lead of the cell pack  and im done?
or is this completely wrong..i haven't connected anything up yet, i want to be sure before i do
```

---
## \#15 Posted by: abenny Posted at: 2018-07-18T23:26:34.124Z Reads: 45

```
okay so ive connected the balance leads to the BMS in the way its set up in post#14, and nothing shorted so that is good. i connected B- to the main negative lead and nothing shorted so thats good too. I checked the voltage from the main negative (P-) on the bms and the main positive and it reads as it should for an 8s battery. now do i just connect my charging port to the P- and the main positive?
![20180718_192420|243x500](upload://7MIYvbmhWJcyFGgWJlJsYZhPrXo.jpg)
```

---
## \#16 Posted by: abenny Posted at: 2018-07-19T05:42:01.521Z Reads: 39

```
i made a rough diagram of what i've done/intend to do.. i haven't yet hooked up the charging port but i will do that friday, hoping someone can confirm my diagram
![Untitled|690x388](upload://1NlV5rV47YGBHqGYhrhrO9gUA4v.jpg)
```

---
## \#17 Posted by: laurnts Posted at: 2018-07-19T13:08:49.492Z Reads: 31

```
Correct. Your diagram and picture is indeed correct.
If you want to connect the loose black wire (I dont like the fact about dangling cable as they normally are unprotected with sleve and can cause short), you can just find the other red cable with the same voltage with your multimeter.
```

---
## \#18 Posted by: abenny Posted at: 2018-07-19T13:21:04.887Z Reads: 31

```
thanks for the clarification...i felt like it was correct but didn't wanna burn the house down...but as you said that loose wire may or may not be connected? so long as i take care of it? (ie. insulation, cutting it super short, connecting it in series like you said etc).
thanks!
```

---

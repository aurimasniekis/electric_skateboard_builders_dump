# Determining belt length

### Replies: 12 Views: 1119

## \#1 Posted by: Schulerbible Posted at: 2018-03-16T22:57:19.565Z Reads: 193

```
Hi, Please apologize the stupid question, but what's the correct way to determine the belt length WITH an IDLER pulley. I measured the inner length of the belt band (see below) but I'm not sure if this is right!?

![image|690x439](upload://pVwTPUhZ7cWPbMN6DEFYpMFIuvg.png)
```

---
## \#2 Posted by: ZackoryCramer Posted at: 2018-03-16T22:59:21.830Z Reads: 188

```
Seems legit.
```

---
## \#3 Posted by: Idle Posted at: 2018-03-16T23:09:35.340Z Reads: 186

```
Got to say, 
That's awesome...

The Idler prolly only adds an additional ~5mm to your belt length in its loosest position.

Is that about what your math shows?
```

---
## \#4 Posted by: Schulerbible Posted at: 2018-03-16T23:51:51.402Z Reads: 172

```
Nah, yeah somehow. The measurement just shows where I measure the belt length. I am not sure if measuring the belt length on the inner side is correct. I would assume the neutral axis is what I have to take into account. 

![image|480x480](upload://biLFKBKHeKEJvYEiIuuTW46rmtS.png)
(Source: http://www.custompartnet.com/wu/sheet-metal-forming)
```

---
## \#5 Posted by: Deckoz Posted at: 2018-03-17T00:48:10.699Z Reads: 149

```
Count the teeth multiply by 5... Belt length.
```

---
## \#6 Posted by: Schulerbible Posted at: 2018-03-17T00:54:06.753Z Reads: 145

```
The issue is, I set the amount of teeth in the model. So, the difference between 62 and 63 for example is so minimal but gives you a different belt length. I need to know where the band length is measured and then I'll apply the corresponding number of teeth which you can figure out e.g. here:

https://www.bbman.com/belt-length-calculator/
```

---
## \#7 Posted by: Deckoz Posted at: 2018-03-17T00:56:16.924Z Reads: 145

```
The total length of a tooth including space between teeth is 5mm

Meaning a 2 tooth belt is 10mm. A 40 tooth belt is 200mm. Model your belt like this? From the inner face of the belt at the surface of the gaps is where it's measured
```

---
## \#8 Posted by: Schulerbible Posted at: 2018-03-17T00:58:07.937Z Reads: 138

```
Yeah, maybe I could do this. Just need some restructuring.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-03-17T01:01:14.360Z Reads: 135

```
Measure from this surface marked in pink.. sorry for the shitty finger line

![received_10160072308245521|690x439](upload://ef8aPKhHrCe0q92DdHjkK4x4BYB.jpeg)
```

---
## \#10 Posted by: Schulerbible Posted at: 2018-03-17T01:08:23.122Z Reads: 130

```
This is what I did so far ...
```

---
## \#11 Posted by: Schulerbible Posted at: 2018-03-17T02:18:25.615Z Reads: 124

```
Ok, I think I found it. The belt length is referred to the pitch length (sort of neutral axis) and not to the inner belt length. That's why I had some discrepancies in the model.
![image|690x363](upload://bJ22bjpejsfaE4HD0x6dd6ecyXn.png)

![image|529x500](upload://4qD8ReoJGq0g2nIl2XUMldupo2N.jpg)
```

---
## \#12 Posted by: Schulerbible Posted at: 2018-03-17T03:11:55.551Z Reads: 112

```
Fits now :) 

![image|628x500](upload://r1LuCbvekKr2jJYc0W7cvrq45eh.jpg)
```

---

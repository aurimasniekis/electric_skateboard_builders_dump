# Charging battery while ESC connected at 21V? Opinions

### Replies: 14 Views: 1179

## \#1 Posted by: PXSS Posted at: 2017-01-02T00:57:13.655Z Reads: 92

```
Hey,
So I want to have 2 5S4P packs wired in series to operate the board and then wired in parallel to charge the battery.

So what I had thought of was to have my anti-spark switch between the 2 packs, to disconnect the series connection for charging and connecting the two packs in parallel.

Diagrams below...
<img src="/uploads/db1493/original/3X/e/9/e9011e1efc0141fdbc93f175a251a0ed1b0de0a4.JPG" width="666" height="500">

My question is, is it ok to charge while the ESC is on at 18-21v or should I have a second loop key to disconnect the esc while charging. Can I set any settings on the ESC to make it safe (low voltage cutoff?)

The reason I want to charge like this is because I only have 8S balance chargers and my BMS/Charger is not scheduled to arrive until mid January...
```

---
## \#2 Posted by: PXSS Posted at: 2017-01-02T02:51:17.743Z Reads: 70

```
@chaka, @JLabs, @psychotiller, @barajabali 
You guys are pretty savvy, any input?
```

---
## \#3 Posted by: psychotiller Posted at: 2017-01-02T03:14:37.065Z Reads: 66

```
The esc doesn't have any way to offer any input to charging..I honestly wouldn't do what you're trying to do.
If you have an 8s balance charger you can charge one 5s side at a time.
```

---
## \#4 Posted by: PXSS Posted at: 2017-01-02T03:16:43.838Z Reads: 65

```
Not sure I follow. I would be charging with a balance charger. Thing is, I would connect the packs in parallel to charge while the ESC is connected (so I don't have to open the enclosure...) and it would see ~21v while charging.
```

---
## \#5 Posted by: psychotiller Posted at: 2017-01-02T03:19:56.485Z Reads: 61

```
The esc isn't a factor as long as you have a fail safe set in the receiver so you're board doesn't take off on you
```

---
## \#6 Posted by: PXSS Posted at: 2017-01-02T03:24:05.364Z Reads: 53

```
If I set my low voltage cutoff in the setup as 28V, that should not be possible correct? 

I just don't want to fry the thing. Lol
```

---
## \#7 Posted by: psychotiller Posted at: 2017-01-02T03:27:02.386Z Reads: 48

```
That's what I'm trying to explain to you . Your esc. Isn't part of the charge system. Only part of the discharge system.
```

---
## \#8 Posted by: PXSS Posted at: 2017-01-02T03:34:51.719Z Reads: 47

```
But the ESC is plugged in in the charge system, how is it a no factor? Is it because of the failsafe on the receiver?
```

---
## \#9 Posted by: psychotiller Posted at: 2017-01-02T03:46:22.123Z Reads: 48

```
No it's not. Why would it be? It should just be plugged to the battery right?
```

---
## \#10 Posted by: psychotiller Posted at: 2017-01-02T03:52:11.327Z Reads: 48

```
Ok. I see. The problem is you have your loop key in the wrong spot. It should be in either the red or the black wire right before the esc.
```

---
## \#11 Posted by: PXSS Posted at: 2017-01-02T05:28:29.309Z Reads: 46

```
Yes but then when I remove the loop key, the pack is still a 10S pack which is why I placed it where I did. 

The functional diagram is the one on the bottom right... I can add a second loop key but it's what I was trying to avoid.
```

---
## \#12 Posted by: psychotiller Posted at: 2017-01-02T06:46:53.119Z Reads: 42

```
Ok, it works with the second loop key :slight_smile:
```

---
## \#13 Posted by: oripaamoni Posted at: 2017-01-03T19:43:36.284Z Reads: 23

```


I was battling with the same decision. I ended up just adding a second loopkey to be safe. I used an xt90 antispark for the esc loop key, then a male xt60 for the series connector  and female xt60 for the second charge connector, at least that way it can only plug in one way.
```

---
## \#14 Posted by: PXSS Posted at: 2017-01-03T19:52:51.736Z Reads: 21

```
I did similar. Will post pics later
```

---

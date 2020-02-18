# Will this work?

### Replies: 23 Views: 953

## \#1 Posted by: capfirepants Posted at: 2017-03-28T09:37:35.935Z Reads: 118

```
Redoing my Build right now and want to do electronics correctly.
Will this setup (cabeling) work? Especially the green highlighted cable near the batteries and the anti spark switch. The Yellow Boxes are XT90 connectors, the oney at the sides will be used as charging ports and the orange connecter is the anti-spark switch. Only 1 battery will be charged at the same time.
<img src="/uploads/db1493/original/3X/0/8/081adae17600d47ecdadf6952f532318ff37d28e.png" width="690" height="345">
```

---
## \#2 Posted by: laurnts Posted at: 2017-03-28T09:56:32.692Z Reads: 102

```
Seems to be ok for me. but if you want to be very sure, please buy / borrow a multimeter to avoid shorts.
```

---
## \#3 Posted by: kovjanos Posted at: 2017-03-28T12:05:03.845Z Reads: 94

```
anti spark is ok.

RE: charging ports: would you charge the batts one-by-one, independently? e.g. after disconnecting the others' internal XT90s? If yes, it's OK.
```

---
## \#4 Posted by: capfirepants Posted at: 2017-03-28T12:07:45.671Z Reads: 89

```
I would like to charge them seperatly, yes, but not with any disconnecting internally. Eg. I plug in cable at B1 charging port and charge B1, when I'm done I do the same for B2 etc. If the Anti-Spark isn't connected I assume the electrical circuit is not closed?
```

---
## \#5 Posted by: laurnts Posted at: 2017-03-28T12:10:32.679Z Reads: 81

```
yes its not closed.
```

---
## \#6 Posted by: kovjanos Posted at: 2017-03-28T12:13:06.692Z Reads: 68

```
No it won't work. Charging B1 you still have the loop via B3-B4 and - which is bad - a reverse B2.
```

---
## \#7 Posted by: capfirepants Posted at: 2017-03-28T12:21:23.881Z Reads: 63

```
Because the batteries on the right are parallel to the ones on the left?
```

---
## \#8 Posted by: kovjanos Posted at: 2017-03-28T12:23:46.739Z Reads: 63

```
yep. you would need to detach B2-internal (plus charging one at a time).
See how the B2 is bad:
<img src="/uploads/db1493/original/3X/5/8/585c0c7a040ceb3d2b408b474ab7cb70e1eda1f7.png" width="663" height="425">
```

---
## \#9 Posted by: capfirepants Posted at: 2017-03-28T12:30:10.974Z Reads: 59

```
I see. Shit. Any Idea on how to do that? If I use 2 Anti-Spark switches like this? Pretty shit though... Any better solution?
<img src="/uploads/db1493/original/3X/c/d/cdf855de9f957e558a060a1abe8846d82ba2523e.png" width="690" height="384">
```

---
## \#10 Posted by: kovjanos Posted at: 2017-03-28T12:43:04.127Z Reads: 49

```
any reason not making 2 in parallel first and then series?
anyway: I would keep the antispark also on the orig. position. first you would need to get the batteries connected for the balancing current just in case if those are not eq charged.
```

---
## \#11 Posted by: capfirepants Posted at: 2017-03-28T13:18:06.052Z Reads: 45

```
No, no reason not to. Would that change my situation? I'm having a few problems wraping my head around this...
```

---
## \#12 Posted by: kovjanos Posted at: 2017-03-28T13:36:57.427Z Reads: 41

```
well, at least if those are pll and fixed, you can charge them in one step, plus there would be no worries about the balancing current. There would be another challenges like keep them balanced, etc. what type of batts are we talking about? any bms on pack level?
```

---
## \#13 Posted by: capfirepants Posted at: 2017-03-28T13:39:01.729Z Reads: 40

```
The batteries are Zippy Flightmax 5s1P 8000mah https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html
They are balance charged on a per-pack level and I would like to change them balanced.
```

---
## \#14 Posted by: laurnts Posted at: 2017-03-28T13:42:11.938Z Reads: 40

```
Ohh sorry. I see the error in the drawing. I didn't notice the poles. lol I took back my comment.

To be honest I had this setup earlier.
The easiest way would be to just use the balance plug to charge.

5s1p means there are 6 ports on the balance side. You just need to parallel the outer red cable and the outer black cable to an XT60. If you do this, your balance charger would accept to charge. Also you shouldn't get any shorts.
```

---
## \#15 Posted by: kovjanos Posted at: 2017-03-28T13:51:37.246Z Reads: 39

```
Be sure to have not only the B1-B2 (and B3-B4) batts parallel connected but also the balance plugs (green on the pic) for those parallel connected (Y cable) inside the box!! 
So at the end you will have one charge plug and one balance charge port for B1-B2 and another charge plug and balance port for B3-B4.

<img src="/uploads/db1493/original/3X/7/6/76ff8810be2fd3baf6300fe517d39f8b8bf37641.png" width="493" height="500">
```

---
## \#16 Posted by: capfirepants Posted at: 2017-03-28T13:54:56.713Z Reads: 34

```
Ah, that would work. Problem is that my charger only supports up to 6s batteries, I would then have 10s though... I have an imaxb6.
```

---
## \#17 Posted by: kovjanos Posted at: 2017-03-28T13:59:34.747Z Reads: 35

```
B1-B2 are in parallel - if they are 5S - 5S and in parallel: they behave as a single 5S. 

Be careful! you are still not allowed to charged them at the same time!  
I mean 
  - [B1-B2] will be charged the same time from a single socket (and balancing port) 
  - [B3-B4] will be charged the same time from another single socket (and balancing port)
  - but you can't use the two charging sockets (and ports) the same time!
```

---
## \#18 Posted by: capfirepants Posted at: 2017-03-28T14:16:34.987Z Reads: 35

```
I see. The problem is, if I charge [b1 - b2] like that, I can't use the balanced connector that comes with each battery pack.
```

---
## \#19 Posted by: kovjanos Posted at: 2017-03-28T14:25:32.780Z Reads: 39

```
hope this is more clear
All you need is: 2x JST-XH Parallel Balance Lead 5S 250mm (2xJST-XH)
https://hobbyking.com/en_us/jst-xh-parallel-balance-lead-5s-250mm-2xjst-xh.html

<img src="/uploads/db1493/original/3X/3/5/35ae5a26e6730b2ec1addb018d7a5c17b85e646f.png" width="405" height="499">
```

---
## \#20 Posted by: capfirepants Posted at: 2017-03-28T14:57:02.289Z Reads: 39

```
Ah thank you, I understand now. 

I have a few more questions:
1) What happens if cell 1 from B1 is at 3.5v and cell 1 from B2 ist at 3.9v? How do they get Balanced?
2) Where do I put the Anti-Spark in this setup?
3) Where exactly do I connect the main charging pins from the Charger to Charge [B1 - B2] and [B3 - B4]?

Thanks a lot for your help!!
```

---
## \#21 Posted by: kovjanos Posted at: 2017-03-28T15:12:54.663Z Reads: 39

```
1: Be sure B1 and B2 (and of course B3 and B4) are charged and balanced exactly to the same level before configuring the above setup!
If it's set up, then it won't be possible as B1 balance port is pll connected with B2 balance port, Cell-1/B1 and Cell-1/B2 are pll, so they will always stay on the same charge level...

2: the orange box

3: use the green circled output. it has the main charge outlets (+ and -) and the 5S balance lead. - for both [B1-B2] and [B3-B4]. Just don't charge the [B1-B2]  and  [B3-B4]  the same time

let me know if it's not clear!
```

---
## \#22 Posted by: capfirepants Posted at: 2017-03-28T16:40:15.148Z Reads: 28

```
Ah, so if B1 would decharge faster (due to slight difference in internal resistance) then it would compensate with B2 over the Parallell charging port? 

So in that case only 1 Anti-Spark-Switch. Is the battery configuration still 10s then?

Luckily, I can't charge [B1 - B2] and [B3 - B4] at the same time 'cause my charger only has 1 Output :slight_smile:

Thanks a lot for your help.
```

---
## \#23 Posted by: kovjanos Posted at: 2017-03-28T16:43:14.674Z Reads: 26

```
Yes, cells in the same position(only bw B1-B2 and B3-B4) will be on the same level thanks to the balance ports pll conncetion

Yes, your VESCs will see it as a 10S2P:

  (  ( 5S[1P]  +P+  5S[1P] )  +S+ ( 5S[1P]  +P+  5S[1P] ) ) = ( 5S2P +S+ 5S2P ) = 10S2P
```

---

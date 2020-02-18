# DIY 10s battery help

### Replies: 10 Views: 1085

## \#1 Posted by: toma Posted at: 2017-05-13T22:18:47.057Z Reads: 104

```
Hey Everyone,

I'm looking to build a 10s battery pack out of nokia bp-4l cellphone batteries. 
I've got about 400 of these batteries, all brand new, albeit a bit old. they are 1500mah each.
http://www.cpkb.org/wiki/Nokia_BP-4L_battery

How many would I have to stack in parallel to power four 500W hub motors? 
Would 10s3p enough or should I go with 10s6p?
And what should I be looking at in regards to battery protection/balancing/overcharge/overdischarge?

<a href="http://www.cpkb.org/w/images/e/ed/Nokia_bp-4l_battery.JPG"><img src="http://www.cpkb.org/w/images/e/ed/Nokia_bp-4l_battery.JPG"></a>
```

---
## \#2 Posted by: saul Posted at: 2017-05-13T23:22:01.555Z Reads: 83

```
no no no no no no.

no .

no.

no.

no.

don't.
it.
won.t
work.

just no.
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-13T23:35:30.309Z Reads: 78

```
Their rated discharge is so low, you'd end up with exploding batteries even with 10+p
```

---
## \#4 Posted by: toma Posted at: 2017-05-14T00:09:07.644Z Reads: 76

```
[quote="Jinra, post:3, topic:22996, full:true"]
Their rated discharge is so low, you'd end up with exploding batteries even with 10+p
[/quote]

2000W / 36 v = 55.5 amps
They are 1500mah, and they seem to be ~1C.
So 55.5 / 1.5 = 37

So I'd have to build a 10s37p No?



<img src="/uploads/db1493/original/3X/e/0/e056881281c37ddf96543ca3a7e4b5d2a2b52288.png" width="690" height="311">
```

---
## \#5 Posted by: Alan_Smithee Posted at: 2017-05-14T00:24:29.032Z Reads: 68

```
I'd not look forward to connecting all those cells.. It will be so hard to find broken connections with 370 cells. 
and keep this in mind for even current share between parallel packs: https://www.electric-skateboard.builders/t/how-parallel-connections-can-carry-far-less-current/19275

uneven load might quickly develop into a chain reaction killing all your cells
```

---
## \#6 Posted by: Hummie Posted at: 2017-05-14T01:08:23.756Z Reads: 66

```
They're 2.25 amp each. Even better. 

But they might have internal circuitry that limits ur ability to build a pack. Maybe break one open or find the info.  Whenever I see those they have 3 connection points which is weird
Thinking again...I doubt those cells could handle any high current through them in series.  So u build it and forcing high current through them they aren't intended for.  Too thin even if they don't have internal fuse.  So I doubt they're a good idea but maybe discharge one Nd open it up and let's see
```

---
## \#7 Posted by: caustin Posted at: 2017-05-14T01:35:35.688Z Reads: 62

```
Would like to add a small comment to @saul

Ditto on the...NO
```

---
## \#8 Posted by: Hummie Posted at: 2017-05-14T01:36:38.482Z Reads: 62

```
Probably no ...but we should have a good reason for no.  ?
```

---
## \#9 Posted by: caustin Posted at: 2017-05-14T01:43:48.612Z Reads: 61

```
For science, yes love to see it

For safety, no would not like to see it happen to someone

But hey, if you got the skillz and the need to find out what happens, it's a free country lol.
```

---
## \#10 Posted by: cricrithezar Posted at: 2017-05-14T20:22:04.331Z Reads: 37

```
Yeah I'd be cautious running them over 1C and that means to run 2000W of power you would need 2kWh of batteries or pretty much all your 400 batteries connected in 10s40p (which is ridiculous, not even sure how you'd fit that many batteries on a boards.

If you do go through with this it would be really cool to see, but I'm not sure about how viable this is.

If you can find a better estimate of the c-rating on these cells than the 1C guess then even 2C would reduce it to 10s20p which is already more reasonable.

You'd get insane range though if you go 10s40p.
```

---

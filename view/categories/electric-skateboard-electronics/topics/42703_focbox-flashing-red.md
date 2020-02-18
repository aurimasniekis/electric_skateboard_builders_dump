# Focbox flashing red

### Replies: 11 Views: 597

## \#1 Posted by: KBONE Posted at: 2018-01-04T00:43:43.292Z Reads: 131

```
Master Focbox on Raptor 2 is flashing red and nothing happens when pushing throttle forward.
No fault codes in bldc tool and both motor spin during motor detection. What could be wrong?
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-01-04T00:45:53.309Z Reads: 129

```
@blasto or @JohnnyMeduse might be the perfect guys to help troubleshoot this for you.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-01-04T00:46:56.001Z Reads: 126

```
@KBONE please contact Enertion support!!
```

---
## \#4 Posted by: Blasto Posted at: 2018-01-04T00:49:38.103Z Reads: 123

```
Did you change any of the battery settings?
```

---
## \#5 Posted by: KBONE Posted at: 2018-01-04T00:50:27.467Z Reads: 120

```
No i only changed acceleration but have reset everything to default settings now, still makes no difference
```

---
## \#6 Posted by: Blasto Posted at: 2018-01-04T01:00:40.343Z Reads: 114

```
In the ppm tab, you have “current no reverse with brake” ticked?
```

---
## \#7 Posted by: KBONE Posted at: 2018-01-04T01:07:49.051Z Reads: 111

```
No, it was on disabled. Odd as i've used the board after changing settings. Vesc still flashlng red, is it supposed to do that? But wheels spin when changing to current no reverse.
```

---
## \#8 Posted by: DavidBanner Posted at: 2018-01-04T01:39:57.525Z Reads: 102

```
did you check your voltage cutoff minimums are correct for your battery pack?
```

---
## \#9 Posted by: Deckoz Posted at: 2018-01-04T01:50:53.359Z Reads: 97

```
[quote="KBONE, post:7, topic:42703"]
wheels spin when changing to current no reverse.
[/quote]

Let me guess, you clicked "Load defaults" in the bldc tool...

And now
-app configuration is probably set to No App
-ppm tab probably is set to disabled, instead of "Current no reverse"
-your motor detection is probably invalid

You need to reconfigure the VESC from scratch. Follow a VESC setup guide, as it sounds like nothing is wrong other then you loaded defaults thinking it would fix your messing with settings.. lol
```

---
## \#10 Posted by: KBONE Posted at: 2018-01-04T03:05:08.284Z Reads: 78

```
I know. @Blasto helped me fixing it. All good now 😂
```

---
## \#11 Posted by: Deckoz Posted at: 2018-01-04T03:14:58.452Z Reads: 79

```
Hahaha glad is "alive"
```

---

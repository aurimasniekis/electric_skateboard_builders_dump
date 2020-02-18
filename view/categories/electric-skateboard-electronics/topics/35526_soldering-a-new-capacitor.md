# Soldering a new capacitor

### Replies: 24 Views: 610

## \#1 Posted by: 12meterkuk Posted at: 2017-10-14T19:53:29.749Z Reads: 102

```
So I messaged evolve and they are charging me 50 bucks for a new bms. I think only the capacitor of my old one is a little buggy. 

Will getting a new capacitor and soldering it on myself be alright? Anything important to know before I do it?
```

---
## \#2 Posted by: b264 Posted at: 2017-10-14T20:11:09.091Z Reads: 94

```
The way I see it, you'll either

A) spend $50 for a new one

OR

B) maybe fix it for hella cheap, otherwise spend $50 for a new one

Clearly, B is better LoLz
```

---
## \#3 Posted by: Fiori Posted at: 2017-10-14T20:17:04.779Z Reads: 84

```
I tried to get the BMS separate from them and they will not sell it to me. I bought my board a year ago in the store(I even sent them the receipt). I'd get the bms as a backup just incase, then try to repair your old one.
```

---
## \#4 Posted by: 12meterkuk Posted at: 2017-10-14T20:22:22.068Z Reads: 80

```
[quote="b264, post:2, topic:35526"]
Clearly, B is better LoLz
[/quote]

Obviously! :smile:

[quote="Fiori, post:3, topic:35526"]
I tried to get the BMS separate from them and they will not sell it to me
[/quote]

What did they say? I messaged my distributor with pictures of the old bms and told him that the capacitor was a little deformed and it kept shutting down the board randomly and he offered to send me a new one for 50 bucks (37 + 17 shipping)
```

---
## \#5 Posted by: Fiori Posted at: 2017-10-14T20:23:52.841Z Reads: 73

```
I said that mine was intermittently working and that I could see a burn spot on the bms itself. They said my only option was to send it in for repairs. I'll rip that POS out and put two VESC's in before I send it back to evolve....
```

---
## \#6 Posted by: darkkevind Posted at: 2017-10-14T20:25:40.748Z Reads: 68

```
I'd get the cap and repair it yourself if I were you. It's easy enough of you've soldered before.
```

---
## \#7 Posted by: i2oadsweepei2 Posted at: 2017-10-14T20:30:31.725Z Reads: 65

```
[quote="12meterkuk, post:1, topic:35526"]
Will getting a new capacitor and soldering it on myself be alright? Anything important to know before I do it?
[/quote]

I just saw that blasto mentioned to another user today that capacitors are polarized and should have a ground marking on them. I didn't know that either.

Hope everything works out for you.
```

---
## \#8 Posted by: scepterr Posted at: 2017-10-14T20:53:22.389Z Reads: 63

```
Not all capacitors are polarized, the ones that are, are marked as such
```

---
## \#9 Posted by: b264 Posted at: 2017-10-14T20:56:17.260Z Reads: 62

```
[quote="i2oadsweepei2, post:7, topic:35526"]
capacitors are polarized
[/quote]
[quote="scepterr, post:7, topic:35526"]
Not all capacitors are polarized
[/quote]

Most are; the bigger ones definitely are.  If it is a polarized one, it's very important it's installed the correct direction.  The negative leads will be marked somehow.
```

---
## \#10 Posted by: wafflejock Posted at: 2017-10-14T21:02:13.830Z Reads: 55

```
Pretty sure size isn't the issue here (motion in the ocean), but electrolytic capacitors are polarized and go pop or bang depending on the size if you reverse polarity on them.  Believe ceramic capacitors or whatever other non electrolytic ones don't have polarity to them. 

https://learn.sparkfun.com/tutorials/polarity#electrolytic-capacitors
```

---
## \#11 Posted by: b264 Posted at: 2017-10-14T21:04:00.556Z Reads: 49

```
[quote="wafflejock, post:10, topic:35526"]
Pretty sure size isn't the issue here
[/quote]

The bigger ones are more likely to be electrolytic.  The tiny ceramic ones are non-polarised
```

---
## \#12 Posted by: wafflejock Posted at: 2017-10-14T21:05:11.356Z Reads: 45

```
Yup was still editing to add some clarification but saying if they have a small black one with a white stripe down one side they might be confused about what is "small"
```

---
## \#13 Posted by: scepterr Posted at: 2017-10-14T21:05:54.855Z Reads: 50

```
There are also smd caps that are polarized. This doesn't take this much discussion lol 

If it's polarized, it will say so
No matter size or type
```

---
## \#14 Posted by: 12meterkuk Posted at: 2017-10-14T21:54:07.231Z Reads: 44

```
What kind of capacitor should I use? Any recommendation? 

I would like to get something beefier if possible
```

---
## \#15 Posted by: scepterr Posted at: 2017-10-14T21:57:26.192Z Reads: 44

```
A picture or some detail about what capacitor you are trying to replace would be most useful 😉
```

---
## \#16 Posted by: 12meterkuk Posted at: 2017-10-14T22:00:01.809Z Reads: 44

```
<img src="/uploads/db1493/original/3X/f/8/f8b53ec7efe335c6a4e8a5ce2c44c64c34d56711.jpeg" width="375" height="500">

Sorry for the shitty picture I look it a few days ago when making a new pack just for reference. 

It’s the tiny one under the wires
```

---
## \#17 Posted by: scepterr Posted at: 2017-10-14T22:00:36.464Z Reads: 42

```
Lol can you circle it please
```

---
## \#18 Posted by: 12meterkuk Posted at: 2017-10-14T22:01:51.580Z Reads: 44

```
<img src="/uploads/db1493/original/3X/a/9/a9208d7d0e9975c60a296dd170368c43f5074506.jpeg" width="390" height="500">
```

---
## \#19 Posted by: scepterr Posted at: 2017-10-14T22:09:21.695Z Reads: 42

```
What are the values on it?
Also, physically looks fine to me...
```

---
## \#20 Posted by: i2oadsweepei2 Posted at: 2017-10-14T22:10:59.439Z Reads: 43

```
@scepterr @b264 thank you both for the clarification.
```

---
## \#21 Posted by: 12meterkuk Posted at: 2017-10-14T22:13:16.928Z Reads: 40

```
I don't think the picture is clear enough.

The capacitor is a little deformed, its not a tube shape anymore, kind of twisted if you know what i mean.

I'm not sure what the values are but I can ask  evolve customer service.

Not sure if they will tell me though.
```

---
## \#22 Posted by: scepterr Posted at: 2017-10-14T22:14:03.863Z Reads: 39

```
It'll be printed on the cap, just gotta lift it up and  look
```

---
## \#23 Posted by: 12meterkuk Posted at: 2017-10-14T22:14:59.019Z Reads: 38

```
I sealed up the pack yesterday... damn. I'll take a look the next time i open it up. 

Will update the thread then. Thanks
```

---
## \#24 Posted by: scepterr Posted at: 2017-10-14T22:17:27.270Z Reads: 36

```
@longhairedboy Could you enlighten us as to what cap that is ?
```

---

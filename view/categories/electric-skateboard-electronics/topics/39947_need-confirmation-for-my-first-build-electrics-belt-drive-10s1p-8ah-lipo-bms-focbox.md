# Need confirmation for my first build electrics &#124; Belt drive &#124; 10s1p 8Ah lipo &#124; BMS &#124; Focbox

### Replies: 7 Views: 606

## \#1 Posted by: DullElysium Posted at: 2017-12-02T13:11:12.066Z Reads: 97

```
Hello,

I've been looking for how I could build my first eskate for quite a while now and I finally ordered the focbox+controller+wheels from Enertion.

I've tried my best to learn, how I should wire everything, but I'm no electrical expert. So what I'd greatly appreciate would be if someone with greater knowledge could check my setup before I buy any other parts, so I don't blow things up.

I'd like to be able to pretty much screw the enclosure on and only have to open it for maintenance etc.

Some things I've been thinking about:
-2x 5s1p 8000mAh lipo's in series to a BMS
-xt90 loop key
-resistor through a momentary switch to fill the vesc capacitors while the loop key is being put in.
-Momentary switch for the battery current indicator for checking the battery charge in every state

Also, I'd like to add a led to indicate the momentary switch working in the anti-spark system and another one to light up as the xt90 loop key is in place. Would these led's be easy to impliment? The led would be installed after the switches and with a resistor, or is there more to it?

Would this be ok?
<img src="/uploads/db1493/original/3X/5/4/54dc7865aee44d9370da8e75a2e25a032bc85c04.jpg" width="411" height="500">

I'll just put a parts list here for the electronics too to clarify things more:

192kv sk3 turningy motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
2x 5s1p 8000mAh lipo's: https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html
Focbox vesc: http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/
Supower BMS: https://www.ebay.com/itm/221769582503
Battery capacity/voltage display: https://www.ebay.com/itm/282674792095
The switches in the picture are just placeholders.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-02T15:57:03.035Z Reads: 79

```
Your balance wires shoul connect to the bms starting at pin 1. It doesn’t look that way in your diagram. 

About your antiSpark system, it would be much simpler to just use an antiSpark XT90 connector which has a built in resistor
```

---
## \#3 Posted by: FredrikHems Posted at: 2017-12-02T16:12:14.890Z Reads: 78

```
instead of going with the sk3 6364 190kv motor, I would go with the sk3 6374 192kv. Other than that, you will obviously need the longboard itself
```

---
## \#4 Posted by: DullElysium Posted at: 2017-12-02T16:28:24.154Z Reads: 77

```
Whoopsie, flipping the BMS board around seems to have screwed with my brain. Thanks for pointing that out! I edited the pic so that the #1 cell should now be connecting to the #1 slot in the BMS.

I considered the xt90 antiSpark connector, but (correct me if i'm wrong) doesn't it let the small current flow to the vesc constantly? Or is the flow through resistor also cut when unplugging the loop key? I'm just thinking that I sleep better knowing that they're both disconnected. If that makes any sense.

Thanks a ton for the help! Loving the community here.

**EDIT: just found a video which explained the xt90 anti spark connector in detail, going to go with that one**
```

---
## \#5 Posted by: DullElysium Posted at: 2017-12-02T16:36:56.584Z Reads: 67

```
Thanks for the suggestion. I had totally missed the 192kv motor. Seems to have better specs with not too much extra cost, so I think I'll go with that one.

I'm not a 100% settled on the deck yet, but I think I'm gonna try to mount the system on a 8,5" regular skateboard deck, since that's what I'm most comfortable riding. I do have a regular longboard, but it's not as comfortable to ride as a normal skateboard imo.
```

---
## \#6 Posted by: wafflejock Posted at: 2017-12-02T17:39:02.827Z Reads: 64

```
Just minor correction the battery is 10S 8Ah made of two 5S 8Ah since you're connecting them in series (no 2p anywhere usually only applicable to 18650).  Regarding deck I'm using a moose old school deck and still pretty tough fitting everything on there.  Be sure to lay everything out and take measurements to see where things will fit, also keep in mind tighter turn radius basically means also less stable at high speed.

<img src="/uploads/db1493/original/3X/0/b/0be0c1b357dc5d213ca0f9175b5363b66b29ae74.jpg" width="374" height="500">

<img src="/uploads/db1493/original/3X/c/8/c83b8231fc24135551908fde87be8639f757b1d9.jpg" width="666" height="500">
```

---
## \#8 Posted by: DullElysium Posted at: 2017-12-02T17:58:39.519Z Reads: 55

```
I have absolutely no clue as to why I put 2p there. I've been searching so much of different components that they seem to mush together now :smiley: But yeah, you're correct. 2x5s1p is what I'm talking about. I'll edit my original post on that part.

I tried to make that mockup image for myself to see that I could somehow fit everything in the space that would be left of a normal skateboard deck. It's a tight fit, but should be somewhat doable. If not, I'll have to go with something a tad longer with a kicktail. I've seen someone screw the trucks to the nose and the tail to get more space in between.. Looked kind of cool, but I'd really prefer to have a kicktail.

You're also correct about the stability at higher speeds. I might have to tighten the trucks a tad tighter than I'm used to at first to eliminate some speed wobbling. But again, if it doesn't feel right, I can always swap the board for a longer one down the road.

Liking your setup btw! Nice to see normal skateboard decks on e-skates.
```

---

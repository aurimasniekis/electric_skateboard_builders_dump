# Shorting out motor or bad wire connections? Video included

### Replies: 26 Views: 725

## \#1 Posted by: gliz5714 Posted at: 2017-09-24T15:46:45.372Z Reads: 96

```
Good morning(afternoon/evening) all - I was riding my board around this morning when it started to "die" on me.  I'd hop off and the motor would be stuttering then might not spin at all.  I thought it could have been out of juice (was riding for 30ish minutes, should go for ~an hour though).  

Get home and plug it in and everything works fine - so that's when I started the video to start pulling on wires (I swear at 1:06-1:08 so I guess NSFW?) - Also, sorry for vertical video, I know I have sinned...

https://www.youtube.com/watch?v=toCfiV_L73c

You can see early on it works ok then starts to go meh, works again for awhile, but then at 1:03-1:04 it sparks - zoom in right around where the wires get close to the motor you might see a bit of yellow and a small spark sound (bzzzt?). 

Is this a problem with the motor connections that I can solve?  Or?  This is my first foray into building anything with electronics so just trying not to get myself killed on this thing.
```

---
## \#2 Posted by: DavidBanner Posted at: 2017-09-24T15:52:48.162Z Reads: 90

```
Could be an iffy connector or a break in the cable, or possibly a bad connection inside the motor.

If you islolate the dodgy cable first - possibly the middle one from the looks of it:
- then hold the cable behind the connector with a finger to the deck - wiggle the cable between the connector and motor - if no issues then hold the wire the other side of the connector with your finger and do the same on the other side of the cable
- if still no issues then hold the wire to your deck with two fingers either side of the connector and tap/wiggle the connector.

hopefully that makes sense, the idea is to isolate sections of the cable and test those
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-09-24T15:54:21.336Z Reads: 84

```
if there is a spark it must be shorting - any signs of wear in the cables? i.e. bare wires?

be real careful here or a smoked VESC is on the cards
```

---
## \#4 Posted by: gliz5714 Posted at: 2017-09-24T15:57:28.889Z Reads: 78

```
Well shoot.  Looks like the yellow wire has a small (1/4" long) scratch through the rubber coating and you can see wire =/

Something probably got up there (rock, stick) when i was carving around and possibly ripped it.  can I just shrinkwrap that or do I have to swap out a wire?

Still haven't pulled around on stuff, just noticed the cut on the rubber.
```

---
## \#5 Posted by: DavidBanner Posted at: 2017-09-24T15:58:17.040Z Reads: 73

```
shrink wrap it - you'll be fine.

nice easy fix - the best kind :)
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-09-24T15:59:09.401Z Reads: 70

```
you might want to add a few bits of shrink wrap on top of each other for extra peace of mind
```

---
## \#7 Posted by: gliz5714 Posted at: 2017-09-24T16:03:31.414Z Reads: 70

```
Thanks - this is the "cut".  This would cause all that heartache?  😣

 <img src="/uploads/db1493/original/3X/8/d/8dbf04d9074a1800649a9990abc64f9955838816.jpg" width="666" height="500">
```

---
## \#8 Posted by: DavidBanner Posted at: 2017-09-24T16:05:24.340Z Reads: 68

```
only if it's shorting on something... looks close enough to the motor to short on the casing?

it needs fixing anyways though
```

---
## \#9 Posted by: gliz5714 Posted at: 2017-09-24T16:09:21.280Z Reads: 66

```
It faces the underside of the board and wouldn't reach the casing.  Does it have to short on something metal or anything organic that touches it?  

I definitely plan on wrapping it up just curious at this point!
```

---
## \#10 Posted by: DavidBanner Posted at: 2017-09-24T16:11:57.212Z Reads: 69

```
to spark it would need to be shorting or broken internally (but it doesn't look broken).
```

---
## \#11 Posted by: gliz5714 Posted at: 2017-09-24T16:45:56.005Z Reads: 65

```
Landscape this time!  I taped the motor to "on" so it should stay the same speed throughout.  It does not...

Looks like the black wire has a bad connection between the bullet connectors.  Probably a bad solder joint I'd assume.  Does this sound about right?

Thanks for the help!

https://youtu.be/kRuG9Uyitis
```

---
## \#12 Posted by: DavidBanner Posted at: 2017-09-24T16:48:45.667Z Reads: 63

```
awesome video

my money is on a bad solder joint on the black wire connector too.

Strip off the heat shrink, reheat and add a little solder to both the connectors on that cable, add more heatshrink and it should be a done deal, or at the very least eliminate a potential failure point :slight_smile:
```

---
## \#13 Posted by: DavidBanner Posted at: 2017-09-24T16:51:01.710Z Reads: 61

```
[quote="gliz5714, post:11, topic:33850"]
Thanks for the help!
[/quote]

my pleasure
```

---
## \#14 Posted by: gliz5714 Posted at: 2017-09-24T16:51:39.878Z Reads: 57

```
Sounds like a job for tonight - Thanks again for confirming!  Kinda getting the hang of this whole electronics thing ;-)
```

---
## \#15 Posted by: DavidBanner Posted at: 2017-09-24T16:52:59.104Z Reads: 59

```
those big connectors are a great way to brush up your soldering skills. 

a big tip for your iron will make a huge difference (if you don't have one already)
```

---
## \#16 Posted by: OskarCastrone Posted at: 2017-09-24T17:46:00.961Z Reads: 56

```
Yes, a big tip and a fairly powerfull iron will make it much easier.
```

---
## \#17 Posted by: scepterr Posted at: 2017-09-24T17:50:27.601Z Reads: 55

```
If you are using the springy spinny bullets replace with solid bullets
```

---
## \#18 Posted by: gliz5714 Posted at: 2017-09-24T20:57:43.750Z Reads: 52

```
[quote="scepterr, post:17, topic:33850"]
ing the springy spinny bullets replace with solid bu
[/quote]

They are big 5.5mm connectors that I got and soldered all on.  I am a novice solderer so chances are one of them broke loose!
```

---
## \#19 Posted by: gliz5714 Posted at: 2017-09-24T20:58:34.038Z Reads: 48

```
Iron should be powerful enough - did solder it all together to start with but possibly this was my first connector so it just hasn't held on through all the bumps I have been hitting recently...
```

---
## \#20 Posted by: gliz5714 Posted at: 2017-09-30T20:07:02.308Z Reads: 43

```
So looks like I wasn't so lucky.  Redid the solder joints on the black wire and it seems to still be shorting a bit.  Looks to be in the motor... See video below.

How does one take it apart to diagnose?  Is there a solid thread that shows internal repairs?  Figure I might as well try and if it is trash I will just buy a slightly bigger motor (probably 200-230kv) or if it works then I can just wait til next year!

https://youtu.be/meEy6txCXs0
```

---
## \#21 Posted by: GrecoMan Posted at: 2017-09-30T21:26:03.456Z Reads: 40

```
Loosen your motor mount screws a bit and check if there are any sparks inside the motor
```

---
## \#22 Posted by: pat.speed Posted at: 2017-10-01T08:29:11.764Z Reads: 35

```
If there is a circlip on it just take that off with some pliers then the motor can should pretty much fall of and you should be able to see the stator and wires if there are any shorts. If there is no circlip I am not sure how to get it apart
```

---
## \#23 Posted by: MysticalDork Posted at: 2017-10-01T08:46:22.674Z Reads: 35

```
What @grecoman said - It's possible that the motor mount screws are too long and are pressing against the internal windings, causing a short. Try loosening/removing the motor mount screws and see if that helps.
```

---
## \#24 Posted by: scepterr Posted at: 2017-10-01T09:00:14.238Z Reads: 34

```
Seems like there might be a tear in insulation and one of the phases is touching the motor body
The short seems to be happening with movement, not consistently which is what you would expect with a constant short like a screw.
```

---
## \#25 Posted by: gliz5714 Posted at: 2017-10-01T13:53:04.202Z Reads: 27

```
Mount screws are the perfect length actually.  Nothing sticks out the end into the motor (have washers to prevent).  I have taken apart and verified that but it was initially on my mind!
```

---
## \#26 Posted by: gliz5714 Posted at: 2017-10-01T13:54:38.171Z Reads: 26

```
I will check all insulation.  This definitely could be the cause - very intermittent shorting but no sparks that I can see while this is happening.  Might also cut all wires 1cm shorter and solder new connectors in case something else is the matter...

Internal wires all look ok though, once it gets past the sheathing.  No broken wires and windings are nice and tight.
```

---

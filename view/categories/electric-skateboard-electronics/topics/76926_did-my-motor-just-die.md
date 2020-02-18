# Did my motor just die?

### Replies: 29 Views: 455

## \#1 Posted by: accrobrandon Posted at: 2018-12-03T18:03:49.856Z Reads: 173

```
So I was riding to work casually and felt this little "glitch" I think thats a good word as it wasnt cogging ... Then the board felt sluggish which when I stopped i noticed only one motor was running... The motor was super hot.. When I cut the power it cooled..power on gets hot.. I had to keep riding to.get to work but less than a mile... Checking it along the way... And at some point it started moving again but doesnt really spin with the same power/force as the other motor with a lil rev of the throttle.

Thoughts?
```

---
## \#2 Posted by: brenternet Posted at: 2018-12-03T18:30:18.996Z Reads: 155

```
My guess, magnet is loose and having a party inside the can.
```

---
## \#3 Posted by: accrobrandon Posted at: 2018-12-03T18:33:44.450Z Reads: 147

```
I.didnt hear any rattling or feel any friction from something that might have been wedged =\
```

---
## \#4 Posted by: Sender Posted at: 2018-12-03T18:43:29.715Z Reads: 138

```
Is there resistance when you turn it by hand?
```

---
## \#5 Posted by: accrobrandon Posted at: 2018-12-03T18:48:52.282Z Reads: 124

```
I'll need.to try later when I.get back to the board . are there any multimeter tests I can do as well to see.if theres any info there?
```

---
## \#6 Posted by: olestra Posted at: 2018-12-03T18:53:49.805Z Reads: 114

```
not an expert, but resistance between each of the leads would be a good idea -- wire 1-2, 2-3 and 3-1 should have pretty much exactly the same resistance

 -- if one is high, you've got a winding that's been nicked and will fail.
 if one is low, you've got a winding that has shorted.
 you should be able to look up the expected resistance
```

---
## \#7 Posted by: accrobrandon Posted at: 2018-12-03T21:39:39.412Z Reads: 103

```
[quote="Sender, post:4, topic:76926, full:true"]
Is there resistance when you turn it by hand
[/quote]

Yes... Feels like the belt is super tight even tho I have the idlers as loose a possible... My other motor with proper tension spins better =\
```

---
## \#8 Posted by: accrobrandon Posted at: 2018-12-05T21:59:44.147Z Reads: 71

```
just gave it a quick test and all measured out the same,
i was assuming it was still dead and was gonna swap in a random motor for a week to keep the dual power alive, but decided to run motor config. again to see if anything tripped or gave an error code. everything checked out fine and now its running again, although still seems to have some sort of drag on its free spin abilty... can is noticeable warmer compared to the other... still no noticeable sounds to help in diagnosis
```

---
## \#9 Posted by: dareno Posted at: 2018-12-05T23:14:52.098Z Reads: 69

```
[quote="accrobrandon, post:8, topic:76926"]
but decided to run motor config. again to see if anything tripped or gave an error code. everything checked out fine and now its running again,
[/quote]

Took a bit of a chance there.  Usually a bad idea to detect a suspect motor.  Make the vesc go poof.  
I would be getting in there and checking out the bearings and magnets before it does some more damage.  A rear bearing went on one of my motors and the resulting debris shattered the sensor pcb and shorted the motor killing my vesc.  That started off by feeling a bit tight on hand spin.  Definitely time to open her up if its not still in warranty.
```

---
## \#10 Posted by: accrobrandon Posted at: 2018-12-05T23:55:52.837Z Reads: 65

```
im sure it is... but back to china it would have to go =/ #maytech
```

---
## \#11 Posted by: dareno Posted at: 2018-12-06T00:06:22.588Z Reads: 60

```
Pain in the arse.  I've no idea what maytech are like for back up.  Never had one break on me.  Try mailing them and maybe they can help.  When my HK motor went they told me to open it to see.  When I sent it back eventually it was in bits in a box.  Did everything by mail and photos and they sent a replacement before receiving the bad one.  Depends whether maytech stand by their products I guess.
```

---
## \#12 Posted by: accrobrandon Posted at: 2018-12-06T01:57:28.714Z Reads: 48

```
we'll see what happens..just pulled it off and swapped another in...guess i get to test another offset idea for science.... one 6355 190kv at 15/36 and a 6374 170kv at 18/36 =P
```

---
## \#13 Posted by: dareno Posted at: 2018-12-06T02:10:25.576Z Reads: 44

```
dual diagonal for that set up
```

---
## \#14 Posted by: J0ker3366 Posted at: 2018-12-06T02:18:48.177Z Reads: 46

```
I skimmed through this but have you check phase wires connections? My liftboard would always pop a weld on the connectors one the motor. And even could be the vesc side as well. I know when one would pop, id have to push start and it would take off as normal. Motor would get super hot. Cogged like ass from a dead stop.
```

---
## \#15 Posted by: accrobrandon Posted at: 2018-12-06T02:20:15.924Z Reads: 43

```
nah, wont work with all the shit crammed in my box... anyways i got those 6374s coming in from the maytech group buy hopefully in the next week or so, so wont have to be to long like this.... AND got the "cheap ass pnuemies" delivered as well...so all sorts of R&D going on this week lol
```

---
## \#16 Posted by: dareno Posted at: 2018-12-06T02:23:57.628Z Reads: 41

```
I'm all out of builds till after the new year.  Sad times.  Can't wait to start pulling the trigger on some new parts.
```

---
## \#17 Posted by: accrobrandon Posted at: 2018-12-06T02:27:07.106Z Reads: 41

```
sometimes u just gotta fire up the soldering iron for no good reason and act like yur being productive lol
```

---
## \#18 Posted by: dareno Posted at: 2018-12-06T02:28:58.857Z Reads: 42

```
I'm just being selfish.  I still have the wifes board to finish and 4 repairs to bang out.  Nothing for me though.  Me me me
```

---
## \#19 Posted by: accrobrandon Posted at: 2018-12-06T02:55:39.229Z Reads: 35

```
build an ebike then...theres plenty of shit to go wrong and plenty of improvements to keep you busy lol
```

---
## \#20 Posted by: dareno Posted at: 2018-12-06T03:08:48.450Z Reads: 35

```
https://www.esurf.com/
this is what I want to build.  Off topic but its your topic so no drama.
```

---
## \#21 Posted by: iTzDiego Posted at: 2018-12-06T03:28:13.744Z Reads: 33

```
[quote="brenternet, post:2, topic:76926"]
having a party inside the can
[/quote]

time to call the cops and put in a noise complaint
```

---
## \#22 Posted by: accrobrandon Posted at: 2019-02-22T20:00:50.361Z Reads: 23

```
Ok lets bring this back to life. Just had time to crack open the can to take a look..anything seem odd? If you look at the stator there is some hard goo... Could be epoxy for the sensor wires?? Or is that not normal... Also discoloration on that particular arm of winding (not sure the correct terms) inside of can...all.magnets seem fine although there appears to be some of the  surface might have had minor friction of some.sort. 

![0222191452|666x499](upload://nRoCV4p4RhOjvXBN0wAQZUcoM4Y.jpeg) 
![0222191453|666x499](upload://qTyzh2rPDkQxDug1QoMJcYH3ted.jpeg) 
![0222191453a|666x499](upload://rg7G0KQodJgBcZCkm0IRTAuClwq.jpeg) 
![0222191453b|666x499](upload://exzikbGjWVBW5T0P45S65Ye0wgp.jpeg) 
![0222191453c|666x499](upload://vcUuDgQxgvr4RpCc0izyLqSPymv.jpeg) 
![0222191454|666x499](upload://csgcA5TN4EaIezwlfag2JBbv59j.jpeg)
```

---
## \#23 Posted by: accrobrandon Posted at: 2019-02-22T20:04:17.448Z Reads: 20

```
Also look at the solder job on the pcb of the green wire... All other 4 look.similar where as that one looks.like it melted or something?
```

---
## \#24 Posted by: dareno Posted at: 2019-02-23T00:09:57.266Z Reads: 13

```
That is just a tail that hasn't been snipped by the looks of it.  I don't know if its the pic quality but it looks like there is wear on the magnets and what is the dust in there?  All the bearings are good with no play?
```

---
## \#25 Posted by: accrobrandon Posted at: 2019-02-23T00:14:33.059Z Reads: 15

```
yes to wear on magnets... but nothing fell out as far as debris... i assume dust but cant tell... bearings seemed fine...
```

---
## \#26 Posted by: dareno Posted at: 2019-02-23T00:21:57.404Z Reads: 15

```
Sealed can maytechs?  No danger of something getting in there and causing restriction then burn out then. That discolouration on the windings is suss too.  You might just have to put that down to failure and strip it for parts.
```

---
## \#27 Posted by: accrobrandon Posted at: 2019-02-23T01:20:12.234Z Reads: 15

```
yeah imma write maytech and see... as i got this straight from them and its been under a year... but we'll see...
```

---
## \#28 Posted by: dareno Posted at: 2019-02-23T02:25:30.008Z Reads: 12

```
The fact its been stripped down may cause an issue.  Open the communication with no mention of investigation bar electronically testing and let them suggest you take it apart.  Hopefully they won't just tell you to return it and will ask you to do the strip down.  Good luck man
```

---
## \#29 Posted by: accrobrandon Posted at: 2019-02-23T03:36:31.211Z Reads: 10

```
to late...hahaha


its ok... some one local has a couple of TB for 70 a pop so will end up picking those up anyways while i figure this out ;)
```

---

# Slightly unequal power to motors an issue?

### Replies: 26 Views: 497

## \#1 Posted by: Taliesin Posted at: 2018-08-24T04:31:30.981Z Reads: 120

```
https://youtu.be/5-NQRbXBoB0

Is this going to be an issue? It’s only noticeable when I am barely throttling at the start. The right side wheel starts before the left. Will this make the ride feel off center or should I not worry about this?

Could this just be an issue of how tight the axle bolt is on the wheel?
```

---
## \#2 Posted by: goldrabe Posted at: 2018-08-24T04:57:31.304Z Reads: 111

```
Check your belt tension and alignment. It can be also the nut of your wheel. For my liking it looks like too much drag.
And please, before you create a new topic for each problem try the search bar!
```

---
## \#3 Posted by: TowerCrisis Posted at: 2018-08-24T04:58:15.321Z Reads: 108

```
Do you have the vesc's in a canbus master slave? I've found that my slave always starts up a little after the master.

If it's split PPM...
You could have differing PPM config if you did the remote setup separate for both. It's usually best practice to tune one vesc, download it's config to your computer, and then push that same config to the other vesc (and then do motor config) to ensure that all settings are identical. It's the small things like that which have caused me headache in the past.
```

---
## \#4 Posted by: Taliesin Posted at: 2018-08-24T04:59:14.530Z Reads: 100

```
Split ppm. I’ll try that tomorrow. Thank you. Sorry for the excess posts.

And yes I did the remote setup separate for both
```

---
## \#5 Posted by: Cobber Posted at: 2018-08-24T05:00:30.527Z Reads: 92

```
Is it just me, or do the motors look like they are different sizes?
```

---
## \#6 Posted by: Taliesin Posted at: 2018-08-24T05:01:31.221Z Reads: 89

```
Same size.
```

---
## \#7 Posted by: dareno Posted at: 2018-08-24T06:28:40.180Z Reads: 83

```
@goldrabe looks to be correct there.  Both the belts look too tight and the left more so.  Be careful of overtight belts they can cause things to go pop.  Hang loose man.
```

---
## \#8 Posted by: Taliesin Posted at: 2018-08-24T06:51:37.010Z Reads: 80

```
Best way to loosen them?
```

---
## \#9 Posted by: danielz Posted at: 2018-08-24T06:57:31.970Z Reads: 81

```
Mine are slightly out too when not loaded, no quite as much. But just in case, double check both vesc settings are the same esp throttle calibration.
```

---
## \#10 Posted by: Sebike Posted at: 2018-08-24T07:03:07.399Z Reads: 81

```
Loosen the screws holding the motor and adjust it ever so slightly closer to the wheel pulley. 

If you have adjustable idlers you can adjust tension there instead by sliding the idler away from the center of the mount and retighten screws...

You can try the drag by giving the wheels a spin by hand and if the two wheels stop spinning at the same time, belts are likely equally tensioned for the two motors /wheels.
```

---
## \#11 Posted by: Taliesin Posted at: 2018-08-24T07:04:02.725Z Reads: 71

```
Awesome, I’ll give that a shot tomorrow. Thank you so much.
```

---
## \#12 Posted by: dareno Posted at: 2018-08-24T07:06:11.079Z Reads: 71

```
It could be me but those mounts don't look to have lateral adjustment.  What are they?
```

---
## \#13 Posted by: Andy87 Posted at: 2018-08-24T07:15:23.396Z Reads: 71

```
looks like this on

https://www.electric-skateboard.builders/t/motor-mounts-kits-for-trampa-atb-and-mbs-matrix-old-type-matrix-ii-ats/44749?u=andy87

so they should have
```

---
## \#14 Posted by: dareno Posted at: 2018-08-24T07:25:14.952Z Reads: 67

```
@Andy87 yeah make you right there!  All good.
@Taliesin Try motor detection without belts attached too.  My first dual did a similar thing because they were unequally tensioned.   A very nice guru on here gave me that advice and to loosen belts and hey presto it was perfect.  Nice build btw
Oh and don't worry about what you're doing with your posts, it may upset some but the answers are coming.
Put them on the noob thread and you won't get a reply till xmas :joy:
```

---
## \#15 Posted by: lrdesigns Posted at: 2018-08-24T09:11:11.414Z Reads: 62

```
This is perfectly normal, the motors can have slightly different minimum amps before they start to rotate. 

You can up the minimum power the motors receive to make it go away, but its not actually a problem. Just looks weird.
```

---
## \#16 Posted by: Brdchris Posted at: 2018-08-24T09:54:11.225Z Reads: 59

```
In industry we call “motor detection” rotating auto tune. Rotating Auto tune is always done with a motor removed from a load. I don’t know why that isn’t part of the procedure with our boards. It should be.
```

---
## \#17 Posted by: Cobber Posted at: 2018-08-24T10:11:35.988Z Reads: 57

```
Motor detection should be done "un-loaded", no motor spur, cog, gear... nothing just the shaft :nerd_face:
```

---
## \#18 Posted by: Boxer86 Posted at: 2018-08-24T10:22:14.129Z Reads: 57

```
How do you do this “push the same config to the other vesc”? This is a really good idea and I want to do this when I get to setting up my focboxes. Do you save settings to your computer then apply when you plug in your other vesc? Please excuse my ignorance. I will be using enertions vesc tool.
```

---
## \#19 Posted by: Brdchris Posted at: 2018-08-24T12:30:42.889Z Reads: 54

```
I see what you did there 🧐
```

---
## \#20 Posted by: pat.speed Posted at: 2018-08-24T12:57:13.001Z Reads: 53

```
This is normal, happens on my dual board running split ppm, you will notice if you add some friction to the wheels they will both start at the same time
```

---
## \#21 Posted by: Simonwantstobuildabo Posted at: 2018-08-24T13:55:59.534Z Reads: 50

```

Hi! My dual beast 6355 maytech motor setup, with dual focbox and 12s5p has some issues!
( I use maytech standard remote and reciver )

Also i use VESC TOOL!

One of the motors in “fast mode” shuts down? So i can press full throttle in eco mode, no problem, but when i switch to fast mode it shuts off after a while? Like you can hear 100% Throttle, and after 5,10,20 seconds it goes down to like 60% or even less?

Short version: When pressing full throttle in fast mode, motor start slowing down.
```

---
## \#22 Posted by: TowerCrisis Posted at: 2018-08-24T16:39:08.961Z Reads: 44

```
[quote="Boxer86, post:18, topic:65911"]
Do you save settings to your computer then apply when you plug in your other vesc?
[/quote]

Yep. Exactly that. You can import and export settings as a whole.
```

---
## \#23 Posted by: dareno Posted at: 2018-08-24T20:43:08.916Z Reads: 37

```
Hey my friend start a new topic with this issue.  Otherwise its kind of hijacking someone elses thread.
```

---
## \#24 Posted by: Taliesin Posted at: 2018-08-24T21:03:51.437Z Reads: 37

```
I don’t mind. Extend the knowledge :)
```

---
## \#25 Posted by: dareno Posted at: 2018-08-24T21:11:38.616Z Reads: 36

```
[quote="Taliesin, post:24, topic:65911"]
I don’t mind. Extend the knowledge :slight_smile:
[/quote]
I get that about you my friend and it does you credit but he won't get as much help if he posts on someone elses thread.  Forum etiquette is taken quite seriously around here as you have found out lol.  It can take a while to learn how to navigate the site especially if english is not your first language and I'm just trying to point him in the right direction so he gets the help he needs.
```

---
## \#26 Posted by: Taliesin Posted at: 2018-09-03T17:31:35.965Z Reads: 21

```
Loosened belts ever so slightly and it fixed the issue.
```

---

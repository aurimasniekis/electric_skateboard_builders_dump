# *Revised* Wiring diagram for 8s 10,000mah build

### Replies: 9 Views: 1029

## \#1 Posted by: jak Posted at: 2016-09-15T19:00:55.243Z Reads: 157

```
I drew up a wiring diagram for my 8s build. Trying to keep this as simple as possible. Im looking to hardwire the connections that dont need to be disconnected. Should i add an on off switch or is it unnecessary. If so where should it go? And is there a popular one people use. This is hand drawn so if it is hard to read i will try to redo it on the computer. Does the wiring look correct? The batteries will be taken out to charge and used with a paraboard and an imax b6.

<img src="/uploads/db1493/original/3X/9/9/9980a50efe10b489d3af972fda573e86a05d102d.jpg" width="690" height="388">
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-15T19:07:06.288Z Reads: 150

```


[quote="jak, post:1, topic:9646"]
Does the wiring look correct?
[/quote]

At first glance it seems ok but it would be good if somebody else would also have a look!
[quote="jak, post:1, topic:9646"]
Im looking to hardwire the connections that dont need to be disconnected
[/quote]
Bad idea! If some parts get broken you have to replace it. Thus it would be better that you make on every module a connector for easy maintance. You already drew that in your wiring :ok_hand:
[quote="jak, post:1, topic:9646"]
Should i add an on off switch or is it unnecessary
[/quote]

If you dont add a switch you will always need to detach some cables to shut it off. otherwise your system will always drain the battery --> bad idea.

I would add the switch before the display. That way you lcd will shut off when you shut off your board. Otherwise the lcd will always be on and drain the battery.
[quote="jak, post:1, topic:9646"]
And is there a popular one people use.
[/quote]

Yes, the Vedder switch (vedder anti spark switch). [In the next time i will offer some switches for the european room.]
```

---
## \#3 Posted by: jak Posted at: 2016-09-15T19:17:45.430Z Reads: 119

```
what i meant by hard wiring ones that don't need to be disconnected i was mostly referring to the batt. indicator and where the two sets of lipos combine. im just trying to cutdown on bulk and chance for disconnections do to vibration. are you saying those should also be modular? i will look into the vedder switch. would that make the XT90-s where the vesc is redundant? if so i will just change that to a standard XT90 correct? thanks @DeathCookies
```

---
## \#4 Posted by: Namasaki Posted at: 2016-09-15T19:27:50.953Z Reads: 111

```
At a glance it appears that you are connecting in series and then in parallel. 
I would connect the packs in parallel first and then in series because I believe it would simplify the wiring. 
Also it appears that your voltage meter is wired to be always on. Better to have it down stream from the anti spark plug.
You might consider 5.5mm bullet connectors. Easier to solder and less bulky than xt90s. Also they keep pos and neg more separated to better prevent shorts. 
And they make connecting in series as easy as pie.
I'm curious how you plan to charge the batteries. 
8s charger?
```

---
## \#5 Posted by: jak Posted at: 2016-09-15T19:40:02.633Z Reads: 106

```
there is no antispark in the photo. that is why. it was before i decided to in fact add a switch. if i used bullet connectors, every time i took the batteries out and then put them back in i would have to "think" about which were being connected and to where? i.e. the pos to neg for what is in series vs. parallel. i spent quite a bit of time on this diagram as this is not my forte. i feel like im getting more confused. they will be charged with imax b6 and this paraboard. slow to charge but not a problem. kinda why i was using the xt90. im discharging in 8s but charging in 4s.
<img src="/uploads/db1493/original/3X/5/4/549149d4a8abbf8bc7ef14658288acb0caa5d984.png" width="681" height="345">
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-09-15T19:45:48.664Z Reads: 94

```
[quote="jak, post:3, topic:9646"]
i will look into the vedder switch. would that make the XT90-s where the vesc is redundant? if so i will just change that to a standard XT90 correct?
[/quote]

Yes, thats correct.[quote="jak, post:3, topic:9646"]
what i meant by hard wiring ones that don't need to be disconnected i was mostly referring to the batt. indicator and where the two sets of lipos combine
[/quote]

Well, i would prefer to make an adapter for parallel and for series that you can always just buy a new battery and replace it on the fly. [quote="jak, post:5, topic:9646"]
if i used bullet connectors, every time i took the batteries out and then put them back in i would have to "think" about which were being connected and to where?
[/quote]

Not really :D Preferrably you would make a red wire for the positive and a black for the negative. Then you just have to connect red with red and black with black. That simple :D[quote="jak, post:5, topic:9646"]
im discharging in 8s but charging in 4s.
[/quote]

You can connect each battery to the para board. that will work.

No problem dude ;)
```

---
## \#7 Posted by: Namasaki Posted at: 2016-09-15T23:29:54.918Z Reads: 76

```
You could get 2 of these and just connect them in series. 
Then you only have 2 packs to charge. 
http://www.hobbyking.com/hobbyking/store/__16226__ZIPPY_Flightmax_8000mAh_4S1P_30C.html

And bullet connectors make it even more simple. 
Example:
<img src="/uploads/db1493/original/3X/b/c/bc022cb17de76b77561c1209eb73a67b3b40429e.jpeg" width="372" height="500"><img src="/uploads/db1493/original/3X/a/a/aa00d76d264e2c95f657ca1d895ba13e669484ad.jpeg" width="375" height="500">
```

---
## \#8 Posted by: jak Posted at: 2016-09-16T20:56:19.989Z Reads: 58

```
First off thanks @Namasaki for pointing out the redundancies in my wiring. reasons i dont want to use those packs. 1: they are bulky 2: 4 packs allow me to lay them flatter for a more streamline look. 3: those packs only add up to 8 amp hours vs the 10 amp hours of the 4 packs = less time on the board. 4: they are roughly $20 more then using 4 packs. below i added a new, less chaotic wiring diagram with the anti-spark switch added. i also added the bullet connectors like you said for less bulk. you have many good points and i appreciate all the input. if you dont mind reviewing this again i would be grateful. since the lipos will be wired in parallel first, will it be a problem for them to share a bullet conector with each other while charging (discharge side)? they will be charged with seperate XH connectors on the paraboard. so i dont think it will be a problem as long as nothing is connected to the shared bullet, but im not the expert. Also thank you @DeathCookies for the quick answers to my many questions about the wiring and anti-spark switch. 

<img src="/uploads/db1493/original/3X/e/0/e07450115157ba75cd01e61f12abb2836b2c53af.jpg" width="690" height="388">
```

---
## \#9 Posted by: Namasaki Posted at: 2016-09-16T21:55:57.684Z Reads: 53

```
The diagram looks correct. 
If your going to use a parallel balance board then you will be parallel charging so you could permanently connect each 2 pack set in parallel however it would be better to use 2 parallel adapters so that if you encounter a problem (like a dead cell in one pack)
It will be much easier for you to separate and test your packs individually to locate and replace the bad pack. 
Lipos are powerful but they are also fragile. 
You can ruin a pack by simply over discharging it one time. 
I trashed 2 brand new 6s packs by just running them a little longer than I should have. 
Running Lipos in parallel is doable but not optimal. 
You might want to balance charge them to full individually the first time before connecting them in parallel.
```

---

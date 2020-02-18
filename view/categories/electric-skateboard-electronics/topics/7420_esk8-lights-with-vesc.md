# Esk8 Lights with VESC

### Replies: 15 Views: 3393

## \#1 Posted by: sandrewvdv Posted at: 2016-08-10T11:11:45.122Z Reads: 408

```
So I want some front and rear lights on my E-board.
I've read this whole thread :
http://www.electric-skateboard.builders/t/electric-skateboard-lights-headlights-thread/199/41

In this thread there was a mentioning of these products:

- GT Power Large 1/8 to 1/5 Scale Bright LED Kit Off-Road Lighting System
https://www.amazon.com/GT-Power-Bright-Off-Road-Lighting/dp/B00C1BZT3E/ref=redir_mobile_desktop?ie=UTF8&psc=1&ref_=ya_aw_od_pi

- Integy RC Hobby BAJ168 Complete LED Light Kit (4 Front+Brake) w/ KM Type Control Box https://www.amazon.com/Integy-Hobby-BAJ168-Complete-Control/dp/B006957TRW/ref=pd_sim_sbs_21_2?ie=UTF8&dpID=51g0JBiC21L&dpSrc=sims&preST=_AC_UL160_SR160%2C160_&psc=1&refRID=79NNFDRWDR1ECECC1A7B

Which of these 2 are better? how do you connect them to your VESC? Do you need an extra battery, or does it get its power through the VESC?

I'm using a Winning remote, it has a switch for enabling a second channel. I also have a VESC.
I must add, I would like to directly connect it to my VESC. Vedder has ma de video in the past showing that it is possible, but I simply cannot find a well documented guide to set this up.
Video: https://www.youtube.com/watch?v=G8f0xg7DNmM

Thanks
```

---
## \#2 Posted by: Nordle Posted at: 2016-08-10T11:28:53.287Z Reads: 373

```
You'll need a step down module (or ubec), cause the build in one from the VESC can't handle the current you're lights draw.
```

---
## \#3 Posted by: sandrewvdv Posted at: 2016-08-10T11:51:44.307Z Reads: 365

```
In the other discussion there no mentioning of a ubec. I thought it could be powered directly trough the vesc
```

---
## \#4 Posted by: Nordle Posted at: 2016-08-10T11:52:44.897Z Reads: 355

```
Maybe you can but i won't do it. Cause it's not safe
```

---
## \#5 Posted by: jrpwit Posted at: 2016-08-10T12:22:07.467Z Reads: 336

```
Most people power their lights from a set down converter connected to their headlights. A ubec is not necessary but it is another option.
```

---
## \#6 Posted by: sandrewvdv Posted at: 2016-08-10T12:31:38.970Z Reads: 329

```
I would like to connect it directly to my vesc. It has  been doneby Vedder, but I cant find a tutorial on how to do it
```

---
## \#7 Posted by: jrpwit Posted at: 2016-08-10T12:38:32.729Z Reads: 325

```
Same story bro. The nunchuk turn signals are super cool that he showed.
```

---
## \#8 Posted by: Skitzor Posted at: 2016-08-10T19:09:47.798Z Reads: 315

```
I've been looking into this too, I already ordered an st-link to modify some code onto the vesc.

But here is a huge difference. 

The kits mentioned above have a control box which analyses your ppm signal (front brake left right) and switches lights on accordingly.
Vedders mod on video is a multicolor ledbar which he assigns colors and brightness to according to the vesc signals.

There's also someone on this forum who did the same with led-bars and different colors for what speed he's going at. His name escapes me at the moment...
```

---
## \#9 Posted by: Pedrodemio Posted at: 2016-08-10T19:17:45.504Z Reads: 297

```
Not directly by VESC, but with an Arduíno, the same one i use for the remote

https://www.instagram.com/p/BH7vnD4D_Dx/?taken-by=pedrodemio
```

---
## \#10 Posted by: cjoliver Posted at: 2016-08-10T19:43:17.631Z Reads: 272

```
I've seen a BOM list for the VESC and it shows a 3.3v regulator, and I've seen enertion specify 5v at 1A. To really know if you can pull power from the VESC you need to look at the voltage regulator and look up the part number and find the specs. Then you need to figure out how much power(in amps) your lights are gonna pull and see if the amps pulled is less than what your part supports.
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-10T19:44:12.516Z Reads: 259

```
Maybe @Michaelinvegas can chime in on how he does his :)
```

---
## \#12 Posted by: Namasaki Posted at: 2016-08-11T04:41:00.533Z Reads: 243

```
Now that is Sick!
```

---
## \#13 Posted by: sandrewvdv Posted at: 2016-08-11T11:04:19.367Z Reads: 231

```
So with the sets linked above, it is possible to have a working front and rear light that responds to the action on your remote?
```

---
## \#14 Posted by: Skitzor Posted at: 2016-08-11T11:26:49.329Z Reads: 226

```
@Pedrodemio do you have any info on your build posted here somewhere? Hard & software.
```

---
## \#15 Posted by: Pedrodemio Posted at: 2016-08-11T15:25:57.662Z Reads: 214

```
Not yet, I still have some problems on the drivetrain, but as soon I finish I will do a build thread
```

---

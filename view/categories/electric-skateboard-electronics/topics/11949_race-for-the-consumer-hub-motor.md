# Race for the Consumer Hub Motor

### Replies: 15 Views: 1465

## \#1 Posted by: KMeyerson Posted at: 2016-10-26T17:12:04.088Z Reads: 186

```
Probably about to change significantly.

http://newatlas.com/acton-blink-qu4tro-skateboard/46100/

So I might as well pack up shop at this point :-P.  It looks like they've also given up trying to squeeze more than 7.5Nm per motor.
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-10-26T17:32:43.508Z Reads: 179

```
I hate the thought proprietary wheels...

Kills the whole unique build idea
```

---
## \#3 Posted by: Hummie Posted at: 2016-10-26T17:42:00.170Z Reads: 169

```
@KMeyerson dont believe it till you see it. Theyre all after a buck and will claim anything.  that article you linked it seems the author just cut-and-pasted all the stats presented by the sellers.  No verification and so many are known bogus.
```

---
## \#4 Posted by: KMeyerson Posted at: 2016-10-26T17:44:30.840Z Reads: 161

```
They've had several successful campaigns before and they have a working prototype.  Its pretty safe to say they're doing alright.

I've backed them.

I'm just livid at how similar their deck is to one I shared here months ago.  In the end, it's all just design soup.
```

---
## \#5 Posted by: Mikenopolis Posted at: 2016-10-26T17:59:12.169Z Reads: 150

```
I'm already sold on the hub motors (will be my next build). 4WD's idea is great if you need the torque, but you now have 4x the potential for failure (repair cost), increase weight and battery consumption.

My first board was Acton's original Blink board which still works well for me. It was the reason I did my first build. I have read that others have had problems with their boards, but I really never pushed that board's limit because I know it's underpowered for a 210 lb 6'0" person like myself and it's really scary even at 13mph. From MY experience, Acton puts out good products, but like most companies, don't trust their numbers as they are usuallu using "optimum" testing conditions
```

---
## \#6 Posted by: KMeyerson Posted at: 2016-10-26T20:02:18.032Z Reads: 131

```
True. Each motor puts out 7Nm or torque more or less.

That's how they stay cool. I want two motors that put out 15Nm each
```

---
## \#7 Posted by: Hummie Posted at: 2016-10-26T20:16:00.678Z Reads: 125

```
 based on the size of the hub motor I highly doubt anywhere near 7newton meters torque per motor

heres a link and quote from Christian Lucas who designs motors for a living
:The torque belong to the of the stator . So dia is not all ,we need the lengh of the stator . Dia x pi x lengh = surface . Than there are some numbers you can use to find the torque. Formthe first aircooled outrunner we calculate with about 2,5 newton trust per square centimeter of the statorsurface. Short aircooled outrunner reach about 8 newton/cm2 for some seconds lime used for recordairplane ,maybe higher ,aske R.Okon what he currently run . Liquide cooled motors do about 8 newton continius trust and 12 newton for short periode and up to 16 and higher for very short time . Maybe someone can do moore .
Example : Stator with 63mm dia and 20 mm lengh . 6,3 cm dia x pi x 2 cm lengh = 39,6 cm2 x 2,5 newton = 99 newton trust produced x leverarm of the rotorbell ( 0,063 meter /2) = 3,1 newtonmeter torque . So with 16 newton per cm2 you can have about 20 newtonmeter Torque. This is a rule of thumb estimate ,but gives a number . 

https://www.rcgroups.com/forums/showthread.php?t=2445172
```

---
## \#8 Posted by: KMeyerson Posted at: 2016-10-26T22:27:31.427Z Reads: 111

```
I would disagree. I've been zimulating motors in Infolyticas MotorSolve before I wind them and you can push a lot out of a 51.8mm stator with 30mm Length.  The trouble is for how long.

I've been taking advantage of magnet/slot ratios.  46 poles seems to do wonders to torque.  Problem is assembly.
```

---
## \#9 Posted by: Hummie Posted at: 2016-10-27T02:19:46.163Z Reads: 101

```
is that how big their motor stator is.52x30?  i sold 47x25.  that fit in an 80mm wheel but they do 70mm.  
As you say" for how long".  (you run simulation software!  nice I never could sit long enough) how efficient would the motor be if it were to put out such a torque?  I imagine the stator would become magnetically saturated and copper losses would go way up.

maybe you could do some simulating for me?  Id like to know how the different magnet sizes effect things, 80% fill vs 100% 
How much more efficiently will the motor run with 90kv at 20mph on 12s vs max speed on 60kv at 20mph on 12s
```

---
## \#10 Posted by: NickTheDude Posted at: 2016-10-27T02:40:53.171Z Reads: 95

```
This could be somewhat off topic, but from what I've read about the issues with hub motors, isn't a planetary gear like the one used in Stary a good solution?
```

---
## \#11 Posted by: Hummie Posted at: 2016-10-27T02:44:32.200Z Reads: 95

```
in a way maybe a solution but take into account all the space taken up by the planetary gear and you now have a small motor, that now makes so much noise it's not like a hub motor
```

---
## \#12 Posted by: KMeyerson Posted at: 2016-10-27T10:06:04.393Z Reads: 74

```
The trouble with simulations is getting the settings right.

I assume the VESC switches at 16Khz among many things which probably messes up my numbers consistently.  I only recently discovered the Hysteresis vs Space PWM setting.

What I need is to compare a simulation to a real life model to iron out the settings for accuracy. If you have a chance, PM me @Hummie about your gauge, strand count, and turns. I think I've got an old schematic for your stator and magnets somewhere from an early post of yours.

I'll let you know what the program thinks is getting spit out in terms of torque and temp.
```

---
## \#13 Posted by: KMeyerson Posted at: 2016-10-27T15:59:53.920Z Reads: 46

```
I don't know but its the stator found in most 63mm motors. I figure since their hub motors are 99mm diameter total, they're probably not making it any bigger than 63mm (more thane!)
```

---
## \#14 Posted by: Hummie Posted at: 2016-10-27T16:10:19.859Z Reads: 45

```
blink lite is 70mm wheel

woo 300$ for the complete board on the site.  sold at best buy!  wow becoming more mainstream.  at that price.. and considering every other hub motor that's come out...  we will see
```

---
## \#15 Posted by: KMeyerson Posted at: 2016-10-27T16:35:46.968Z Reads: 39

```
Yeah... Its not great for us tbh.

I booked one of the 4WD boards just to be able to ride it. I'll probably resell it for the full value when I get it and study it for a week.
```

---

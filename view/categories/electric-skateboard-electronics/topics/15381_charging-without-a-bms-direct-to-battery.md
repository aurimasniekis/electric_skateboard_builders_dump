# Charging without a BMS (Direct to battery)

### Replies: 14 Views: 3808

## \#1 Posted by: Alextech Posted at: 2016-12-30T07:06:29.146Z Reads: 195

```
I'm trying to use a 42v charger on a 18650 pack I have since I don't have anymore bms to play around with.  I get a clinking noise from it and a flickering of the red charging light.  I know I'm missing something,  any insight might be great
```

---
## \#2 Posted by: PXSS Posted at: 2016-12-30T07:23:41.716Z Reads: 195

```
You're missing a bms...

On a more serious note. You should not connect a wall wart directly to your batteries, the charger never stops... kinda like what happened with the exploding  hover boards...
```

---
## \#3 Posted by: Alextech Posted at: 2016-12-30T07:55:09.979Z Reads: 184

```
Well, I think people have done it before here on the threads.  Just curious on how they did it.
```

---
## \#4 Posted by: jbruce Posted at: 2016-12-30T08:17:31.564Z Reads: 176

```
If you have a charger at the correct voltage for your cells this should work. Lithium battery chargers are made specifically to turn off once they reach the fully charged voltage of your pack, and these are generally the one you want to use because lithium cells unlike lead acid do not like or need trickle charging. However, you could use a normal power supply at the correct fully charged voltage of your cells to charge them, just you would want a voltage and amperage meter to know when the pack is fully charged so that you could disconnect it from your cells and not trickle charge them. If you use a correct battery charger on your cells and they are high quality, you can go with out a bms because the drift is very small. As for the clicking noise your charger makes...it's probably broken :joy: if you have a voltage and amperage meter you could check to see if it's still working.
```

---
## \#5 Posted by: Maxid Posted at: 2016-12-30T09:33:36.237Z Reads: 151

```
What?

A CC/CV charger will work without a BMS. No charger would naturally stop - ever. All they do is follow a preprogrammed threshold and stop charging once the current in the CV phase goes below a certain level.
```

---
## \#6 Posted by: PXSS Posted at: 2016-12-30T10:35:10.587Z Reads: 144

```
I thought he meant he was using a regular 42v wall wart kind of charger, one that would not know when to stop charging your cells.

Per almost every 18650 spec sheet you should not be in cv mode for longer than 2 hours, otherwise you start damaging your cells, if you have them on a charger that is even a slightly bit above 4.2, you are now over charging and are damaging your cells. 

18650 cells are most dangerous when fully charged or overcharged, it is also when they degrade the most. If a battery is left unattended on the charger for hours, you will damage its performance best case scenario in my experience. 

If you are going to be there to stop the charge after a few hours and never forget then yeah, just get a power supply at the right voltage and hopefully you'll never forget.
```

---
## \#7 Posted by: jbruce Posted at: 2016-12-30T10:35:15.061Z Reads: 130

```
I'm pretty sure only lithium specific chargers turn off at the end of the CV phase. Normal power supplies are made to deliver a voltage and not turn off. Imagine your computer power supply wasn't delivering a lot of current and just turned off...lol that wouldn't be good. But like I said you could use a normal power supply as long as you monitor the charging and unplug it manually when it's done charging.
```

---
## \#8 Posted by: Maxid Posted at: 2016-12-30T10:53:53.579Z Reads: 125

```
At the end of CC phase? There definitely has to be CV phase also or you are not charging the batteries fully.
Also I am not sure what my post has to do with yours.
```

---
## \#9 Posted by: PXSS Posted at: 2016-12-30T10:58:29.704Z Reads: 115

```
He meant cv phase. He's trying to make the same point I was... :slight_smile:
```

---
## \#10 Posted by: Maxid Posted at: 2016-12-30T10:59:23.220Z Reads: 114

```
I don't get your points and what they do have to do with the initial question.
```

---
## \#11 Posted by: PXSS Posted at: 2016-12-30T11:02:31.038Z Reads: 106

```
Yeah, I guess we both failed... lol
I did not think the op meant a cc/cv charger in his original post, therefore why I said it could be dangerous if left unmonitored. That was the main takeaway I think lol
```

---
## \#12 Posted by: Baz_L Posted at: 2016-12-30T12:17:55.858Z Reads: 104

```
A good rule of thumb to use is that if it says 'charger'/anything lithium ion related on the back it will cut the voltage, but if it says 'adapter' the likelihood is that it will not cut out (note that there are exceptions to this due to poorly labelled Chinese products, but that is the standard way of telling).
```

---
## \#13 Posted by: Baz_L Posted at: 2016-12-30T12:22:53.612Z Reads: 106

```
@Alextech could you send us a photo of the charger in question? (Specifically the info on the back). If it is a 42v lithium ion charger there shouldn't be any issues, provided that your cells are already balanced (any changes of +/- 0.1v could easily ruin your cells). 

If they're perfectly balanced at the start, and are new cells, there shouldn't be any problems with charging that way. Drift shouldn't really be an issue in the first 50 cycles at least. I would highly recommend getting a BMS though, they're not expensive and could save your batteries in a freak accident where the charger fails (which can easily happen if it's not a high end charger..)
```

---
## \#14 Posted by: jbruce Posted at: 2016-12-30T19:38:58.101Z Reads: 93

```
@Maxid @PXSS yes my bad I meant CV phase. I just edited it for no further confusion. Getting back to the original question, if the charger is making a clicking noise either there is a fan in it that's not working properly or the charger is most like broken and probably shouldn't be trusted with your cells.
```

---

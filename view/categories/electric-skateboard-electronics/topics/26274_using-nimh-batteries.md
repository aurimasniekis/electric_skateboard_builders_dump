# Using NiMH Batteries

### Replies: 9 Views: 1083

## \#1 Posted by: OverHillier Posted at: 2017-06-27T15:26:10.433Z Reads: 126

```
I have came across a big box of perfectly fine 2200 mah NiMH at work. I haven't been able to find much about about using them for an esk8. So my question is what are the downsides to using them, besides the energy density? Also what are some things that I wouldn't need to worry about vs say lipo's?
```

---
## \#2 Posted by: Challlsss Posted at: 2017-06-27T15:33:05.424Z Reads: 124

```
You should test the internal resistance of the cells and see how they do. Also figuring out the model so you can determine their maximum discharge will be handy
```

---
## \#3 Posted by: wmj259 Posted at: 2017-06-27T16:57:12.257Z Reads: 114

```
You are going to need a lot of batteries In series to get the same voltage as lipos or lions. About double per each cell.
Nimh 1.7V
```

---
## \#4 Posted by: OverHillier Posted at: 2017-06-27T17:52:32.361Z Reads: 103

```
The batteries are 2200Mah, 1.2V in C cell form. They are produced by GP Batteries. So to get say a 12S1P setup I would need (44.4V/1.2V = 37) 37 Batteries in series. Which I believe there may be around 50-60 of them. 

@Challlsss I don't have a multi meter with me at the moment, but can check the resistance when I get the chance.
```

---
## \#5 Posted by: sl33py Posted at: 2017-06-27T18:58:35.323Z Reads: 89

```
you could also mount a pair of car or motorcycle batteries on top of the board because you have them...  but unless you are trying to recreate the 70lb esk8 of a few years ago - why?

(edit - forgot newer NiMH don't have typical memory issue)

Bigger issue:
Amp delivery (Sag, heat, poor performance/range).

Seriously - 37 in series?  at 1p?  so you think 1c delivery will work ok for esk8?  2.2Amps might not even turn your motor.  (during VESC motor detection i know sometimes i need more than the low start value)

You will need LOTS in parallel to get even 20-30a to really push you along.  HUGE SAG.

If you have some spare time and just want to play with it - i get it and have fun, but this will not work well without a huge parallel pack!
```

---
## \#6 Posted by: smurf Posted at: 2017-06-27T19:06:37.995Z Reads: 82

```
If I had a box of free batteries I would use them to practice welding or soldering fuse wires on.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-06-27T20:09:47.927Z Reads: 74

```
the only downside is that they are heavy and dont last as long.
other than that a battery is a battery.
```

---
## \#8 Posted by: sl33py Posted at: 2017-06-28T00:05:27.035Z Reads: 59

```
[quote="lowGuido, post:7, topic:26274"]
other than that a battery is a battery.
[/quote]

I'm not sure i agree and am going to give you a hard time here.

a battery is a battery?  So what current in Amps do you consider minimum required to esk8?  I would set it reasonably in the 30-40A range - just cruising flats and single motor.

not knowing the actual c rating of the NiMH batteries - i'd bet around 1c, but hope i'm wrong.  if 1c(2.2A) 10 x 37 (to get 22A and 12s voltage) = 370 cells!

that's not a battery, that's a rolling lead weight!  No way you could get it to fit on a normal board.  

I see this equivalent to "i found 100 used laptop 18650 batteries and want to make a pack!" discussions.  Can you do it with time and testing - sure.  But at the end of it you likely have a 20lb battery that barely runs your esk8, and probably overheats the cells and becomes unbalanced quickly.  My definition of PITA with time and problems to keep fixing.

Now if you find a steal on some used high drain batteries, test them and group them by tested capacity and resistance... that's a different story.  Building from like tested cells vs a bunch of random cells of poor performance...

Still a lot of work.  I'd look on nkon and others for legit quality new cells if you want to go that route.

I'm no custom DIY battery expert - my .02 so YMMV.
```

---
## \#9 Posted by: lowGuido Posted at: 2017-06-28T02:14:06.391Z Reads: 45

```
I used to use NiMh in my high current RC car applications and we would flog the shit outa them till they would almost burn up. (But they didnt)
 For like the last 20 years high torque  power tools used nimh before lithium became an option. There are good nimh out there and they could work if you wanted them to. 

They arent the best option. Of course it wont be as good as lithium.  Thats not the question.  The question is can you use them? Answer is yes.
```

---

# How-To Charge Lipos?

### Replies: 11 Views: 418

## \#1 Posted by: DuskisNigh Posted at: 2018-07-17T17:11:06.952Z Reads: 139

```
I have to charge the batteries…thought it would be relatively simple…of course not.

I have a Turnigy Reaktor Pro 350W 23A power supply and a Turnigy Reaktor 250W 10A balance charger/discharger and a 40A Paraboard (not sure if I even need this) and a harness for in series battery use.

I don’t know what goes into what and how to program the balance charger/discgarger and I've searched everywhere to find out how.

I’d be much obliged for help.

![20180622_204616|374x500](upload://zyj5Pcq95eQwxv0Ozpo5aW3iBf.jpg)
```

---
## \#2 Posted by: wafflejock Posted at: 2018-07-17T17:17:53.323Z Reads: 131

```
Yah so power supply plugs into the wall converts power from AC->DC.  The power supply gives DC power out to the input power of the charger itself.  The parallel board I would skip on for the time being until you have the basic charging stuff figured out.  Once you have power going to the charger you should be able to select LiPo charge or LiPo Balance charge (ideally) from the list.  The main battery cable and balance lead plug from the battery into the balance charger directly for now (skipping the parallel charger).

Once you have everything hooked up when you select balance charge most of the time you have to hit start to get the charger to show you how many cells it senses connected to the balance port and then you hold start to actually start charging (this interaction may vary some).

The parallel board you use if you want to hook multiple batteries to the charger but for the moment I would skip on it to avoid extra complications.  You'll want to be sure your batteries are very close to each other voltage wise before plugging into the board (looks like you grabbed the one with fuses which will help avoid accidentally rapid charging from one with more voltage to one with less voltage, you want them to be within .2-.3 V of each other overall typically if you are going to parallel charge, when you hook in parallel the batteries/cells will 'self-balance' with other cells they are hooked up to through the parallel board.

---

Only things to note are when you go to start charging you need to be sure the Amperage is set to something less than 1C for your battery (looks like 8Ah so just needs to be less than 8A) and you need to be positive the voltage/number of cells in series on the charger matches the reality.  If the charger thinks it's a 5S battery but it's a 4S it would be pushing the voltage far too high (typically they have safeties built in to avoid letting this happen), other thing is to make sure Amperage is limited so you aren't excessively cooking the battery while charging.
```

---
## \#3 Posted by: E1Allen Posted at: 2018-07-17T20:42:05.384Z Reads: 111

```
YouTube!!!
```

---
## \#4 Posted by: wafflejock Posted at: 2018-07-17T21:03:15.599Z Reads: 108

```
Sure can youtube for generic instructions, if you have specific questions @DuskisNigh let us know.

In particular recommend watching this before using the parallel board at all:

https://www.youtube.com/watch?v=mRlsaD5tf_8
```

---
## \#5 Posted by: DuskisNigh Posted at: 2018-07-21T19:01:46.771Z Reads: 90

```
thank you for the run down.  the problem I'm getting is in the picture.

I don't know what "cell low volume" means.

![20180721_145937|374x500](upload://qUojO73yD67564ERAD4fhE5Y1lE.jpg)
```

---
## \#6 Posted by: E1Allen Posted at: 2018-07-21T19:19:23.867Z Reads: 85

```
So long as you plugged in the balance plug it means the voltage of at least one cell is below the limit the charger allows for balance charging.  I've either had to do lipo charge to bring all the cells up, insert a tiny plug to one cell from the balance Port to bring the low cell up, or do NIMH charge on the one cell slowly to bring it up.  Hopefully that cell or cells aren't toast.
```

---
## \#7 Posted by: wafflejock Posted at: 2018-07-21T20:23:53.898Z Reads: 82

```
Like @E1Allen said one of the cells is reading too low a voltage, VOL for voltage in this case double check the voltage from the balance leads (can use a lipo battery tester or look up how to check them on the balance connector with a multimeter).  If any cell is below 3.0 typically chargers won't attempt to charge them, could be loose connection or over drained cell.  If over drained probably need to just replace the battery.  You can do the nimh "trick" but personal experience is that's a short term fix.
```

---
## \#8 Posted by: DuskisNigh Posted at: 2018-07-25T15:49:39.521Z Reads: 69

```
So I did the Nimh charge and it worked great on one but it doesn't seem to be working on the other.  how do I know if the battery is busted or not? 

Also, how long can I do the Nimh charging thing on a Lipo?
```

---
## \#9 Posted by: E1Allen Posted at: 2018-07-25T22:16:43.828Z Reads: 60

```
I only do it to like 2.7 or 2.8v per cell I think.  Have to bring it up to minimum level for lipo charging. It's somewhere around there. Not sure exactly.
```

---
## \#10 Posted by: DuskisNigh Posted at: 2018-07-29T12:32:30.745Z Reads: 48

```
how do I bring up the voltage on just one cell with the batteries i have?

should i discharge them completely and then try the nimh charge trick?
```

---
## \#11 Posted by: E1Allen Posted at: 2018-07-29T14:00:08.661Z Reads: 45

```
![image|375x500](upload://hsg2JXHEXu6y7dLLrKMxAWWSlmc.jpeg)You can't discharge completely because the low cell will drop even further below what is supposed to be.  I made a little connector that fits into the balance plug.
```

---

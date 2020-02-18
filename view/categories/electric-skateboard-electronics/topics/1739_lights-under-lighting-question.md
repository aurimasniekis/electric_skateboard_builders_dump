# Lights + under lighting question

### Replies: 10 Views: 1730

## \#1 Posted by: barajabali Posted at: 2016-03-09T16:05:44.489Z Reads: 408

```
Hey guys so on my board i have under lighint and head lights .  The head lights need 5-8v and the under light is 12v.  What i did is just run the 5-8 v to the 7.2 output on my battery and the 12 to the 11.1.  IT actually works fine ive riden it miles and for weeks too.  But my battery crapped out and its pretty new.  I use two Lipos and the one that the lights are connected to is the one that crapped out.  

My question is, do you think it is because of the lights connected to it?
```

---
## \#2 Posted by: Sebastiaan Posted at: 2016-03-09T16:08:54.122Z Reads: 405

```
Not sure about the lipo damage. Why don't you use a sBEC for the lights ?

http://www.hobbyking.com/hobbyking/store/__72700__Turnigy_Multistar_Twin_Output_5_10_Amp_6_50V_SBEC_for_Lipoly.html
```

---
## \#3 Posted by: barajabali Posted at: 2016-03-09T16:10:51.690Z Reads: 397

```
frankly because my option was free. also there is no sBEC for 12v. just for 5.  So id have to connect to the battery anyway
```

---
## \#4 Posted by: mattdig Posted at: 2016-03-09T16:21:34.431Z Reads: 385

```
The SBEC posted above is dual voltage, 5v and 12v, so it's exactly what you need. The battery is probably dead because you're drawing power from the the cells at different rates and they got way out of balance.
```

---
## \#5 Posted by: barajabali Posted at: 2016-03-09T16:35:20.944Z Reads: 362

```
Oh I'm sorry @Sebastiaan 

Thanks I didn't even know they came in dual! Perfect. Now I have to see if i can fix my battery lol
```

---
## \#6 Posted by: Sebastiaan Posted at: 2016-03-09T16:37:26.178Z Reads: 348

```
Hehe, i'm using one in my setup, works great, before i used two becs, saves some space and wiring.

What exactly is the problem with the lipo? Do you have a multimeter to check all the cells on the balance port?
```

---
## \#7 Posted by: trbt555 Posted at: 2016-03-09T16:41:28.217Z Reads: 338

```
You probably over-discharged that lipo by connecting directly to it. lipo's don't like that.
```

---
## \#8 Posted by: barajabali Posted at: 2016-03-09T16:42:47.895Z Reads: 335

```
Yes I checked every cell they are all reading correctly with the multimeter but when I plug it in to my voltage reader it goes all strange reading 8 cells some with 100 percent and some with 0 and some blanks. Now if I wiggle some connections for a little then it'll read correctly 1-6s all at 85%. But the second I plug it into my board and turn it on a huge spark flys out of the negative main terminal of the lipo.

I've ruled out a connection issue. 
I've ruled out faulty battery reading devices

The lipo is either shorteD internally (even tho it can read the correct number sometimes)
OR
It's shorting on the cell itself because they're aluminum I'm pretty sure.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-03-09T17:10:36.445Z Reads: 319

```
Better keep that lipo in a safe location, you don't want it shorting out on its own when you're not around.
I keep mine in an old cooking pot.

If you're feeling adventurous, you could remove the shrink-wrap and have a peek inside to see if you can't find the fault.
```

---
## \#10 Posted by: barajabali Posted at: 2016-03-09T17:14:38.825Z Reads: 310

```
Oh I took it out of there already. I had to change the oreontation of the cells. Yea maybe i should just junk it.
```

---

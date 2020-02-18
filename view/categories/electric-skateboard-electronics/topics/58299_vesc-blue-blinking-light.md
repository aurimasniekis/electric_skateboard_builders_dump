# VESC Blue blinking light

### Replies: 13 Views: 397

## \#1 Posted by: sodniwe Posted at: 2018-06-09T02:13:16.067Z Reads: 79

```
Hello!
I'm having some issues connecting my battery to my VESC.  Whenever I connect the battery the blue light on the VESC blinks very quickly.  I have a different battery that I hooked up and it worked fine.  The battery that worked fine was a 12S 3P battery pack.  I'm trying to connect a 14P 5S pack but it doesn't detect the device VIA USB and the blue light keeps blinking.  I think its an issue with the battery itself.  Has anyone else encountered / solved this issue.   I can't wait to get riding! Thanks!

Vesc i'm currently using: collections/featured-items/products/torque-esc-bldc-electronic-speed-controller
```

---
## \#2 Posted by: wafflejock Posted at: 2018-06-09T02:17:21.296Z Reads: 74

```
Did you check voltage on the battery are there any signs of damage on the vesc?  Does it still work if you use the other battery.  Would suspect voltage settings causing issued maybe but would be good to have more details and ideally pics.
```

---
## \#3 Posted by: sodniwe Posted at: 2018-06-09T02:19:56.501Z Reads: 74

```
Hello Waffle!
It works when I use the other battery without any problems.  It's 100% an issue with the battery but unsure how to figure out what the issue is (it's a battery that a built myself).  The voltage of the battery currently reads 49.8v.  Anything specifically that could cause the issue with the battery / BMS setup I should check?
```

---
## \#4 Posted by: sodniwe Posted at: 2018-06-09T02:28:39.862Z Reads: 66

```
Might have found the issue.  When i Built the battery I got a 16S BMS but the battery I built is only 14S.  Could this be the issue?  Is there any way I can use this BMS with a 14S battery?

![IMG_1116|666x500](upload://zqtPSdHfItvU5AZb6JqKu0JNWbU.jpg)
```

---
## \#5 Posted by: sodniwe Posted at: 2018-06-09T02:48:51.321Z Reads: 59

```
I took apart the battery and found that the reading out of the BMS is 49.6v but when i read the voltage directly on the battery it's 52.1v.  Did some checking on the battery and found a group of cells in parallel that read 1.6v and all the other groups of cells read the correct voltage.  I'm guessing one of the cells in the group is bad?  Could this be my issue?
```

---
## \#6 Posted by: wafflejock Posted at: 2018-06-09T03:43:01.541Z Reads: 51

```
Sorry I'm not familiar with the details of configuring a BMS or trying to use it with less cells than it's designed for really.  Regarding the cells in parallel reading 1.6V if that's in fact a correct reading then I'd guess all the cells in that group have gone bad somehow (since they're all in parallel with each other they should have the same voltage) and if it's 1.6V they're far below the 3.0V limit most cells can deal with before having permanent damage.  I'd double check that and if it still seems low pull it apart and test the individual cells to see if they are all in fact at 1.6V if so think you need to just replace that set.
```

---
## \#7 Posted by: jerry9800 Posted at: 2018-08-20T18:16:42.268Z Reads: 28

```
Hi sodniwe,

does the VESC blink blue several times and then just turn off? 

Thanks
```

---
## \#8 Posted by: sodniwe Posted at: 2018-08-20T18:30:00.443Z Reads: 26

```
@jerry9800.  I was able to resolve my issue.  I believe their the battery had a bad cell group.  The first group of cells in series (1S 4P) all had a voltage of 1 volt which is wayyyyy too low.  I ended up fixing my other battery and will move back to this once when I start working on my electric bike again :D
```

---
## \#9 Posted by: jerry9800 Posted at: 2018-08-20T18:59:35.008Z Reads: 23

```
Hi Sodniwe,

reason why i'm asking was i'm having the same issue and was wondering when this did happen, did the blue light blink several times followed by no LED light being lit at all? I'm trying to figure out if my VESC is not being powered by the battery. This is my first build and i cannot connect it to the computer and want to rule out that as being a cause. 

Thanks so much for you reply =]
Jerry
```

---
## \#10 Posted by: jerry9800 Posted at: 2018-08-20T19:00:29.712Z Reads: 21

```
Also should the vesc have a solid blue light?
```

---
## \#11 Posted by: sodniwe Posted at: 2018-08-20T19:23:44.358Z Reads: 20

```
@jerry9800 It just kept blinking blue.  Did you build the battery yourself?  What are the specs of your battery?  I would recommend checking every cell of your battery to ensure its put together correctly.  If you look at where all the wires go into the BMS you can measure the voltage between each one to ensure it's the correct voltage.

What are the specs of your battery?
```

---
## \#12 Posted by: jerry9800 Posted at: 2018-08-20T20:06:39.031Z Reads: 20

```
Should the vesc have a constant blue light?

My battery is a 10s2p 4ah from ownboard (I’m not that adventurous in making a battery yet lol)

I don’t know if you can help me with this but my battery is connected to a button which is than connected to the vesc. Upon powering, vesc blinks several times and turns off. The blue led on the on/off button is bright upon turning on then dims but is still lit. I will try connecting the battery directly to vesc to see if that changes anything. Right now I’m trying to program the VESC but can’t get it connected to the pc and trying to rule out any problems.

All my connectors are xt60. Don’t know if this makes any difference.
```

---
## \#13 Posted by: sodniwe Posted at: 2018-08-21T01:40:06.449Z Reads: 20

```
Jerry,
You need to connect your battery to the VESC and plug it into the computer at the same time.  You could potentially have a battery issue which is what I ran into.  Have you tried connecting the battery to the vesc and pluugging it into the computer?
```

---

# Battery sucks. Trouble with voltages. Help needed

### Replies: 18 Views: 236

## \#1 Posted by: xsynatic Posted at: 2019-03-19T15:57:10.945Z Reads: 88

```
*Long post*

Hello everyone..

I'm kinda bummed that my battery sucks so hard. I should've informed me more and not buy something because one person recommends it.

I have 2x 12.000mAh Lipos in series.
I currently use them with a single 6374 Motor and 90mm wheels.

EDIT : the box is just to test if it even works. NOT the final enclosure 

Minimum Capacity: 12000mAh
Cell Count: 6 / 22.2V
Constant Discharge: 12C
Peak Discharge (10sec): 24C

I soon upgrade to AT (200mm pneumatics and dual 6374)

I'm a speed person so i often times hit 40-50km/h with my current setup.

If i use my Wowgo 2s i can get 40-50km range with 2x 6.4 Ah battery (If i drive rather slow, if not about 16km per battery) and that range is what i want with my new board.

I really would like to top mount it instead of the bottom if possible but with 18650's its hard to get a compact battery pack.

Does anyone have a recommendation for good batteries.
30-60km range would be great. EU is prefered.
My second "problem" is acceleration.

I use a vesc and the general acceleration is fine but i've noticed that when i get speed sometimes there is a small jolt. It reminds me of driving a car if you shift into next gear and you have a small drop and then a small jump with the further acceleration. Is this normal?


My third problem is Voltage.

If i remember correctly.

Series = double voltage, same range
Parallel = double range, same voltage

But my battery meter shows something different.

Battery meter showed 59% (both batteries connected) and something about 45.x volt.

If i connect one of my batteries to the charger it says 36% remaining. But shouldn't the range be the same if connected in series? The battery meter is programmed for L - 12.

With programmed for 6s the battery meter shows 59% at 22.7 volts
```

---
## \#2 Posted by: xsynatic Posted at: 2019-03-19T18:41:37.102Z Reads: 65

```
Also the VESC tool recommends a soft voltage cutoff at 39.2v which i extremely low isn't it? 3.26v per cell is near dead.
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-03-19T18:47:47.480Z Reads: 60

```
[quote="xsynatic, post:1, topic:87642"]
Does anyone have a recommendation for good batteries. 30-60km range would be great. EU is prefered. My second “problem” is acceleration.
[/quote]


What are the size contraints for your pack? in terms of 18650 cells, as well as 21700/20700s and we can better help you

Can we see pictures of the wiring as well as some links to whatever modules you have to read voltage. 

What vesc are you using? Im not sure it has much to do with your issue but are you using a flipsky vesc? I know their voltage reading ability is a little off
```

---
## \#4 Posted by: Bobby Posted at: 2019-03-19T18:54:07.675Z Reads: 51

```
I think 3.2 sounds right. Not an expert tho
```

---
## \#5 Posted by: xsynatic Posted at: 2019-03-19T18:56:39.085Z Reads: 52

```
So my current enclosure is just a cardboard box with 27x20x8cm where both of my lipos and the vesc is inside.


Mounting wise am i open to mount it on the bottom of needed. (if i go with 18650/21700/20700

the vesc is a torqueboard vesc 4.12.

The battery meter is a lcd cheapo meter from ebay wired onto my cable triangle (battery,loopkey and vesc  xt90 plugs.



![IMG_20190319_195325|666x500](upload://97692PGkjsvXAdxWxDj3xwPzpwh.jpeg) 
![IMG_20190319_185253|666x500](upload://bZa0uzS9dYgqoUENVsta57aLeaU.jpeg)
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-03-19T19:03:42.624Z Reads: 47

```
Homie you might want to upgrade that box. Its completely open to the elements. At the very least you should get a snap to close (please pardon my spelling of this(?)) Tupperware container. 

That would be my first stop :man_shrugging:
```

---
## \#7 Posted by: ninTHIENdo Posted at: 2019-03-19T19:07:01.837Z Reads: 42

```
At least use some gorilla tape or duck tape

Also, is your battery meter lcd configured to a 12s Li-Po?

What kind of range are you getting that it sucks so bad?
```

---
## \#8 Posted by: xsynatic Posted at: 2019-03-19T19:29:17.311Z Reads: 39

```
Its just a protoype box to test if it even works :slight_smile:  

Yes it is configured to L12.

I have yet to test it with a full battery. I tested it with 70-90% and got about 20km+/- with 26% left.
```

---
## \#9 Posted by: xsynatic Posted at: 2019-03-19T19:29:46.110Z Reads: 38

```
Its just a "prototype" box to test if it even works. But yes.
```

---
## \#10 Posted by: ninTHIENdo Posted at: 2019-03-19T19:47:52.518Z Reads: 34

```
That range doesn’t seem too bad, you could always get 2 more and run 2 in parallel and then series those together. That should double your range.
```

---
## \#11 Posted by: xsynatic Posted at: 2019-03-19T19:53:36.189Z Reads: 32

```
i think for the money i've spent on those (or 4 like you said) i could've gotten something better.

I payed 110€ per battery plus 70€ for import dutys/tax
```

---
## \#12 Posted by: xsynatic Posted at: 2019-03-19T20:05:13.279Z Reads: 27

```
Edit : 20km is with 90mm urethane wheels. AT decreases that significantly.
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-03-19T22:01:21.885Z Reads: 27

```
@xsynatic  18650 cells are far more power dense - for the same physical size battery pack, you could have much more capacity. It's pretty easy to make compact top-mount 18650 packs, using [these holders.](https://www.banggood.com/4x5-18650-Battery-Spacer-Radiating-Shell-EV-Pack-Plastic-Holder-Bracket-p-1122766.html)

Regarding your series/parallel question, you're using  the wrong units: It's not voltage and range, it's voltage, current and capacity. Given two (idealized example for round numbers) 10v 10ah batteries that can supply 10 amps each, you will have a total energy of 100wh each. If you put them in series, you get 20v and 10A. If you put them in parallel, you get 10v and 20A. Either setup has the **same** energy, and thus the same range. The only difference is one provides more voltage, while the other provides more current. Same watts, same watt-hours, same range. 

Those "% - style" battery meters are making a guesstimate based on common values of voltage vs state-of-charge (which is non-linear) and assumptions of the exact battery chemistry (there are dozens and they all behave differently). It's a ballpark gauge at best. I always just used one that gave me actual voltage numbers so I could do my own guesstimates.
```

---
## \#14 Posted by: xsynatic Posted at: 2019-03-19T22:29:08.138Z Reads: 24

```
First of all thanks for the response.

If i were to build my own pack. Wouldn't i need a spotwelder? I think i rather let someone build it even if i have to pay a premium on top. I'm known to fuck up really easy things.

What do you think is a good cutoff voltage?
The VESC tool says 39.2v on a nominal voltage of 3.7 in a 12s configuration, which would translate to 3.26v per cell. If i'm not wrong. But 3.26 is a biiit to low, correct?

My battery in series has 50.4V
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-03-19T22:35:47.982Z Reads: 22

```
Yeah, having someone else build it might be a good idea. 

Cutoff voltage is all about trade-offs, and which type of cell chemistry you have. LiPo cells generally don't like going much below ~3.7ish, maybe 3.5 at a minimum, whereas 18650s are usually okay down close to 3.0v, and some are rated all the way down to 2.5 in their datasheets. The closer you go to these minimums though, the more wear and tear on the cells. If you want absolute maximum range, go lower. If you want to baby the pack and get more cycles out of it, go higher.

Read up on cycle life and battery wear, it's an interesting subject.
```

---
## \#16 Posted by: xsynatic Posted at: 2019-03-19T23:09:10.969Z Reads: 19

```
Do you happen to know any reputable builder (except LHB) ?
```

---
## \#17 Posted by: MysticalDork Posted at: 2019-03-19T23:39:29.365Z Reads: 18

```
Not off the top of my head, unfortunately. Where are you located?
```

---
## \#18 Posted by: xsynatic Posted at: 2019-03-19T23:53:36.357Z Reads: 15

```
Germany

10char
```

---

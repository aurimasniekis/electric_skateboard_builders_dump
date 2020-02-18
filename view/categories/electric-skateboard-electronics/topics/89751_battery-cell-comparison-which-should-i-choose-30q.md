# Battery cell comparison. Which should I choose? 30Q?

### Replies: 21 Views: 904

## \#1 Posted by: turbolovah Posted at: 2019-04-07T23:18:50.012Z Reads: 168

```
Hey guys, I'm a little confused
I am in the process of choosing what cells to use to make my 12s4p battery pack in my first diy skateboard

I am going to run 2 200kv 6374 motors through either the new flipsky dual 4.2 vesc with fixed resistors or a flipsky dual 6.6 vesc

I currently have 20 Samsung 20R, batteries right now that I could use that have a 22A maximum discharge current, but they only have 2000mAh capacity

I see that people like to use Samsung 30q batteries that have a nice 3000mAh capacity, but only produce a 15A maximum discharge current

I have a limitless supply of LG M26 cells that I could use as well and make as big of a pack as I want without spending anything, maybe even a 14s4p pack. LG M26 cells have a 2600mAh capacity but a measly 10A maximum continuous discharge current. Would this fair better in my setup at 14S?

I assume that the 20R will experience a worse voltage sag because of the smaller capacity, but I wonder why people use Samsung 30q batteries in high powered setups as they have a smaller discharge current.

What is my best option to power these motors, what are the pros and cons in your opinion of these 3 choices. I am leaning towards the Samsung 30q cells because of popularity, but I would like a better understanding of why they are the go to batteries in the eskate community. 

If I made the LG pack, (which is free to me) what issues would I run into?
```

---
## \#2 Posted by: AlanZhou Posted at: 2019-04-07T23:29:35.888Z Reads: 159

```
https://www.electric-skateboard.builders/search
```

---
## \#3 Posted by: Esk8enginneer Posted at: 2019-04-08T03:12:32.524Z Reads: 148

```
Hahahaha burn.
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-04-08T03:30:24.168Z Reads: 142

```
there are a ton of posts on this forum on what to choose. 30q's are widely accepted as a 20a battery and not 15a. the best alternative are sony vtc5 or vtc5a, lg hg2, or samsung 25r. if you are running dual 6374 i strongly recommend 12+ ah pack at 10 or 12s. a vesc 4.xx doesn't usually do well over 10s. and yo answer your question, a 14s4p pack would be crap with that discharge rating. your voltage sag would be awful and you wont have any hill climbing or acceleration abilities. when my parts arrive, i will be making a few 10s4p packs. i could make you a 10s8p if you want. (made from vtc5 cells 2600mah 25a)
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-08T03:36:07.303Z Reads: 134

```
[quote="Dirt_Bag, post:4, topic:89751"]
vesc 4.xx doesn’t usually do well over 10s
[/quote]

Trust me 12s is usually no problem on 4.12, ollins vesc is 4.12, focbox is 4.12 and both are some of the most reliable vesc
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-04-08T03:38:22.225Z Reads: 126

```
ollin's is still not as stable at 12s and a focbox is hit or miss. ive cooked 2 focboxes on 12s before. (small motors, not overcurrent) the vesc 6 has overspeced parts that handle voltage better. 4.xx hardware really should be used at 10s unless you need a 40+ mph board for some reason
```

---
## \#7 Posted by: Dirt_Bag Posted at: 2019-04-08T03:40:31.552Z Reads: 121

```
i should say one thing. the ollin vesc and focbox are generally more reliable than regular vescs. they still dont handle the voltage as well as i hoped when buying them. a 6.xx is the best investment i ever made for my mtb
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-08T03:42:21.408Z Reads: 115

```
You know that both vesc 4xx and 6xx are rated for 63v right?
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-04-08T03:42:53.714Z Reads: 111

```
I'm gonna be running 13s on my focboxes and mabye I'll try a unity
```

---
## \#10 Posted by: Dirt_Bag Posted at: 2019-04-08T03:56:12.151Z Reads: 110

```
the 4.xx may be rated for it, but i have never heard of a board running 12s+ that lasts.
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-08T03:56:40.898Z Reads: 111

```
... trust me it will last

There are lots of people running 12s on 4.12 that lasts
```

---
## \#12 Posted by: Dirt_Bag Posted at: 2019-04-08T03:56:51.248Z Reads: 108

```
be careful, i cooked mine on 12 after 2 months. i was using dual 6374 on a streetboard
```

---
## \#13 Posted by: AlanZhou Posted at: 2019-04-08T03:59:09.934Z Reads: 107

```
That’s your personal experience doesn’t mean everyone’s results is gonna be like that

I’m gonna see how my fox box holds up on 13s10p :rofl:
```

---
## \#14 Posted by: Dirt_Bag Posted at: 2019-04-08T04:00:31.065Z Reads: 106

```
ik ofc. but i never hear of a 4.xx frying with 10s unless over current. but i have heard of them frying left and right at 12s. if you use 12s foc, its pretty much guaranteed to cook a 4.xx thats not a focbox at some point
```

---
## \#15 Posted by: Dirt_Bag Posted at: 2019-04-08T04:01:17.767Z Reads: 104

```
best of luck though! it will be interesting to see how they handle it. what motors are you using?
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-04-08T04:01:58.403Z Reads: 103

```
Hummie hubs as of now and tb dd when they come you can check out my thread


Many people have used focbox on 13s but they didn’t post updates
```

---
## \#17 Posted by: Dirt_Bag Posted at: 2019-04-08T04:02:34.390Z Reads: 103

```
i will do that for sure!
```

---
## \#18 Posted by: deucesdown Posted at: 2019-04-08T04:29:43.688Z Reads: 101

```
Back on topic, 30q are popular because they balance capacity, discharge amps, and price.

Dual 6374 you're looking at about 40a per vesc, 80a total. 30q have been tested by many to handle 20a continuous. They have low IR, so voltage sag is under control.

your 20R sound like good cells, but 20 cells is about half what you need.

The M26 will likely sag a LOT unless you get like 8p or 10p. 10s10p is a lot to put on a skateboard.

There are other good/great cells, but they usually cost significantly more than 30q. VTC5a is currently very cheap at ru.nkon.nl though, cheaper than 30q. The tradeoff is, at 25a discharge, this cell is better for power but slightly (maybe) worse for capacity.
```

---
## \#19 Posted by: Dirt_Bag Posted at: 2019-04-08T06:09:06.774Z Reads: 93

```
Everything he said is spot on. In testing though the capacity of a vtc5a is lower than a vtc5 cell when pulling 5a or more from it. Strangely enough the vtc5 and vtc5a can handle the same current but the 5a lacks its rated capacity. If you want torque, go with the vtc5 or vtc5a. If you want a little extra range at the cost of torque, then the 30q or lg hg2 is the best option
```

---
## \#20 Posted by: turbolovah Posted at: 2019-04-08T16:46:26.044Z Reads: 71

```
@Dirt_Bag the 4.2 from flipsky is supposedly reliable at 12s now after a recent hardware update where they replaced some resistors. Schtekarsten & Gamer43 found the original fault and have tested the new resistor setup apparently pretty rigorously? The original thread is here https://www.electric-skateboard.builders/t/flipsky-4-20-a-explanation-to-the-mystery-and-how-to-stop-the-cutouts-entirely/87824
```

---
## \#21 Posted by: Dirt_Bag Posted at: 2019-04-08T17:02:09.921Z Reads: 65

```
i have seen that topic. I actually plan on testing a 2 flipsky 4.xx's soon. but my statement stands, compared to the 6.xx hardware, a vesc 4 is not nearly as reliable on 12s. ofc its not always going to ruin your vesc, but it certainly is a risk
```

---

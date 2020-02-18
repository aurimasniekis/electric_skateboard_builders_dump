# Trying to bleed out my battery pack&hellip;is it safe? help!

### Replies: 14 Views: 379

## \#1 Posted by: theviith Posted at: 2018-06-06T06:50:04.590Z Reads: 162

```
Hi guys, so one of my battery pack is severely unbalanced. It's a 10s5p LG HG2 pack with cell groups 8 and 9 severely unbalanced. I don't have a direct power source to individually charge the cells so I thought to manually bleed out groups 1-7 instead. The voltages of groups 8 and 9 is around 3.6, while all the other groups are at 4.1ish. I am thinking about bleeding out groups 1-7 to 3.6V by connecting FIVE 6V rated light bulbs in series. Since the voltage up to cell group 7 is about 29.2V, theoretically the 5x light bulbs in series should work..but would it be safe? Given that it is essentially a 7s5p with 15A of current output to the light bulbs, would the wires/bulbs burn out due to the massive current?

As for group 10, I can bleed it out with a single bulb since its low enough voltage.

Thanks in advance
```

---
## \#2 Posted by: Hummie Posted at: 2018-06-06T07:16:07.867Z Reads: 151

```
i think if you were able to find the resistance of the 5 bulbs using a multimeter or some other method then it would just be the voltage you connected to that and work out the current that will happen using ohm's law and see if would equal what the bulbs could handle.  in the wattage calculation on the bulbs i think they use the rms voltage of the 120ac since its ac but not sure.  maybe add more bulbs than you think.  why do you think it would be 15amps output? the current would be based on the bulbs' resistance no?
```

---
## \#3 Posted by: Martinsp Posted at: 2018-06-06T07:23:55.023Z Reads: 142

```
It would definitely work, not sure if using the 6V bulb is the best idea even though it would work. I was using high beam car 50W  bulbs. They are rated for 12V. I was using one on each 3S part of my battery. You could even connect one bulb to each parallel group so 1S. I am not sure about the current you are mentioning and where it came from since you did not mention any wattage. You could also use power resistors to do the job, but bulbs are easier to get of course.
```

---
## \#4 Posted by: theviith Posted at: 2018-06-06T08:28:51.177Z Reads: 122

```
@Hummie thanks for the info. I said 15A because LG HG2 cells are 3000mah each and I have them wired in 5p so that would be 5x3000mah so about 15000mah = 15A. Please correct me if I'm wrong though haha.

@Martinsp I'm not sure what watts the bulbs are but based on the size, I'd say about 1.5W-ish? This is what they look like![20180606_011607|690x335](upload://4nPjrJIG9MtBtQ9159FZIrbogLR.jpg)
```

---
## \#5 Posted by: Martinsp Posted at: 2018-06-06T08:32:47.764Z Reads: 104

```
Yeah that sound about right, that would take super long to discharge 15Ah pack... you would be better off taking one car bulb and sticking it across 2 or 3 cells at a time
```

---
## \#6 Posted by: Hummie Posted at: 2018-06-06T15:09:25.008Z Reads: 75

```
[quote="theviith, post:4, topic:57975"]
I said 15A because LG HG2 cells are 3000mah each and I have them wired in 5p so that would be 5x3000mah so about 15000mah = 15A. Please correct me if I’m wrong though haha.
[/quote]

that would be math for maybe a charge or discharge rate at 1c.    those cells can do 20 each I think and then you have 5p so they could do 100 amps continuously COMFORTABLLY, but to figure the amount of current that will actually come out of the battery when connected in circuit with the bulbs, and make sure it isn't so much that the bulb goes pop, and make sure the current coming out of the cells is within that 20a each, you could use Ohm's law and you will need to figure the resistance of the bulb and using that and the voltage the formula will give the current that will occur.  those bulbs look pretty dinky and I think they will pop like poprocks in your mouth.   do you have a multimeter?  otherwise I think you might be able to make an assumption based on the bulbs wattage but I don't know but if you looked on endless-sphere I'm sure you could get an answer.
or forget the math and hook up a car bulb and see what happens.  if it looks too bright and blows up then you know its too much voltage.
```

---
## \#7 Posted by: deucesdown Posted at: 2018-06-07T00:01:09.397Z Reads: 54

```
Can you get your hands on halogen tracklight bulbs? Like MR16? Usually 12v or 24v DC and 20-50w?

Like

https://www.amazon.com/dp/B010CMS44Y

12v 50w 3 pack x 2. Put them in parallel?
```

---
## \#8 Posted by: Hummie Posted at: 2018-06-07T03:16:33.828Z Reads: 43

```
tell me if I'm wrong but with resistors (or bulbs) in parallel wouldn't it be less resistance and therefore more current vs doing the bulbs in series?
```

---
## \#9 Posted by: deucesdown Posted at: 2018-06-07T04:37:09.137Z Reads: 38

```
Yeah sorry brain's cooked, can't remember how it works. I was thinking to lower the voltage seen by each bulb. Decent chance I got it totally wrong.:)

Gonna refrain from typing more nonsense until I've slept.

EDIT sorry for posting with dead brain and without checking facts. Series connections, to lower the voltage seen by each bulb. Resistance increases but I don't think that's the interesting part.
```

---
## \#10 Posted by: Eboosted Posted at: 2018-06-07T05:01:15.332Z Reads: 32

```
If some packs are unbalanced there is usually a problem you need to fix first.

May I ask you:

how do you connect the packs? 
What bms are you running? 
How old is the battery? 
How much charges when the charger turns off?
```

---
## \#11 Posted by: theviith Posted at: 2018-06-07T05:26:03.459Z Reads: 27

```
first off, thanks everyone for the input. I think I'm gonna do a bit more searching around the house to see if I can find a larger voltage bulb or something equivalent before deciding on anything.

@Eboosted 
1. I connected them as 10s5p with nickle strip spot welded together. I've checked all the connections and there doesn't seem to be any break across the pack.
2. I was using a Supower BMS.
3. It's over a year old.
4. I'm not sure on this since I didn't really check after the charger stops charging at around 92%.
```

---
## \#12 Posted by: Eboosted Posted at: 2018-06-07T05:31:08.202Z Reads: 28

```
I had a lot of drifting after only a few charges when connecting individual packs with nickel strips.

Since I started connecting the packs with 12awg wire I haven't experienced drifting, use a second nickel strips to connect your packs or even a third or solder a 12awg wire between packs
```

---
## \#13 Posted by: E1Allen Posted at: 2018-06-07T06:53:31.236Z Reads: 27

```
This is why having a hobby charger works great.  So long as you can get to wires where you need to you can charge or discharge to whatever voltage you want.

Your two P groups are probably toast.  If they only charge to 3.6v and then you go ride, you can expect them to drop well below safe cutoff while the other batteries are above it still.  

So why do you want to lower the voltage of the other P groups?  There's a really good chance 3.6v is all those batteries will charge to. But hopefully not.
```

---
## \#14 Posted by: theviith Posted at: 2018-06-08T05:41:35.260Z Reads: 25

```
@Eboosted so the reason why there's drifting with nickel strips is because there's too much resistance?

@E1Allen Reason I wanted to lower the voltage of all the other cell groups is so that the BMS would be able to balance charge all groups. Thinking about it, I think what might have happened was that groups 8 and 9 got drifted and the difference becomes too great for the bms to effectively balance charge all the groups, so it bypasses groups 8 and 9 and they ended up drifting further and further apart. 


Good news everyone! I managed to dig out an old lipo charger from storage and charged up the drifted groups. Now I just need to test ride it and see if the pack stays balanced with the new BMS (Bestech). Will report back here once I have some data
```

---

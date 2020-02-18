# Battery Pack help needed! Aka: I messed up! Tell me how much!

### Replies: 14 Views: 1314

## \#1 Posted by: Papperlapp Posted at: 2017-04-28T12:08:07.904Z Reads: 199

```
I got my battery pack from this group buy: [https://www.electric-skateboard.builders/t/also-usa-10s4p-samsung-25r-190/12458/146](https://www.electric-skateboard.builders/t/also-usa-10s4p-samsung-25r-190/12458/146)

So, I had my battery pack for a while now. Since I am still waiting for my VESC to arrive, I thought I would shrink wrap the pack since I was not 100% happy with the fake carbon tape solution. Technically everything works fine with this pack. I just wanted to stress that here. Just the wrapping I wasn't to fond of.

So I removed the tape:

<img src="/uploads/db1493/original/3X/5/2/52b12abd233e70e41a97381d1608d1a809ef4358.JPG" width="666" height="500">

On the other side is layer of plastic sheet to stabailze the BMS, switch, etc.
I wanted to get rid of that in the process, to save some height to better fit my enclosure.
<img src="/uploads/db1493/original/3X/f/0/f0a1f3230f78857c919bc04a668fec8ea2f5eec2.JPG" width="666" height="500">

Without the plastic sheet:
<img src="/uploads/db1493/original/3X/3/7/37b291f83f5cce20fa419e4ecdd421a141ff8e25.JPG" width="375" height="500">

Bare pack:
<img src="/uploads/db1493/original/3X/0/e/0e726611bbb8407bf483a4ef3a48d6028806c981.JPG" width="666" height="500">

I got my shrink wrap today and I wanted to see if it fits. And here is where I messed up:
<img src="/uploads/db1493/original/3X/7/3/73cc246a262eeb8198eaef4c442d7fad69f073ad.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/1/c/1c909e6727aec38814af3b841c356bd1838416a9.JPG" width="666" height="500">

I put stripes of aluminium on either side within the shrink wrap testing to further stabilize the pack horizontally. When I moved the pack it shorted and burned a whole through the aluminium. I am glad that nobody got hurt.
<img src="/uploads/db1493/original/3X/0/f/0ffb149497fd740c23de362c39b43983f0bc19bc.JPG" width="375" height="500"> 

My stupidity is not in question here. I know I messed up.
I was wondering **first**, what went wrong, since I always thought that aluminium does not carry electricity?
And **second**, where do I go from here? The pack still turns on. 

I obviously have to solder the cable back on.
But, is it save to still use it like that or do I have to fix something? And if so, what and how?
```

---
## \#2 Posted by: fedestanco Posted at: 2017-04-28T12:24:09.210Z Reads: 183

```
Aluminum does carry electricity. But don't panic: there is a good chance your cells are still fine. First step is check the voltage of every sincle series.
I can offer you a free repair if the pack is still repairable.
```

---
## \#3 Posted by: KTMinni Posted at: 2017-04-28T13:48:42.665Z Reads: 174

```
I agree with the above comment.  I have sparked my batteries a ton of times(not that I recommend it or anything) and all of the cells are still fine(somehow the pack gained 0.1V in the process, but I double checked it was fine). Just keep in mind, one of the properties of metallic anything on the periodic table is being a good conductor of energy, whether it's heat or electricity.
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-04-28T13:58:38.356Z Reads: 167

```
This happens to me on occasion. Usually i clean up the site with a dremel sanding drum and add another layer of nickel over the wound. 

You can probably just run it as is though. I have much worse packs than this doing things around the shop.
```

---
## \#5 Posted by: willpark16 Posted at: 2017-04-28T14:20:00.543Z Reads: 162

```
They are samsung and have some really good protection I shorted mine on the can and it still ran fine just watch it for a few says
```

---
## \#6 Posted by: Papperlapp Posted at: 2017-04-29T13:15:08.554Z Reads: 131

```
Thanks for your help.

@fedestanco: I'd like to take you up on your offer. What do you need? Should I measure something? Although chances are, that I break it even more in the process.
```

---
## \#7 Posted by: fedestanco Posted at: 2017-04-29T14:17:01.517Z Reads: 122

```
You will need a multimeter (google it if you dont know it) used to measure voltage. 
If you look closer, the battery is divided in smaller groups of 4 cells each (these groups are called series). Using the multimeter you should measure each group's voltage and tell me the values you find. 
A second inspection you should make is the "spot welds inspection"; this is to check if you broke some spot weldings while shorting the battery.
Using some thin tool (like a small screwdriver) apply a VERY VERY WEAK amount of leverage under the burned nickel strip. If the welding held up, your leverage action should be very limited, and the nickel strip should seem to be "glued" to the battery.
```

---
## \#8 Posted by: Papperlapp Posted at: 2017-04-30T13:22:58.167Z Reads: 109

```
I had a multimeter already.

I get 3,9 Volts from all 10 series.
When I measure the whole pack I get 40 Volts.

The strip seems still solidly stuck to the batteries where the short was. Although there seems to be a part missing. You can see that in the pictures.

What's next? Do I have to fix something? Do I have to send it back to you?

Btw: Thank you all so much for your help!! I would be stuck without you.
```

---
## \#9 Posted by: fedestanco Posted at: 2017-05-01T14:11:22.237Z Reads: 90

```
The voltage of shorted series isnt different from the other series, which is good. I suggest you one last test: internal resistance (Ω on your multimeter) of the cells with burning marks. Compare it with the internal resistance of other good cells.
You will also have to solder back the balance wire (the red one). Aluminum enclosure is fine as long as you properly insulate the battery. I suggest you to tape any metallic part of the battery with kapton tape or normal insulation tape; the more layers, the less change of shorting.
```

---
## \#10 Posted by: Papperlapp Posted at: 2017-05-03T08:14:38.000Z Reads: 76

```
Internal resistance of all cells are almost equal.
I soldered the balance wire back on.

Now all that is left is putting it all in shrink wrap. I will post pictures when I actually get to do the shrink wrapping. Life is a bit busy right now...

Again, thank you for your help!
```

---
## \#11 Posted by: Papperlapp Posted at: 2017-05-11T17:39:40.610Z Reads: 65

```
So, I finally got around to getting closer to finishing the battery pack.

1. I put plastic stripes on the outsides of the pack and one stripe across at the end (with hot glue)
2. I put shrink wrap around
3. (still needs to be done) cut holes for the power switch etc.

It is much more sturdy and even a bit slimmer towards the electronic parts now. Both were very important to me!

Maybe you want to use some of what I did for your next batch @fedestanco. Or you can tell me if I overdid it :yum:

The pack works great so far. Although it might be a few days/weeks till it actually gets used in eanest. 

<img src="/uploads/db1493/original/3X/e/d/edb8b13a3426d9d86c3b31ae29cf5e85fcfe0537.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/b/bbf4cf0075e9b3bcfe83a69daa797771a05415fa.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/3/d3b76dd6b57bc1e84d69866aee0cc4a235d81e61.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/4/e45792521feafb48d19752ecb1599d46d25c0458.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/2/6/26a763a8a24889d4701b9ae8847f77d1f62ea96e.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/0/9063078c0754f6d195a92dae6214b626b4f394bd.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/4/1/4140130b32034648fd3c20386c0389789eafbe5c.JPG" width="666" height="500">
```

---
## \#12 Posted by: zk8_builder Posted at: 2017-05-12T07:15:06.092Z Reads: 51

```
What size heatshrink is that??
```

---
## \#13 Posted by: Papperlapp Posted at: 2017-05-12T10:59:03.967Z Reads: 44

```
165mm accross flat dimension.

I got mine here: http://www.akkushop.de/de/accucell-schrumpfschlauch-165mm-21-pvc-1-meter/
Took me quite a while to find it.
```

---
## \#14 Posted by: zk8_builder Posted at: 2017-05-12T11:09:55.028Z Reads: 45

```
Ok thanks.......
```

---

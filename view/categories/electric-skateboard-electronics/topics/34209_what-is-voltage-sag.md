# What is voltage sag

### Replies: 25 Views: 3810

## \#1 Posted by: Brycehoosiers Posted at: 2017-09-28T21:16:29.345Z Reads: 314

```
What is exactly is voltage sag on electric skateboards,I kind of understand it ,but I just want to make sure I fully understand it.
```

---
## \#2 Posted by: Stevemk14ebr Posted at: 2017-09-28T21:32:43.539Z Reads: 313

```
Power = Current * Voltage

To draw more power you need either more current or more voltage. An ideal battery would have a fixed voltage that never changes, if you need more power you get more current from the battery. In reality the voltage drop a battery can provide varies depending on how much current you need. So if you go up a big hill your voltage will appear to sag since you are drawing more amps and our non-deal battery drops its voltage a tad when under high load.
```

---
## \#3 Posted by: Aeroquiv Posted at: 2017-09-28T21:34:14.552Z Reads: 310

```
Voltage sag is the total input impedance of the system with respect of the current flowing through the load. For instance, let's say your VESC is pulling 10 amps from the battery. The internal resistance of the battery, which is usually around 50-100 mOhms will drop the voltage through the battery by Ohm's Law, V=IR. So a fresh 4.2V battery with 50 mOhm impedance drops to 3.7V, but there is also impedance through the BMS, anti-spark switch, the VESC and even the wires themselves. So while they're insignificant by themselves, the total system impedance add up with battery internal resistance usually being an order of magnitude larger. Thus, voltage sag.
```

---
## \#4 Posted by: GrecoMan Posted at: 2017-09-28T21:38:58.330Z Reads: 295

```
@Clonkex @scepterr @wafflejock...
here we go again
```

---
## \#5 Posted by: scepterr Posted at: 2017-09-28T21:40:09.765Z Reads: 286

```
The wonders of search...
https://www.electric-skateboard.builders/search?context=topic&context_id=34209&q=Voltage%20sag&skip_context=true
```

---
## \#6 Posted by: darkkevind Posted at: 2017-09-28T21:42:21.755Z Reads: 280

```
Further to the explanations above, if you had a battery that could provide 200A of current, and you used it for eSk8, you would see virtually no voltage sag at all because drawing say 50-60A for a single motor would be well within the battery's capacity, it would only draw a relatively small amount of current from each cell and therefore be able to keep it's voltage relatively contant.

On the flip side, if you regularly draw 50-60A and your battery can only provide a maximum of 60A, you would see a quite considerable voltage sag where the cells are - in laymen terms, dealing with trying to supply the current over worrying about keeping their voltage constant because each cell can only provide a nominal amount of current.

Not sure if that explains it very well but what the hey...
```

---
## \#7 Posted by: thisguyhere Posted at: 2017-09-28T21:42:34.917Z Reads: 257

```
both excellent explanations but...first of all you're throwing too many big words at me. okay now, because I don't understand them I'm gonna take 'em as disrespect.

visually speaking, take a look at the first two images in this post.

you'll see 6v sag when there's 75amp draw on the battery:

https://www.electric-skateboard.builders/t/6v-sag-too-much/32002

sag could cause problems:

https://www.electric-skateboard.builders/t/ate-shit-today-and-loop-keys/33613/30
```

---
## \#8 Posted by: TheRedPanda Posted at: 2017-09-28T21:43:05.390Z Reads: 223

```
Beat me to it @Aeroquiv  ^

To add to this solid explanation voltage sag affects your eSK8 in a couple ways.

1. If your battery is not fully charged voltage sag may drop the voltage in the pack below what the BMS will allow the pack to function at(cutoff voltage), and will not let your battery run until the voltage is back up again, usually this happens quickly but can be quite disruptive if you're accelerating hard and your power cuts out.

2. Depending on the particular cells you are using you may find reduced performance from voltage sag where others aren't really affected. For example LFP Cells(see A123 26650) are excellent at maintaining their rated current through it's SOC(State of Charge), it also doesn't hurt that the rated current is extremely high in this chemistry. But in a low end standard 18650 if your cell is not fully charged you may be unable to access the advertised current draw due to the voltage sag. (Check out Voltage/Current charts for the cells you plan to use and make sure the required current for your application can be met with your pack design from fully charged to "empty")
```

---
## \#9 Posted by: scepterr Posted at: 2017-09-28T21:46:58.843Z Reads: 200

```
We don't need 162535263 topics explaining the same thing, this is getting silly
```

---
## \#10 Posted by: Brycehoosiers Posted at: 2017-09-28T22:13:38.911Z Reads: 191

```
Thanks for the replies
```

---
## \#11 Posted by: wafflejock Posted at: 2017-09-28T22:22:46.577Z Reads: 187

```
Lots of good responses just also wanted to add some real world data here from the metr bluetooth module hooked up to the VESC and transmitting data to be logged on my phone:

https://metr.at/r/rKZvg

Can see as you go from left to right you're going over time and as the throttle is pulled (current goes higher) the voltage goes lower.  For reference I'm using a 149kv motor 10S 5Ah (185Wh) with 2 5S 5Ah 20C lipo packs.

Another one from my history:

https://metr.at/r/ZLeqH

---

Also to clarify the bluetooth module is a regular one but one is sold to go with the app with a cable for easy connecting and to support the dev a bit (I think).
```

---
## \#12 Posted by: Brycehoosiers Posted at: 2017-09-28T22:25:42.849Z Reads: 175

```
does your vesc or bms ever shut off because of your sag?
```

---
## \#13 Posted by: wafflejock Posted at: 2017-09-28T22:26:57.537Z Reads: 172

```
I don't use a BMS so can't speak to those but from other threads looks like that can happen, for the VESC I have a wide range for limiting power so it starts to dip the power usage itself at a pretty safe point and I stop maxing the throttle since I'm usually trying to get home if that's the situation.

I have a 2V range between the soft cut off (limits power) to hard cut off, I start cut off at 37V and turn off completely at 35V I was using 38 and 36V which is more conservative but now just try to not drain it by paying attention and recharging when needed, which is regularly.

---

When the vesc itself cuts off the power you just can't accelerate anymore you're left to kicking or dragging your board but nothing bad happens aside from that.
```

---
## \#14 Posted by: thisguyhere Posted at: 2017-09-28T22:28:14.148Z Reads: 164

```
yes, sag went below lower voltage cutoff, bms reset during hard acceleration.  got thrown off, been nursing wounds for a week now.
```

---
## \#15 Posted by: SORRENTINO Posted at: 2017-09-28T23:04:12.781Z Reads: 161

```
<img src="/uploads/db1493/original/3X/0/e/0e995a21025533eeb018ce008fce2ce453797047.gif" width="495" height="497">
```

---
## \#16 Posted by: Mikenopolis Posted at: 2017-09-28T23:08:38.433Z Reads: 151

```
[quote="scepterr, post:9, topic:34209"]
We don't need 162535263 topics explaining the same thing
[/quote]

I understand your RTFM comment and made me wonder why schools exist now that the answers are basically at our fingertips...We often ask/scold people to use the search feature...I think instant gratification is something we all enjoy, reading and scrolling old threads vs. getting someone to answer from a fresh thread is not a hard decision.
```

---
## \#17 Posted by: Deckoz Posted at: 2017-09-28T23:34:04.069Z Reads: 146

```
<img src="/uploads/db1493/original/3X/2/0/205b96630ab3b8786b2599620cc67d77d079e5ff.gif" width="275" height="252">
```

---
## \#18 Posted by: Clonkex Posted at: 2017-09-28T23:35:17.314Z Reads: 148

```
Ultra simple answer:

If you accelerate hard, your battery will have a heavy load on it and the voltage will go down a bit. When you let up on the throttle the voltage will come back up again.

More stuff:

- Lipos experience less voltage drop than li-ions. I don't know the exact values.
- Obviously the voltage will be going down overall as well because you're using the battery, so it might not come back up to the same voltage it started at.
```

---
## \#19 Posted by: GrecoMan Posted at: 2017-09-28T23:39:37.324Z Reads: 148

```
It’s just a common curtesy thing, you inconvenience other people just so you can be lazy and not type your 20 characters into the search bar, honestly I’m kind of sick of hearing, “we all have to start somewhere”.   I agree with that statement but it is just how different people deal with not knowing things.  For example, a user with 30 days visited, 20 hours read and 5-6 topics created is in my eyes, much more curtious than someone who has 50 days visited, 3 hours read and 40 topics created.

My 2 cents
```

---
## \#20 Posted by: Deckoz Posted at: 2017-09-28T23:42:27.508Z Reads: 148

```
Ah this is because this simple thing right here.

18650 are a specific size, you can only jam so much inside the cell

Lipo and lion are the same chemistry. And they share the same attributes.

The bigger the surface area of the anode and cathode the more mAH you gain. The more sheets of A/C layers, the more ampacity you gain. Granted you gain both going both ways but one plays more of a part on their respective behalves.

So a lipo can be, well any size.

A li-ion has to be engineered by how long the sheets are (mAh), vs how many sheets(Ampacity) together are able to be rolled up and be stuffed inside a standard size casing.  And with this we have ..nothing more important then before I typed it..lol
```

---
## \#21 Posted by: Clonkex Posted at: 2017-09-29T00:02:19.845Z Reads: 134

```
Lipo and li-ion are not exactly the same.Li-ions typically have lower discharge rates, for instance. I'm not 100% sure what you're saying.
```

---
## \#22 Posted by: Deckoz Posted at: 2017-09-29T00:12:48.892Z Reads: 136

```
...that's due to how many anode and cathode sheets are inside that make up the battery as well as the length of the sheets. 

If you have a single anode and cathode sheet that's say 48 inches long rolled up, you'll have a bigger battery(mAh) with very bad amp output. But if you have 4 anode/cathode sheet combos that were 12 inches long and layered together. You'd have less mAh but more ampacity on the cell.  These are analogy numbers(fake)

But the point is you can only have so Many anode&cathode sheet combos * x size(ie surface area per sheet) stuffed into an 18650...  

Lipos have no standard size restrictions. So you can make a high quality battery with many anode and cathode combos making the ampacity of the cells high(increasing C), or you can make the same size mAh sheets but fewer and still have x size battery with a lower C
```

---
## \#23 Posted by: Okami Posted at: 2017-09-29T06:42:07.129Z Reads: 118

```
Good info, in sort of glad someone opened thid topic and brought these different explanations to the table.. im sure it might have taken a lot of scrolling in some other threads but here it somehow got pretty condensed :)
```

---
## \#24 Posted by: scepterr Posted at: 2017-09-29T06:46:25.797Z Reads: 117

```
Too bad there's gonna be another thread asking the same thing tomorrow...🤣🤣🤣🤣🤣
```

---
## \#25 Posted by: GrecoMan Posted at: 2017-09-29T11:34:19.543Z Reads: 111

```
Now we can direct them here 😉
```

---

# \[How To\] Fix Anti-Spark Softswitch

### Replies: 27 Views: 3793

## \#1 Posted by: Stevemk14ebr Posted at: 2016-07-23T16:07:01.882Z Reads: 383

```
I see alot of people here use the anti-spark softwitch for their boards. I've also seen alot of people posting that they blow the mosfets on them and the switches get stuck permanently on. The fix is super easy and more people need to know about it.

Recently the switch i was using blew two of the three mosfets onboard. The mosfets are wired in parrallel and are surface mounts. An acceptable replacement for the built in mosfets are these: https://www.digikey.com/product-detail/en/nxp-semiconductors/PSMN030-150B,118/568-5950-1-ND/2531237 (150v, 55.5A, $1.80 each). When wired in parrallel these give a total switch spec of 150v, 166A. Simply solder these in place of the blown ones and you fixed your $50 switch for $5.

I have ordered the mosfets myself and they are shipping, i will update this thread when i receive them and see how they work. 

I theorize that the mosfets blow due to the lack of a capacitor or resistor in the circuit on the input line and the mosfets suddenly being saturated with voltage when a battery is plugged in (notice there isn't an actual anti-spark circuitry inside, the mosfets are expected to handle it all on plugin). I will personally be wiring an anti-spark xt-90 before my softswitch so that the resistor can suppress the spark. A large capacitor or two on the input line would also work. I would also use a better sealant, on the switch i have it was gunked with some sort of calk that didn't seem to transfer heat too well, you may want to consider using something similar to CPU heat paste for a better heat transfer.

Old mosfets:
http://i.imgur.com/zmx1Mof.jpg
http://i.imgur.com/uGZY7Uo.jpg
```

---
## \#2 Posted by: Menwaylo Posted at: 2016-07-23T16:12:30.967Z Reads: 349

```
This is good to know if it works, I have had 2 break immediately after using them for the first time.
```

---
## \#3 Posted by: Stevemk14ebr Posted at: 2016-07-23T16:14:25.902Z Reads: 345

```
I see no reason why it wouldn't work, but i'll know within a week and update everyone. I also chose mosfets that are WAY higher voltage than we need on eboards (150v) so i think this should be a solid choice.
```

---
## \#4 Posted by: ikjahaa Posted at: 2016-07-23T18:35:06.216Z Reads: 331

```
Be sure to order DC rated ones.
Why don't you just use a switch with the right rates ?

I use :
http://www.digikey.com/product-detail/en/nkk-switches/S7AW/360-1931-ND/1007009

Do not that this is a DPDT switch of 20Amps on each pole, so 40Amps if you combine them.
Also up to 30V since i'm just running 6S.

I use this switch turn my board on, completely off and into charging mode (closed connection to the esc).
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-07-23T22:09:24.860Z Reads: 309

```
I had bought the switch originally since i saw alot of others used it and figured it would be reliable, go figures ahah. Now that its blown i decided to not waste $50 and figure out how to redesign it to be better. That switch you got still has a pretty low amp rating, especially for 6s, on 12s id be more comfortable with that.
```

---
## \#6 Posted by: ikjahaa Posted at: 2016-07-24T19:48:26.366Z Reads: 275

```
20amp on each pole, 40 amps if you connect them and use them as one...
Seems enough for 6s, not?

Correct me if I'm wrong though.
```

---
## \#7 Posted by: barajabali Posted at: 2016-08-02T18:10:32.449Z Reads: 259

```
I have a blown soft switch damn thing won't turn off so I just cut it for now. 

Where is your update sir? @Stevemk14ebr
```

---
## \#8 Posted by: longhairedboy Posted at: 2016-08-02T18:46:35.669Z Reads: 258

```
dammit! i'm seeing this too late. but now i know how to fix the two i have in boards should they fail.
```

---
## \#9 Posted by: barajabali Posted at: 2016-08-02T18:48:54.271Z Reads: 254

```
What voltage are you running in the two boards that these work for? I don't think they're good for anything over 9s
```

---
## \#10 Posted by: longhairedboy Posted at: 2016-08-02T18:54:58.583Z Reads: 254

```
DIYs were rated at 14S and failed me in the last batch, but i have one from well over a year ago that's still going strong at 12S. The ones i have in mine and two customer builds are from Miami Electric and they're flier clones exactly like DIYs. 

I'm using Ollin vedder switches moving forward but i have have torn around on these flier clone switches from multiple vendors without issue, so i think there was a bad batch of mosfets going around.
```

---
## \#11 Posted by: barajabali Posted at: 2016-08-02T18:57:25.098Z Reads: 241

```
Yea I just blew one with fully charged 12s pack.  Woulda been great if they worked..
```

---
## \#12 Posted by: Stevemk14ebr Posted at: 2016-08-02T19:36:49.490Z Reads: 240

```
The board was more messed up than i thought. Just replacing the mosfets didn't work, it seems to me like the small step down circuit in the board that powers the blue light in the switch is blown aswell. I can't really so anything else without a circuit diagram so i've resorted to building my own switch with the mosfets i've bought and salvaging the blue switch. Should cost ~$7. I had a tb switch aswell.

The switch seems needlessly complicated to me. They added alot of junk just to get an led in the switch, i wish they would revert back to vedders original diagram, its much simpler and appears more robust.
```

---
## \#13 Posted by: barajabali Posted at: 2016-08-02T19:38:48.198Z Reads: 225

```
So it's not salvageable ?
```

---
## \#14 Posted by: Stevemk14ebr Posted at: 2016-08-02T19:39:55.112Z Reads: 227

```
The switch that plugs in is. The actual board doesn't appear to be. If @torqueboards wants to send me the schematic i can investigate more but it's hard to tell what's going on with it without one.
```

---
## \#15 Posted by: barajabali Posted at: 2016-08-02T19:40:28.790Z Reads: 226

```
Oh okay this thread is potentially really good if this can be figured out :)
```

---
## \#16 Posted by: torqueboards Posted at: 2016-08-13T17:32:10.818Z Reads: 221

```
I've been using these on 12S for a long time now. They have been more than reliable. Occasionally, though you'll have one break.

@Stevemk14ebr - I don't have the schematic for this one.

I have a re-design for the Vedder Spark and was going to offer it but decided against it since I didn't really like the 40amp limit. I'll look into it again.
```

---
## \#17 Posted by: MicroRAsus Posted at: 2016-08-31T13:55:16.823Z Reads: 214

```
I just installed this $60 on and off switch and switched on and off couple times and now the switch no longer turn off and connector sparks! I use 12s battery by the way, it is within the range. Bad quality! Is it mosfet problem?
```

---
## \#18 Posted by: Stevemk14ebr Posted at: 2016-08-31T15:07:54.911Z Reads: 204

```
It is a Mosfet problem yes. To be specific when wiring mosfets in parallel there is a short amount of time where the first few receives the full load of the system. So the fets do not immediately balance the load between them. This can cause the fetch to blow out and cause a cascading failure. There rearly isn't a good solution to this, I just use an anti spark loop now.
```

---
## \#19 Posted by: MicroRAsus Posted at: 2016-08-31T22:17:35.397Z Reads: 195

```
I just brought 4 pairs of xt90s. really sad, $60 into toilet..
```

---
## \#20 Posted by: Mobutusan Posted at: 2016-09-18T17:43:30.999Z Reads: 181

```
So, just to be clear, if these soft switches lose the ability to turn off, then there is no fix for them? They are just blown?
```

---
## \#21 Posted by: Stevemk14ebr Posted at: 2016-09-18T20:03:21.020Z Reads: 166

```
Correct. They suck
```

---
## \#22 Posted by: Sourcecode Posted at: 2017-04-14T05:35:06.305Z Reads: 123

```
sorry to res this thread from the dead but i just had this happen to me got 2 new switches and both died after one use!

http://imgur.com/l4JfGGC
```

---
## \#23 Posted by: Jebe Posted at: 2017-05-19T21:44:11.359Z Reads: 103

```
there is bugger all load when first powering up, unless you are on your board with the throttle fully open.
```

---
## \#24 Posted by: ACIN Posted at: 2017-05-19T22:33:53.298Z Reads: 99

```
Happened to me too :frowning:
I am hoping to use the (still working) LED switch with an original Vedder AntiSparkBoard, using the 5V or 12V output of my SBEC to power the LED, that is the plan.

Does anyone know for that matter where you can buy the Vedder AntiSpark in Europe? Protoboards stock is emptier than my wallet after buying this piece of crap switch!
```

---
## \#25 Posted by: evoheyax Posted at: 2017-06-19T16:57:01.197Z Reads: 94

```
A lot of people have had issue with this switch, including me. I was hoping to fix it but I guess it's not that simple...
```

---
## \#26 Posted by: sl33py Posted at: 2017-06-19T17:40:40.125Z Reads: 91

```
For those who want to repair one of these - it likely needs new FETs.  You need to replace all on the PCB - i believe there are 3 total.  You should always replace all the FETs at the same time - not just the one which may have failed.  The others will fail shortly if you don't replace them anyway.

Since the FETs are the most expensive part - they are usually ~$4-8 ea.  So, if you have the skill to reflow SMD (hot air or skillet or reflow oven), and the time, it's likely a big portion of the total cost of the switch.  AND it might not be the true fix, if something else failed you wouldn't know until swapped...

I would suggest the Vedder AS switch as much more robust.  I think there is a market for a more durable AS similar or even over-built compared to Vedder/Fechter's.
```

---
## \#27 Posted by: Surfer Posted at: 2017-06-19T18:31:19.199Z Reads: 88

```
The ones from @goldenHusky are bomb proof, if it's not sufficient he is always backing the products with amazing warranty conditions. Cheers
```

---

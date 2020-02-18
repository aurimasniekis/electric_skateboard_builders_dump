# Two questions on BMS wiring

### Replies: 29 Views: 5114

## \#1 Posted by: jga Posted at: 2017-08-08T12:42:57.942Z Reads: 309

```
I have a BMS with no C-, so only B- and P-, which means I will have to solder both the charger - and ESC - on the P- of the BMS. Is the best solution to solder both cables to the BMS or to solder one and then have a sort of Y connection a couple of cm after (hope this is clear...)?

For the sensor wires, is there any specific order for the connection to the cells or is that just to be able to identify a defaulting one more easily?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-08-08T13:20:34.119Z Reads: 304

```
You can connect the negative charge cable either way. 
The balance wires must be connected in correct cell order. If you get it wrong you may permanently damage the bms
```

---
## \#3 Posted by: jga Posted at: 2017-08-08T13:36:34.477Z Reads: 291

```
Ok, noted.
There are no numbers on the wires coming from the BMS. So i just need to make sure the first one is connected to the cell that is the positive side of the battery, and then move along until I arrive at the cell with the main negative wire?
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-08-08T13:42:44.247Z Reads: 286

```
[quote="Namasaki, post:2, topic:30062"]
If you get it wrong you may permanently damage the bms
[/quote]

WILL permanenlty damage the BMS. You'll have all that wiring done, and you'll plug it up and see that nothing sparked and it will seem fine. Meanwhile the traces are heating up rapidly and as soon as you pick up the BMS (provided its heat shrinked) one or two resistors will melt off and stick to the heatshrink and if you're lucky you won't burn traces, but the board will be useless until the resistors are replaced or re-flowed. And most times that doesn't even fix it because something else burned up and didn't do it in an obvious way. 

i have a bin of dead BMSs that i killed this way. 

check your voltages on each balance lead to assure they are indeed sequential BEFORE plugging in the BMS. Do that 100% of the time and you will catch and fix errors before you cook off balance resistors.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-08-08T15:06:22.337Z Reads: 247

```
There should be some markings on the bms board where the balance wires connect that shows cell order
```

---
## \#6 Posted by: longhairedboy Posted at: 2017-08-08T15:11:18.917Z Reads: 249

```
@jga yep! there should be numbers screen printed right next to the pins. unless there is weird shit going on like in Evolves BMSs, pin one will go to the first positive after the negative side of the pack, then 2 to the second, three to the third.. etc.  The last pin will go to the same place your mains positive comes from but don't tie it into the mains, solder it right next to it.
```

---
## \#7 Posted by: dyingmoss Posted at: 2017-08-08T15:29:02.759Z Reads: 244

```
If i am using this BMS and wiring to 3x3s lipo's then I am not going to use any of the ground wires on any of the batteries correct? Also the last wire that is going to go on the main line is it going to be the last red wire on the Positive end of the main battery terminal? <img src="/uploads/db1493/original/3X/2/b/2b016715c66bfc07d1acd8d197e7f324f1a8ffc8.jpg" width="353" height="500">

This is the BMS i am using?

Following this diagram from @Namasaki
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014/72?u=dyingmoss

This will charge and discharge though the BMS correct??
```

---
## \#8 Posted by: Namasaki Posted at: 2017-08-08T15:35:49.804Z Reads: 226

```
That is correct
Please note that with this bms, the E-switch must be on while charging
```

---
## \#9 Posted by: dyingmoss Posted at: 2017-08-08T15:51:01.510Z Reads: 221

```
Will charger and charger plug be good enough to charge with? Also this switch can hook right up to the BMS power cables correct? 
http://www.ebay.com/itm/122146543795
http://www.ebay.com/itm/352048459383
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-08-08T16:23:16.974Z Reads: 204

```
[quote="Namasaki, post:8, topic:30062"]
Please note that with this bms, the E-switch must be on while charging
[/quote]

that's why i just went with the modded vedder switches and dropped the BMSs with built-ins. So annoying.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-08-08T17:33:46.031Z Reads: 202

```
To each his own I guess. 
Turning the board on to charge hasn't bothered me.
```

---
## \#12 Posted by: Mikenopolis Posted at: 2017-08-08T17:47:05.746Z Reads: 199

```
you totally should make a YouTube tutorial on battery build, BMS with LCD, charge port and power button. I would love to learn the process from professor Damon
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-08-08T18:00:25.751Z Reads: 195

```
well there's this thing that the motors do when the board's on the the remote is off... it doesn't do it when reverse is disabled but the motors sit there and tick-n-twitch. it drove me nuts so bad that i swore off reverse and swore off bms's with built ins. 

i know i know.. i'm just a picky little bastard
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-08T18:04:37.807Z Reads: 193

```
I've never used reverse. 
I have gotten twitching with remote off when down by the coast (maybe some interference)
I don't seem to have any twitching when at home.
```

---
## \#15 Posted by: Darby Posted at: 2017-08-14T14:12:31.828Z Reads: 191

```
<img src="/uploads/db1493/original/3X/d/7/d75738a17766d4eb92950226c7edca85092c8cc8.jpeg" width="640" height="480">
My ordering was corrected for me.. :) 

I have a question that's relevant to this thread, as I'm about to start soldering my BMS connections.  I was told that I should connect the B- and P- points before making the sensor connection. My plan was to do a bullet connection between the segment of wire already connected to the battery and one running to the BMS that I will solder.

 Is it ok for me to solder all the sensor wires without the B- connected and then Connect the B- bullet joint first, and then connect the sensor wires to the BMS? 

My assumption is this is fine as there wouldn't be any completed circuits until the connections are made, but as I'm new confirmation feels appropriate.  Thanks!
```

---
## \#16 Posted by: jga Posted at: 2017-08-14T15:43:17.502Z Reads: 180

```
Why don't you have a wire going the positive side of the cell where the main B- lead is?
Or maybe it's just the marking that is not at the right place as it gives the impression you have two on the B+
```

---
## \#17 Posted by: longhairedboy Posted at: 2017-08-14T16:46:33.971Z Reads: 176

```
i would run all of the balance leads first, before connecting to the BMS. Then use a volt meter to make sure you have them in the proper order. 

Then solder the pack into the BMS, then connect the balance leads. Then check the voltage again, and also to be triple sure, hold the bms for a few minutes and make sure its not getting warm. 

I do all of those things. I measure, i measure again, then i feel it and smell it. You just never know how something will go wrong so try to involve all of your senses, not just your eyes and logic centers.
```

---
## \#18 Posted by: Darby Posted at: 2017-08-14T16:47:26.053Z Reads: 172

```
I was wondering that too.. but all of the spots @kaly provided for me to do the soldering are on the negative in the chain.. EXCEPT # 12.. I don't know enough about how the Sensor cables actually function to provide an answer.. just enough to do the soldering and hook-up. :) with the correct instruction.
```

---
## \#19 Posted by: Darby Posted at: 2017-08-14T16:49:20.180Z Reads: 170

```
Thanks @longhairedboy! any confirmation on the order on the pack and the question brought up by @jga?
```

---
## \#20 Posted by: longhairedboy Posted at: 2017-08-14T16:52:26.716Z Reads: 174

```
if you're using the BMSs from batterysupports.com, the balance lead ordering will start at 1 at the first positive after the main negative. 

then if its a 12S, number 12 balance lead will be on the same metal as the positive terminal.
```

---
## \#21 Posted by: Darby Posted at: 2017-08-14T17:08:32.799Z Reads: 169

```
[<img src="/uploads/db1493/original/3X/7/5/756cd4251a2fc72e4106bb4a2a523c85cba9cba5.png" width="677" height="375">](http://)

I think it must be a different one that Ernesto uses.. I was just double checking the diagram he sent after the question and all the connection points are (while between + and -) they are made on the negative side of the (is it "parallels"?) He's built a number of function boards, so I can only imagine this is the correct way to do it for this BMS, I just don't know  the "why."

I'll certainly take the advice on the checking and double checking after I get it all hooked up.. and will solder first and connect after. Thanks!
```

---
## \#22 Posted by: longhairedboy Posted at: 2017-08-14T17:14:09.651Z Reads: 158

```
no, they're not. They're on the positive side. The diagram is ambiguous because its a 1P. But look at #12, and notice there is no balance on the negative side of #1
```

---
## \#23 Posted by: Darby Posted at: 2017-08-14T17:27:16.918Z Reads: 154

```
? so then are all these spots opened and waiting for me to solder in the incorrect location? @kaly can you chime in here? I think I've read some posts from @Eboosted who's done a Kaly build?
Also... I can simply solder this together as indicated in my photograph, where the current solder points were provided for me (not hook it to the BMS) and see if I'm getting the correct Voltage readings via the voltmeter.. ya.. I think I'll do that.
```

---
## \#24 Posted by: Kaly Posted at: 2017-08-14T19:53:51.279Z Reads: 149

```
Hi there
the spots are marked correctly, you are going to start connecting the balance leads by the positive side of the negative main wire, that is the one marked #1 on the picture above and them follow the diagram. notice that the balance lead has to be connected on the bridge part of the cell connection it can be on the positive side or negative side but on that join connection. 

As you can see on the picture i choose to put the tap on the negative side of the connection because in the event that the shrink wrap on the cell get scratch the metal tab will only touch the negative side of the cell on which is already connected minimizing any possible complication.

for more info check 
http://www.batterysupports.com/44v-48v-504v-12s-60a-12x-36v-lithium-ion-lipolymer-battery-bms-p-270.html
```

---
## \#25 Posted by: Darby Posted at: 2017-08-14T20:17:17.412Z Reads: 141

```
Thanks for the clarification Kaly! I gathered you had it done right, but with the new question there was some hesitation on my part. Uncertainty, I can do without when dealing with this much battery. :) 
Huge help here, thanks!
```

---
## \#26 Posted by: onramp Posted at: 2017-08-14T22:57:35.074Z Reads: 135

```
kaly, how do I get info and pricing on a build? Thanks.
```

---
## \#27 Posted by: jga Posted at: 2017-08-15T07:22:06.848Z Reads: 128

```
Practical question: how do you check the balance wires with the voltmeter?
```

---
## \#28 Posted by: longhairedboy Posted at: 2017-08-15T12:59:34.736Z Reads: 124

```
attach your negative probe to the negative side of the pack using a clip or something, then place your positive probe on each one of the connector contacts starting at pin 1. They should get progressively higher in voltage on each pin and the differences between each pin should be very very close in measurement, in fact they should all be the same as the measurement of one cell because the cells should have arrived with all the same voltages, which should be somewhere close to nominal (about half charge). So pin 1 should be around 3.6v while pin 12 should be around 43.2 for example. if they're at 3.2 or something like that its ok, i've seen cells arrive at 20% charge before and they turned out fine once the pack was built, charged, and balanced.
```

---
## \#29 Posted by: jga Posted at: 2017-08-15T13:35:51.285Z Reads: 123

```
Perfect! Thank you, I will give it a try tonight.
```

---

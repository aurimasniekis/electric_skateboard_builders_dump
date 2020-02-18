# Help me troubleshoot my board - FAULT_CODE_LOW_V

### Replies: 22 Views: 1307

## \#1 Posted by: wookiepedia Posted at: 2017-02-12T14:37:42.895Z Reads: 76

```
Hello, everyone!

I am having some trouble with my first build and would like some assistance in troubleshooting the issue.  My build thread can be located here:  http://www.electric-skateboard.builders/t/flatlander-firstbuild-meb-freestyle-deck-fun-box-10-trucks-carvon-v2-5-single-direct-drive-meb-12s2p-liion-pack-vesc/14175

Relevant parts in use:
Miami Electric Boards 12s2p 18650 based battery pack
Power switch from Miami Electric Boards
VESC from Carvon running firmware 2.18
Carvon v2.5 hub motor

Symptoms:
When I accelerate hard, the motor will no longer be driven and I will coast.  Battery voltage reading in VESC Connect app will drop from ~42V down to 12.7V and dropping.  If I time it correctly and apply some brake, battery will jump back to previous 42V+ level and board will remain powered on.  Sometimes, however, the board shuts down entirely even though the power switch is turned on.  When the board completely powers down, I also get a FAULT_CODE_LOW_VO (I assume it's "voltage" and just being truncated by the display).  Also, the duty cycle in the VESC Connect app will jump from wherever I was (usually about 50-55%) up to 95% when this happens.

What I have done to troubleshoot so far:
I have tweaked many many settings on the VESC, most of which seem to make the problem worse.  I have disabled FOC and gone back to using BLDC to see if this caused the issue.  In doing so, I had much trouble with performing motor detection, which often forced the problem to occur during detection.  I performed a "read default configuration" to get back to sane values and was able to get the motor detected properly.  Every time I try to do detection, the first attempt fails inside of BLDC tool, but the second try gives me useable values.

Because I was experiencing issues with the power switch, I wired the battery directly to the VESC, and still experienced the cutouts of throttle.  I was, however, able to get the motor back online by applying brake to "jumpstart" the VESC back up.


What I plan to do next:
I will be  taking detailed screenshots of my VESC settings and I also saw some great data logging that others have posted in their troubleshooting threads using metr, so I will be playing with that to gather some data.  Please let me know what information would be helpful to diagnose this issue.  Also, I think I will be duct taping an action camera to the underside of the board to watch the voltage display on  the battery pack to see if the voltage is actually sagging when the motor cuts out, helping me to pinpoint the issue to the battery pack or eliminate it as a suspect.

Thanks in advance for your help, folks!
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-02-13T01:08:26.795Z Reads: 51

```
Make the check with the video on the voltage display. I think the voltage really collapse. If the battery has a BMS then I think that's the issue. Otherwise your battery has some trouble. 

You don't need to check your settings. There is nothing I can think of that could cause a voltage collapse on the VESC.
```

---
## \#3 Posted by: wookiepedia Posted at: 2017-02-13T01:15:03.071Z Reads: 51

```
I have been playing with the board most of the afternoon, and the problem comes up only when the battery goes below 75%.  When the battery  gets to around 50% of capacity, the problem becomes unreasonable (can't use the board at all, hard shuts down every time I try to throttle even the slightest bit).

I had the battery down below 50% and managed to watch the display while free wheeling (board laying on its back plugged in to BLDC tool) and the battery voltage sagged a bit, but was well above 42V when it cut out.

I think you're right, it may be a BMS board that's gone south.  I've reached out to the vendor that I bought the pack from to see what my options are.

Thanks for replying!!
```

---
## \#4 Posted by: Ackmaniac Posted at: 2017-02-13T01:20:02.298Z Reads: 49

```
That means your battery is at 3.5V a cell when you give no throttle. That is more or less already empty. So your cells are already discharged and then they collapse when you try to get some power from a already empty cell. 
Get a bigger battery.

Set the battery cutoff start to 36V and the cutoff end to 33.6V. 

I thought your problems also happen when the battery is full.

And don't trust what these external voltage meters show. They show something but not more. Never trust them.
```

---
## \#5 Posted by: wookiepedia Posted at: 2017-02-13T01:37:22.561Z Reads: 45

```
From my most recent testing, the issue of hard cutouts started when the cells hit 3.7V.  This is the nominal voltage of a samsung 25R cell, and I usually can beat these cells down in other applications to about 3.4V or lower.  Am I expecting too much of these batteries?
```

---
## \#6 Posted by: Alextech Posted at: 2017-02-13T02:23:42.507Z Reads: 44

```
What is your max amp pull on your Vesc.
```

---
## \#7 Posted by: wookiepedia Posted at: 2017-02-13T03:28:55.506Z Reads: 44

```
Max battery amp draw I've seen is just under 7A.  Motor amperage, I think I've seen up to about 35A or so.

I just charged the pack up, and noticed that instead of a solid red light to charge, I was getting the red light flashing off and on for the last 30 minutes of the charge and the battery topped out at about 49.1V.  I think my battery pack may be dead.  :-(  Board wouldn't even move at all and just kept shutting down.
```

---
## \#8 Posted by: Alextech Posted at: 2017-02-13T03:30:01.423Z Reads: 41

```
You may have cooked your battery. It's only rated at 40a and your fairly close to it.
```

---
## \#9 Posted by: wookiepedia Posted at: 2017-02-13T03:52:26.367Z Reads: 42

```
The battery pack I bought has a 50 amp BMS in it.  I'm curious how a 7 amp draw would have killed it.  Am I misunderstanding the VESC settings?  The highest I had my VESC configured for battery current draw is 40 amps.
```

---
## \#10 Posted by: Alextech Posted at: 2017-02-13T03:58:08.894Z Reads: 44

```
You have a 12s2p. 

The Samsung 25r is a 20a cell, 2 in parallel is 40a maximum from the cell, don't matter if the BMS is 1000a the pack can only provide 40a. Your Vesc could have been slightly pulling more and killing the cells slowly leading to a dramatic faliure. Also the Samsung 25r voltshe sags alot when it's near its 20a pull. So that may explain low speeds.
```

---
## \#11 Posted by: Ackmaniac Posted at: 2017-02-13T08:46:41.856Z Reads: 37

```
If you had the battery max at 40A then it should have been OK for Samsung 25R. But are you sure that your battery pack has them. I see the new batch from Miami Boards uses Samsung 30Q but i guess you have a older batch.
And what were your battery cutoff start and cutoff end settings?
```

---
## \#12 Posted by: wookiepedia Posted at: 2017-02-13T14:48:14.909Z Reads: 34

```
I think I got the very last one built with 25R's.  I was out testing the board and had the battery cutoff points set low to see if that was the cause and monitoring voltage on my phone with vesc monitor while circling a parking lot.  I think the lowest voltage I saw was just above 42V.

I am going to drop my current limit to 30A, and see if an all night charge resurrected the pack.  If not, I will be moving to a 12s3p pack or looking at lifepo4.  I am quite convinced that this failure was self inflicted now.
```

---
## \#13 Posted by: TarzanHBK Posted at: 2017-02-13T15:28:23.459Z Reads: 32

```
12s3p should be minimum with 25Rs.
If you build lower, like you did with 12s2, you´re going to kill the battery after the first few hills.
This setup delivers 40A max, healthy is probably more at the 30A side and thats not much!
Always build something with a bit wiggle room on top!
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-02-13T15:41:25.605Z Reads: 29

```
I have to disagree. If your pack is made with samsung 25R it will be ok as long as the battery cutoff start and cutoff end is set properly.
So in your case the cutoff start should be at 3.0V a cell (12S * 3.0 = 36V)
and the cutoff end at 2.8V a cell (12S * 2.8V = 33.6V)

This way the VESC takes care that the voltage doesn't go below that when draw high amps. I guess you had lower settings and by that you stressed the cells to much. 

And if your cells are Samsung 25R you can use 40A without issues. The average consumption is below that. Only problem is that you have a relatively short range. And after a couple of kilometers you will hit the cutoff limits and your power gets reduced.

So what were your old battery cutoff start and cutoff end settings? Because i think that this is the reason for your problems.
```

---
## \#15 Posted by: wookiepedia Posted at: 2017-02-13T15:47:09.756Z Reads: 26

```
When I was testing, I had cutoff start at 33 and stop at 30.  This may have killed the pack.
```

---
## \#16 Posted by: Ackmaniac Posted at: 2017-02-13T16:03:30.806Z Reads: 25

```
2.5V a cell (12S * 2,5V = 30V) is the edge. So that's low but not too low. Just use 36V and 33.6V for the future to give them a bit more space. Because below 2.8V the cells start to press out the last bit of juice they have. 
Just charge your battery, use my settings and give it a try.
```

---
## \#17 Posted by: wookiepedia Posted at: 2017-02-13T16:05:30.267Z Reads: 25

```
I just modified my current settings to 30A for battery and motor and changed my cutoff values to 36V/33.6V and tested the board in the house.  At least it now will move, so that's a good start!  I was still able to cause the system to shut down entirely by slamming the throttle forward, but at least this is workable.  I will have to look into some sort of throttle input smoothing or similar.  When my next round of conference calls is over, I'll go take the board for a quick spin and see how it does actually getting up to speed and such.

Thank you so much for your input!
```

---
## \#18 Posted by: Ackmaniac Posted at: 2017-02-13T16:08:31.731Z Reads: 25

```
The problem is that your battery is already empty now. So you push the throttle and a little bit of current draw causes the cell to collapse. Just charge the Battery and when you realize in the future that your boards start to loose power then try finish your run soon. And when you only can get a little bit of power then stop your run.

You have to undertstand that there is a difference of the the battery voltage when you draw no current and the situation when you draw current. So for example when the battery is at 3.5V a cell when you draw no current then it is already empty. When you draw current from that cell the voltage collapse because it is already empty.

In this picture you see how much juice you have left when you draw no current from the battery.
<img src="/uploads/db1493/original/3X/7/2/724cb9047cb6a9b3060240e82c5c3073c2b9983b.jpg" width="281" height="500">
```

---
## \#19 Posted by: wookiepedia Posted at: 2017-02-13T16:13:35.376Z Reads: 25

```
Battery pack BMS has been hooked up to the charger / power supply all night to trickle it back up to 49V neighborhood.  I do think I've done permanent damage to the cells, though, as the voltage sags pretty severely whenever I hit the throttle.

Looks like I might be upgrading to one of @oriol360 's new 12s3p 30Q based packs soon.  Like, on wednesday.
```

---
## \#20 Posted by: Ackmaniac Posted at: 2017-02-13T16:14:47.393Z Reads: 24

```
Could be the case that the cell are already damaged.
```

---
## \#21 Posted by: wookiepedia Posted at: 2017-02-13T16:21:17.721Z Reads: 25

```
I just realized that I'm using your VESC Monitor app on my phone to do my troubleshooting.  Thank you so much for making such a useful tool.  If you're ever in north texas, I'd love to buy you a few beers (and go ride!).
```

---
## \#22 Posted by: Ackmaniac Posted at: 2017-02-13T16:22:21.985Z Reads: 25

```
If i do another world trip i come back to that offer.
```

---

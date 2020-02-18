# Getting throw off the board! Please help

### Replies: 8 Views: 1005

## \#1 Posted by: jesser722 Posted at: 2017-04-21T19:04:58.667Z Reads: 157

```
My board just started braking at random times and throwing me off. I have the winning remote, would this be the issue? or would it be vesc/motor issues?
```

---
## \#2 Posted by: yaca Posted at: 2017-04-21T19:16:25.659Z Reads: 157

```
Did you adjust failsave to neutral 50%?
[https://www.electric-skateboard.builders/t/has-anyone-not-had-issues-with-the-winning-remote/8524/161](https://www.electric-skateboard.builders/t/has-anyone-not-had-issues-with-the-winning-remote/8524/161)
```

---
## \#3 Posted by: jesser722 Posted at: 2017-04-21T21:56:30.910Z Reads: 121

```
Where do i find those settings?
```

---
## \#4 Posted by: psychotiller Posted at: 2017-04-21T22:09:05.020Z Reads: 118

```
Instructions for the failsafe are on my site.
https://psychotiller.com/product/winning-24ghz-mini-thumb-stick-controller

You will also need to adjust the min/max pulse width settings on your vescs.
```

---
## \#5 Posted by: jesser722 Posted at: 2017-04-21T22:17:38.981Z Reads: 100

```
what is a good setting to have them at?
```

---
## \#6 Posted by: psychotiller Posted at: 2017-04-21T22:35:58.606Z Reads: 98

```
When you are plugged into your bldc tool. You'll see the apps tab on the top. Click on that and then click the ppm tab  on the side. 

Click read configuration, click disable in control mode and then click write configration at the bottom.

Now, at the bottom there is a display bar. select display, turn on your remote and pull full brake on your remote. Hold it and look at the pulse width number next to the display. You might see 1.04? now type what you see in the minimum pulsewidth box. (it's next to the uart tab)
Now go full throttle and type what you see into the maximum pulsewidth box.

Below click on write configuration. 
The display bar should be hovering around the 50% mark now. If you're at 52% you can "raise" your minimum pulsewidth number a couple of points. Example change 1.04 to 1.06 and when you hit write you'll see your diplay get closer to 50%. 
Hit write again to check.

Then go up to the top and change your control mode to "Current, no reverse with brakes"

Click write configure and you are done. Make sure your drive wheels are in the air before you try your remote. You're wheels are live now.

Now do the failsafe from my website.
```

---
## \#7 Posted by: yaca Posted at: 2017-04-21T23:18:01.762Z Reads: 84

```
If neutral after setting the pulsewith is not at 50% you can also use the throttle trim on the remote - below the two LEDs. You need a small screw driver. Check again the min and max pulsewith after using the throttle trim.
```

---
## \#8 Posted by: brun Posted at: 2017-06-05T06:49:00.302Z Reads: 46

```
Just got thrown off my board...first time ever.  Been riding for a year or so and this is my second board.  I was going about 20mph, when it I experienced a complete un-commanded full break. I was wearing a hemet, padded gloves and a jacket otherwise I'd have a banged up head and badly scraped hands right now. I hit the pavement hard Pete Rose style and felt very lucky to walk away with some bruises and cuts.   Not sure how long it's going to take to get me back on, at least until I can pin point the problem.  My trust is at a low point.

I've ridden this board several times for a total of about 1 hour with absolutely no problems.  On the last ride and early on in this ride, I had felt some very quick and subtle, power pulses.   Stupidly I didn't pay enough attention to the signs.  

I don't think the uncommanded brake was due to low batteries in the remote.  The batteries are fine in the remote (DIY) and seem to work after I limped home and bench tested for 15 minutes.  

I do think suspect the connection between the receiver and the VESC.   I hadn't yet soldered the connections, using only the male-female connection with a little electric tape.  I think the vibration during the ride had loosened this up just enough to create a bad connection. Something about how a PWM signal behaves when it's interrupted in this way must look like a break command. (Ie the vesc receives a  pulse width < the 50% mark, maybe just for an instant)

I've had loose receiver/vesc connections issues before and have seen everything from a simple dead-stick where the board just coasts to a stop (the ideal), to full un-commanded acceleration...and both times this was from vibration and poor connection.  I can probably fix this with a soldered connection, hot glue and lots of padding.  I'll be riding very slowly for a while.  

That said, the VESC control logic clearly needs work.  It should settable to ignore brief and unrealistic stop commands, especially higher throttle settings and speeds.  While I do want to be able to deliver -40-50AMPs at full break, I don't want to go from even 50% power on to 50% break in an instant.  Even in the most urgent breaking scenarios, where the i want to apply full break intentionally, there is a limit to how quickly the VESC should respond.   There is no way to be prepared for that kind of deceleration.  I've read the control logic for PWM on the VESC and there is nothing there to second guess the controller, or limit the RATE of increase of breaking.

Again, my fault for not paying attention to the warning signs.  Next time, if my board isn't feeling absolutely 100%, it's getting opened up and figured out before heading out.  

I'm going to have another look at the code, and maybe re-write the throttle control and brake ramping.  I hear a firm ware update is coming out soon with lots of changes.  Anyone happen to know when?

Be safe.
```

---

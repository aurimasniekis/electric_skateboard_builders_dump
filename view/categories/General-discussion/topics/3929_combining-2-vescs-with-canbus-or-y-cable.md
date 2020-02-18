# Combining 2 VESCs with CANBUS or Y-CABLE?

### Replies: 26 Views: 3535

## \#1 Posted by: c4Lvin Posted at: 2016-05-28T07:11:07.523Z Reads: 284

```
Guys I know there is a canbus cable but can I just get a cheap Y splitter cable on ebay for a buck instead? Any disadvantages from the CANBUS cable? What connector plug type does it use?  I know it's just a black and white cable.  Any thoughts are greatly appreciated.
```

---
## \#2 Posted by: flatsp0t Posted at: 2016-05-28T07:28:32.770Z Reads: 283

```
The VESC is capable of traction control if you connect two over CAN
```

---
## \#3 Posted by: c4Lvin Posted at: 2016-05-28T07:38:40.444Z Reads: 279

```
Ok so that's good to know.  Can I make that connection myself?  Thanks again!
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-05-28T07:40:34.061Z Reads: 273

```
you can, i dont know the connector type.
you also can simply buy it
http://www.ollinboardcompany.com/product/canbus-connector-for-vedder-s-motor-controller

Or you can solder the connection
```

---
## \#5 Posted by: Hummie Posted at: 2016-05-28T07:42:14.117Z Reads: 257

```
I'd like to solder it but ...have u done it or have advice?
```

---
## \#6 Posted by: Jinra Posted at: 2016-05-28T08:02:54.970Z Reads: 251

```
If you have spare computer parts or a spare computer case, you can use the power button/LED wires for the connection, you'll need to snip the wire and put another header on there though.
```

---
## \#7 Posted by: flatsp0t Posted at: 2016-05-28T08:05:44.441Z Reads: 248

```
Or if you have an  Raspberry / Arduino, you can use two single gpio wires
```

---
## \#8 Posted by: trbt555 Posted at: 2016-05-28T18:30:37.511Z Reads: 225

```
The CAN bus connection is nothing more than just two wires. It can't get any simpler than that.
```

---
## \#9 Posted by: Hummie Posted at: 2016-05-28T18:45:40.298Z Reads: 224

```
Is there a risk of overheating the rest of the board?

Also you're the only person I've come across who has an explaination for how voltage reduces heat in a motor. I remember long ago you explained it as similar to an ac circuit or something..could you again!?  It was a while ago.  As of lately I can't find such an explaination
```

---
## \#10 Posted by: c4Lvin Posted at: 2016-05-28T19:49:14.451Z Reads: 217

```
Thank you. That's just the answer I expected! I've read that the CANBus is only for data transmission. It still needs additional wires for power? More research and reading to do! Thanks guys.
```

---
## \#11 Posted by: trbt555 Posted at: 2016-05-28T20:04:55.849Z Reads: 222

```
Power equals Voltage x Current : P=U x I
So for any given Power, Voltage and Current will be inversely proportional.
Raise the voltage and the current will drop proportionally.
Dissipated heat is quadratically proportional to current.
If you halve the current, you quarter the heat.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-05-28T20:06:52.134Z Reads: 220

```
http://www.electric-skateboard.builders/t/vesc-faq-connect-two-vesc-via-canbus-for-dual-motors/142
```

---
## \#13 Posted by: sgaana Posted at: 2016-05-28T22:22:45.852Z Reads: 208

```
I don't have much soldering skills, so I crimp both ends of both wires and connect to a 4 pin JST-PH 2mm female connector. Then connect to male connectors in each VESC.
Here is a picture of how I made it.
http://www.electric-skateboard.builders/uploads/db1493/original/2X/c/cfeba170a336a6d581be09e5f60ad901e6c1d3ec.JPG
```

---
## \#14 Posted by: Hummie Posted at: 2016-05-28T23:27:04.133Z Reads: 195

```
But you get the same heat to torque ratio regardless of what winding you have.  So running a given motor at 100 volts and one amp will produce the same heat as a motor at 1 volt and 100 amps.  Do u have a link that better explains what you're saying about the dissipated heat being quadraticly proportional to current? 
If you raise the voltage on a given motor the current won't drop unless the winding has more turns.  More turns means thinner wire and greater resistance and more heat.  I read they end up the same
You can't just add more volts to the same motor and expect it to run cooler in fact it will run hotter as the motor is most efficient running at 80% of its no load rpm.  This is what I read

Volts x amps being power I think is more so a potential.   In terms of power out... Torque x speed. Speed is a potential of voltage but not a gaurentee
```

---
## \#15 Posted by: c4Lvin Posted at: 2016-05-29T03:14:18.611Z Reads: 184

```
Thanks sgaana! Where did you get those JST-PH connectors? I assume eBay as well since I've seen them before. What wire gauge did you use for the two wires? Thank you for the picture references.
```

---
## \#16 Posted by: sgaana Posted at: 2016-05-29T05:34:33.356Z Reads: 181

```
Local electronics store.
I'm not sure about wire gauge size. I explained to my local store what I was going to build and they said any wire would work, as long as you can crimp them.
I am not too handy and did not have tools to do this. I ended spending money buying tools and tried tens of times before I got it right. But it was a nice learning experience. 
You can buy from some members of this forum for reasonable price and they are well made, unlike mine. . 
http://www.ollinboardcompany.com/product/canbus-connector-for-vedder-s-motor-controller
http://www.hellray.de/shop/#!/eSkateboard-JST-PH-2mm-Kabel-für-VESC-mit-4-Pin/p/60319783/category=15255004 (you need only two middle wires)
```

---
## \#17 Posted by: trbt555 Posted at: 2016-05-29T07:58:29.597Z Reads: 180

```
[quote="Hummie, post:14, topic:3929"]
So running a given motor at 100 volts and one amp will produce the same heat as a motor at 1 volt and 100 amps
[/quote]
FALSE.

Look up the equation for *Joule Heating*, you'll find the heat produced is proportional to I squared.

P= V x I is one of the most basic electrical engineering equations out there. It doesn't matter if it's a toaster putting out 500W or a brushless motor putting out 2500W, this equation governs the relationship between Power, Current and Voltage. 

With respect, If you want to doubt this, feel free to do so, but don't try to convince me.

Now let's not hijack this thread any further.
```

---
## \#18 Posted by: Hummie Posted at: 2016-05-29T08:02:22.375Z Reads: 164

```
We will see.  Ur changing the situation.  I'm interested. But too tired.  I'll find you a good rebuff in the morn
```

---
## \#19 Posted by: Hummie Posted at: 2016-05-29T08:09:29.074Z Reads: 163

```
heat produced is related to the thickness and length and material of the wire and ultimately it's resistance

Power ... I don't know.  Do you believe that if you add 100 volts to the set-up you're running now it will be more efficient?
```

---
## \#20 Posted by: trbt555 Posted at: 2016-05-29T14:47:40.248Z Reads: 157

```
Dude, why the hell do you think electrical power distribution networks run at voltages in the kiloVolt range and not just plain 110V or 230V ?
I'm done discussing the obvious.
```

---
## \#21 Posted by: Hummie Posted at: 2016-05-29T16:27:30.266Z Reads: 149

```
Motors are not power lines.  If that's the extent of your rational for believing motors run cooler with more volts I'll let it rest and keep believing those who have a better rational.   There are a lot of people who believe the same as you but it's not true 

http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

Read the first two paragraphs.
```

---
## \#22 Posted by: trbt555 Posted at: 2016-05-29T17:30:16.738Z Reads: 152

```
You really are clueless aren't you ?

I am very familiar with Vedder's post and I'm even more familiar with basic electrical engineering principles, I use them on a daily basis in my profession.

It's not about believing or not believing, it's physics.

If YOU want to *believe* someting else, go ahead but stop trying to drag me down to your level. Next thing you'll start saying the earth is flat.

I'm done, you're now on my ignore list, idiot.
```

---
## \#23 Posted by: Hummie Posted at: 2016-05-29T17:48:13.356Z Reads: 146

```
Wow. I guess a discussion about science is too hard for some people.  Too bad you couldn't bring some real science to the table.  I will for you and I'll post it here.  But I guess u won't get to see it.
```

---
## \#24 Posted by: Hummie Posted at: 2016-05-29T18:08:52.527Z Reads: 146

```
http://www.rcgroups.com/forums/showthread.php?t=675160

From the link above by someone who knows what they're talking about. 

 "Motors themselves do not show any real efficiency gains with higher voltages if they are wound to take them correctly

That is, at similar RPM two motors - one on 3s wound with three turns, one on 6s wound with six turns, will behave identically.

However the gains are to be had in the wiring and speed controllers, which can be of lighter gauge wire, and/or use smaller and lighter transistors."

I'll find a couple more links and quotes and put them here so people aren't misled.


http://www.rcgroups.com/forums/showthread.php?t=286610


http://vedder.se/forums/viewtopic.php?f=6&t=6&p=1375#p1375

dont think u even can block people here.

Wonder if he will come back and admit he's wrong or hide under a rock.  Try to help him and...
```

---
## \#25 Posted by: Chris604 Posted at: 2016-07-26T03:18:33.372Z Reads: 130

```
Do you get traction control off this connection?
```

---
## \#26 Posted by: sgaana Posted at: 2016-07-26T06:53:18.703Z Reads: 116

```
You mean good connection? Yes.
```

---

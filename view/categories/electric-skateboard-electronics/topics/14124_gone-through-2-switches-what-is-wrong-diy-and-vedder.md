# Gone through 2 switches, what is wrong; DIY and Vedder

### Replies: 21 Views: 2069

## \#1 Posted by: jasonyng Posted at: 2016-12-03T17:16:36.431Z Reads: 208

```
I have a 12s4p battery that had what looks like a power switch from DIY.  After about 10 on/off while setting up the board it would no longer turn off.  I replaced it with a vedder anti spark and after more testing and setup (never used while riding) it has failed after about 20 on/off.

Why are these switches failing and what am I doing wrong.  Neither was used under riding circumstances just assembly on my bench. 

Any help would be greatly appreciated.

Thanks,
Jason
```

---
## \#2 Posted by: Eboosted Posted at: 2016-12-04T03:47:52.568Z Reads: 186

```
The Vedder switch failed? I though those were very reliable
```

---
## \#3 Posted by: Pathaim Posted at: 2016-12-04T03:55:52.957Z Reads: 182

```
Do you have a max amp limit in the vesc? Is it possible you pulled allot of amps while going uo a hill etc and blew it?
```

---
## \#4 Posted by: jasonyng Posted at: 2016-12-04T04:31:33.243Z Reads: 184

```
I have the amp limit set to 25 on both VESCs and it went bad on the bench.  It never had any riding time so I would assume very little amps would have been through it.

Here is a picture of the vedder and everything looks good. 

<img src="/uploads/db1493/original/3X/b/4/b4c29eae458c2a295a04f7bb96885489964d9aee.jpg" width="666" height="500">

I tested the toggle switch and it looks ok, but I can't test at the switch end.  Is there anyway to test the vedder without the toggle?  

Thanks
```

---
## \#5 Posted by: Pathaim Posted at: 2016-12-04T06:36:18.540Z Reads: 172

```
Abit off topic but can I ask where you bought the vedder switch?
```

---
## \#6 Posted by: barajabali Posted at: 2016-12-04T06:39:00.200Z Reads: 171

```
I built the battery with a Flier switch. ( switch fried which happens sometimes with them) so I sent out an ollin board vedder switch free of charge (all of my batteries come with them as of a while ago) and it fried also. 

Maybe @chaka can chime in with any tips

P.s. I've sold about 20 vedder switch battery packs with zero problems and I've used them on my personal Killer Trampas which pull immense amps and 12s. So im not sure what the issue is.
```

---
## \#7 Posted by: barajabali Posted at: 2016-12-04T06:43:46.345Z Reads: 164

```
Also on testing the switch without the toggle, you'd have to connect the pins but which particular ones, Im not sure.
```

---
## \#8 Posted by: jasonyng Posted at: 2016-12-05T02:51:36.561Z Reads: 137

```
Any other thoughts before I try and get another switch?

Thanks
```

---
## \#9 Posted by: chaka Posted at: 2016-12-05T15:02:13.477Z Reads: 127

```
The two outer pins are Ground and Positive. Connecting the center pin to Positive turns the switch on, connecting the center pin to Ground turns the switch off. It is possible that your mosfets have failed but it could also be a wiring issue between the switch and toggle.

I doubt the mosfets have failed unless you have a huge bank of capacitors to charge when you power up your system.

If trouble shooting doesn't correct the issue you can send the switch to our shop and we will fix or replace your switch.

One question, are you toggeling the switch rapidly? That will fry a switch sometimes at 12s, it can cause the switch to heat up.
```

---
## \#10 Posted by: jasonyng Posted at: 2016-12-05T15:25:22.710Z Reads: 118

```
Great I will try and bypass the toggle switch tonight.  No rapid on and off, I really only turned it on and off maybe 20 times total.

One last question, the plug for the toggle is that a Mini Micro Jst 2.0 Ph 3 Pin Connector?

Thanks
```

---
## \#11 Posted by: chaka Posted at: 2016-12-05T15:34:38.665Z Reads: 111

```
Yes, jst-ph 3pin. https://www.digikey.com/product-detail/en/jst-sales-america-inc/PHR-3/455-1126-ND/527357

You also need a crimper and terminals to make your own. An alternative would be to remove the jst header and directly solder the toggle wires to the pcb.
```

---
## \#12 Posted by: jasonyng Posted at: 2016-12-06T02:50:04.236Z Reads: 101

```
I tested without the toggle switch and still have the same issue, it wont power off.

Jason
```

---
## \#13 Posted by: chaka Posted at: 2016-12-06T14:49:22.935Z Reads: 94

```
You can find all our shipping info and address on our support page. [http://www.ollinboardcompany.com/support](http://www.ollinboardcompany.com/support)

Send it in and we will get it working again.
```

---
## \#14 Posted by: jasonyng Posted at: 2016-12-06T15:17:51.678Z Reads: 90

```
Cool, I will try and send it out today.  One of the wires on the toggle switch also broke off, I am assuming from the plugging and unplugging I have been doing to test, I will send that as well and if I could just get a new end put on it would be greatly appreciated.

Thanks!
```

---
## \#15 Posted by: chaka Posted at: 2016-12-06T15:20:18.938Z Reads: 89

```
Yeah, no problem. Only takes a few seconds to re-crimp with new terminals.
```

---
## \#16 Posted by: jmasta Posted at: 2016-12-06T15:29:27.544Z Reads: 85

```
FYI, my wires got pulled out of the JST connector as well. I only unplugged the switch once

Not a big deal because I was going to replace the switch anyway. Just thought you should be aware.  It might be better to solder wires directly to the board and use an inline connector
```

---
## \#17 Posted by: chaka Posted at: 2016-12-06T15:41:43.403Z Reads: 81

```
I don't recommend pulling the wires to disconnect jst ports. They have a little locking tab and you need to grip the plastic housing when disconnecting ports.
```

---
## \#18 Posted by: jasonyng Posted at: 2016-12-06T15:46:00.373Z Reads: 79

```
No doubt I think I just did to much fiddling with mine.  Is there any solution that would send that out at a right angle instead of straight up? I am a little worried as it sits on top of my battery pack and that is the tallest point of the pack.
```

---
## \#19 Posted by: chaka Posted at: 2016-12-06T16:27:41.414Z Reads: 78

```
I actually use right angle jst's on the switches now, I'll swap it out for you.
```

---
## \#20 Posted by: jasonyng Posted at: 2016-12-06T16:29:28.721Z Reads: 80

```
Awesome thanks!
```

---
## \#21 Posted by: jmasta Posted at: 2016-12-06T18:36:14.337Z Reads: 77

```
[quote="chaka, post:17, topic:14124, full:true"]
I don't recommend pulling the wires to disconnect jst ports. They have a little locking tab and you need to grip the plastic housing when disconnecting ports.
[/quote]

I think it would be helpful to include that recommendation with the product or listed on your site.  The connector is hidden under shrink wrap and sandwiched between two stiff high gauge wires. Most people's first instinct when attempting to remove the JST connector will be to pull gently on the wires
```

---

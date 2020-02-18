# VESC configuration for Flipsky Mini ESC 4.20, Ownboard Samsung 30Q (10S 6.0Ah), and Flipsky 6355 motors

### Replies: 26 Views: 2040

## \#1 Posted by: chrischo1996 Posted at: 2018-09-23T22:44:26.641Z Reads: 259

```
I am looking for some help making these parts work well in conjunction.
[Dual Flipsky Mini 4.20](https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike)

[Dual Flipsky 6355 Motors](https://flipsky.net/collections/accessories/products/6354-190kv-2450w-2) 

[Ownboard Samsung 30Q 10S 6Ah batteries](https://www.ownboard.net/products/ownboard-electric-skateboard-battery?variant=6940852715562)

I need help with motor min, max, battery max, etc.
Also any suggestions on whether to run FOC or BLDC.
I've done a lot of reading on these topics, but I am not sure I fully understand it and would like any insight with someone with more knowledge and experience than me.
Let me know if you need any more information about my build.

Thank you!
```

---
## \#2 Posted by: brenternet Posted at: 2018-09-23T22:51:14.695Z Reads: 248

```
As it stands I don't think many people have experience with the FESC Mini 4.20. I would probably be cautious personally and use BLDC until some testing has been done here.

I'll let someone more knowledgeable give you settings!
```

---
## \#3 Posted by: chrischo1996 Posted at: 2018-09-23T22:53:54.563Z Reads: 241

```
I'm still waiting on my battery from Ownboard, but yeah I will definitely have to be cautious. How do people usually test? Set some settings, ride around, check temps, then change settings?
```

---
## \#4 Posted by: brenternet Posted at: 2018-09-23T22:57:27.569Z Reads: 239

```
Well on these there appears to be a capacitance limitation which is leading to cut outs under stress (heavy braking or acceleration) - Which is easy enough to see through a fault or your board simply not responding until you release the remote trigger/dial to allow it to reset.

This is on other models though, the mini is largely unreported.

Also a lot of people here will buy it to chuck on and test it out, if this is your main/first build you might want to let them do the testing and keep it simple for yourself as not to damage your esc and leave yourself without something to ride!
```

---
## \#5 Posted by: Riako Posted at: 2018-09-23T23:11:43.231Z Reads: 217

```
I would like to try those Minis ... but they won't work with CAN (made another wire but even if the other work on my mtb but ... nothing passed, I will send them back). I haven't try splitting the signal but I will when they return back if still not working ...
But detection and parameters in vesc tool work as good as for dual and test bench working great on the master :smile: 
https://amadridefr.files.wordpress.com/2018/09/img_20180919_205314-e1537384234306.jpg
I should make my Quattro with 4.12 ... :sweat_smile:
```

---
## \#6 Posted by: chrischo1996 Posted at: 2018-09-23T23:19:15.005Z Reads: 207

```
Shame about your canbus connection, hope mine work...
```

---
## \#7 Posted by: Riako Posted at: 2018-09-23T23:22:38.766Z Reads: 205

```
Don't really what I can do more, I switch them try again parametric the master in slave and vice-versa ... the slave won't run ... but it should work in single...
```

---
## \#8 Posted by: chrischo1996 Posted at: 2018-09-23T23:24:04.460Z Reads: 205

```
I have a dual setup, once I get my battery and am able to test I will post.
```

---
## \#9 Posted by: luv2sk8te17 Posted at: 2018-09-26T13:55:24.128Z Reads: 190

```
I had some issues at first. I was expecting waaay to much from this vesc. Here are some settings that got me going with few cutouts. They will probably go away once I gear it down a tad more. I also probably have too big of motors. At least they stay really cool.

Motor max: 35(30 if you want even less cutout)
Motor max brake: -35
Abs max: 130(this can prob go to 140)
Batt current Max: 50(35-40 if you have li ion pack or want to be more safe)
Batt max regen : -10(maybe -15 if you need more braking power and your battery can handle it)

I had issues with setting up ppm and can/bus connection as well. It would only work if I set up the side with the receiver wire coming out of it as the master. First plug in the opposite side and do the input wizard to setup as slave. Then go to other side and set as master. You should then be able to setup your controller.

I also found it very helpful to set some negative expo in the controller under throttle curve. This kept it from nailing the throttle and cutting out. You also need to go under the wattage tab and change the max wattage to match your motor. This lets the controller know that 100% throttle is the max watts and also helps with throttle sensitivity. I had an issue where quarter throttle was full throttle. 

Good luck to ya!

![29de12a96115e052fda5c847aa3ec871a11e8246_1_375x500|375x500](upload://zQblQYr43ZrZUAhY8sq7SNyZo2W.jpeg) ![90dd51f08899c10a6426057b239c4fcca3e37d61_1_666x500|666x500](upload://lvdjK3T4atd6IfrW3xvj5LJRVRK.jpeg) ![515ddaa630571bccacab39775957c63c668e061a_1_375x500|375x500](upload://w7BZmRrsxKWsfQijqhkW8NCezBy.jpeg)
```

---
## \#10 Posted by: gaetjen Posted at: 2018-09-26T14:05:38.472Z Reads: 172

```
I also had the problem of my two minis not working in dual with can, but the customer service was really nice and they let me send them back for a refund. They even paid for the shipping back.
```

---
## \#11 Posted by: chrischo1996 Posted at: 2018-09-26T14:11:13.628Z Reads: 175

```
Am I correct in assuming that you're running 12s lipo? I believe the esc's do a little better when they're running in 10s, but I'll have to see. Thanks so much for the suggestions, I'll keep them in mind.
```

---
## \#12 Posted by: luv2sk8te17 Posted at: 2018-09-26T14:18:29.503Z Reads: 175

```
It's actually 10s. The ones in the middle are single not double stacked. Hard to tell but true lol
```

---
## \#13 Posted by: chrischo1996 Posted at: 2018-09-26T14:19:43.442Z Reads: 173

```
Well damn... Wish me luck, I'll pray my helmet keeps me alive during testing.
```

---
## \#14 Posted by: chrischo1996 Posted at: 2018-09-27T05:41:21.035Z Reads: 167

```
I tried everything you said but still can't get them to connect over canbus. Any other tips?
```

---
## \#15 Posted by: luv2sk8te17 Posted at: 2018-09-27T12:19:38.952Z Reads: 163

```
Are you referring to “send through canbus” button or app in vesc tool? Or you can’t get both of them to work simultaneously?
```

---
## \#16 Posted by: chrischo1996 Posted at: 2018-09-27T13:34:03.255Z Reads: 150

```
Both of them to work simultaneously. I contacted Flipsky and they said they are aware of the issue and will replace it if I send it back. More waiting for me I guess.
```

---
## \#17 Posted by: luv2sk8te17 Posted at: 2018-09-27T16:00:37.555Z Reads: 148

```
I had this issue as well a few times when messing with ppm setup, I had confused myself and the vesc on which one was master/slave and the only one I could name the master was the side with the receiver lead coming out. So just make sure you have tried them both as a master setup with opposite one being a slave. Otherwise something is probably wrong. If you try to setup ppm on both it messes it up. Only needs one.
```

---
## \#18 Posted by: chrischo1996 Posted at: 2018-09-27T16:33:04.527Z Reads: 143

```
Just to clarify, I have two single 4.20 Fsesc's, not a dual. I believe that may be the difference between them, and why mine is not working.
```

---
## \#19 Posted by: luv2sk8te17 Posted at: 2018-09-27T16:45:39.266Z Reads: 143

```
Ah I see. Well why not just use a servo y connection to split the signal to them?

https://www.electric-skateboard.builders/t/servo-y-connector-completely-powering-second-esc/7821
```

---
## \#20 Posted by: chrischo1996 Posted at: 2018-09-27T17:12:00.460Z Reads: 144

```
Threads like [this](https://www.electric-skateboard.builders/t/y-piece-or-canbus/26461/249) make it hard to make a solid decision, but based on the fact that I want data readings from the VESC's using the Flipsky bluetooth module, traction control, and that Benjamin Vedder himself doesn't recommend splitting the ppm, I'll try to go with the canbus route for now. We'll see what Flipsky has to say about their return policy though, price to ship it back to them is around $100 and it better be coming out of their pocket not mine.
```

---
## \#21 Posted by: luv2sk8te17 Posted at: 2018-09-27T17:15:57.434Z Reads: 133

```
$100 shipping? WTF!!! I'm guessing your express shipping it? If it's going back would you think about asking for the dual as a replacement? It seems it would be easier to manage for programming.,,,maybe not I don't about doing two separate ones. Sorry your having bad luck.
```

---
## \#22 Posted by: chrischo1996 Posted at: 2018-09-27T18:12:03.443Z Reads: 127

```
I might try to ask for the dual, it's sleepy time over there in China so no response yet. Does the dual also require a canbus connector, or is it integrated? Thanks for the help
```

---
## \#23 Posted by: brenternet Posted at: 2018-09-27T18:25:53.968Z Reads: 122

```
Integrated.
```

---
## \#24 Posted by: gaetjen Posted at: 2018-09-27T20:11:06.343Z Reads: 121

```
I talked with them about that problem for a couple of days. I did send them videos of me setting everything up. But, even with their ideas I couldn´t get them to work in dual. I shipped both back. I paid 20 Euros from Germany to China tracked. They refunded the money even before the item arrived, so that I could buy the 6.6 dual during the flash sale.
```

---
## \#25 Posted by: chrischo1996 Posted at: 2018-09-27T20:39:21.058Z Reads: 119

```
Did they refund the shipping cost as well?
```

---
## \#26 Posted by: gaetjen Posted at: 2018-09-27T20:50:45.603Z Reads: 122

```
Yeah up to 20$
```

---

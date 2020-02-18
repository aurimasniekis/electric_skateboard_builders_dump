# Winning remote - battery

### Replies: 34 Views: 2383

## \#1 Posted by: Nordle Posted at: 2016-08-25T17:20:36.287Z Reads: 215

```
I recently got my first one and i really like it, but the battery feels a bit low. I went out for an hour or so yesterday (fully charged) went home and turn my remote off. But when i wanted to go out again today my battery was empty. Do i really have to charge this remote everyday? Do you know the capacity of the battery cause i really want to do an upgrade.
cheers
```

---
## \#2 Posted by: Raf Posted at: 2016-08-25T17:21:47.395Z Reads: 212

```
be careful with that remote at low battery. its been known to throw people off their boards
```

---
## \#3 Posted by: Jinra Posted at: 2016-08-25T17:21:53.295Z Reads: 209

```
My battery lasted for at least 3-4 days (8 mile ride each day). I might've gone longer but I ended up charging it. There may be something wrong with the remote.

@Raf I'm not convinced this is the cause of the signal issue. I've had weird issues even on higher charge.
```

---
## \#4 Posted by: Raf Posted at: 2016-08-25T17:23:25.635Z Reads: 202

```
ahh okay, I've just read a lot of people saying when it gets low the signal isn't as strong and can cut off
```

---
## \#5 Posted by: Nordle Posted at: 2016-08-25T17:26:57.003Z Reads: 189

```
@raf thanks but i really don't need such tips :D i set my remote up in the right way, dropout leads to freewheel no braking or accelerating, it's done and tested by myself so don't worry. **really just want to discuss the battery here**

maybe i just got one with a bad battery, if @jinra's lasts that long
```

---
## \#6 Posted by: Raf Posted at: 2016-08-25T17:28:49.715Z Reads: 183

```
no worries, was just a heads up incase you didn't know. as for your battery, the actual battery might be the problem. maybe buy a replacement and see if thats still a problem
```

---
## \#7 Posted by: ajaynagra Posted at: 2016-08-25T17:30:24.490Z Reads: 178

```
[quote="Nordle, post:5, topic:8317"]
@raf thanks but i really don't need such tips :smiley: i set my remote up in the right way, dropout leads to freewheel no braking or accelerating, it's done and tested by myself so don't worry. really just want to discuss the battery here
[/quote]

Maybe get a replacement battery just in case
```

---
## \#8 Posted by: Nordle Posted at: 2016-08-25T17:32:09.251Z Reads: 163

```
i think i'll do that.
some one knows the capacity of this one? anyways i'll get the biggest i can fit^^ my previous had 2 NCR.GA's upgrade and i never ever charged it :D but can't fit them in this one
```

---
## \#9 Posted by: Jinra Posted at: 2016-08-25T17:33:09.210Z Reads: 162

```
500mah

10 chars
```

---
## \#10 Posted by: Pantologist Posted at: 2016-08-25T17:48:06.882Z Reads: 162

```
The battery could just be garbage. It's a non branded cell.

This looks like the exact one 

https://www.adafruit.com/products/1578?gclid=CjwKEAjwrvq9BRD5gLyrufTqg0YSJACcuF81PcSD9COLTLHYPWeXs1zzcOoPrRWvZj7q5tbqYTHdzBoCSBTw_wcB
```

---
## \#11 Posted by: mccloed Posted at: 2016-08-25T17:58:06.117Z Reads: 163

```
I have one that doesn't last, also. I put a larger battery in it and it still does not hold the charge for that long. I think we both have semi-defective ones. Something is using the battery even when it's off. I just charge mine before I need to use it.
```

---
## \#12 Posted by: Nordle Posted at: 2016-08-25T18:01:46.760Z Reads: 174

```
did you try to modify so that the switch turns off gnd from battery? could help if some parasitic drain is the reason
```

---
## \#13 Posted by: longhairedboy Posted at: 2016-08-25T18:14:58.193Z Reads: 176

```
make sure the binding is good on those Winnings guys. Jason sent me these instrux because i kept streeting my face on a repair and could not figure out what the deal was. It turned out to be the remote binding and something they call "fail-safe functionality." Beleive me, without it, it fails very unsafe.  

> Please test the fail-safe functionality (like moving the transmitter as far away from the board and checking if the motor shuts down if out of reach). If the motors doesn’t shut down or applies brakes, please perform the following steps for binding and calibrating:

> Check and make sure all the wires are connected and that the REMOTE is OFF. Insert the bind plug into CH3(Bind) on the RECEIVER.

> With the REMOTE OFF: switch on the ESC to power up the RECEIVER, the red LED light will flash.

> PRESS and HOLD the bind button on the REMOTE and then turn the REMOTE ON.

> You should notice the REMOTE and RECEIVER LED light go from flashing red to solid red.

> Once you see a solid red light, the binding process is complete. Then without turning the REMOTE OFF or touching the THROTTLE pull the bind plug out (for the receiver to record the throttle mid point, neutral, to engage the fail safe)

> Then you can test it again by turning OFF the REMOTE and the RECEIVER LED should flash. By turning the REMOTE ON the RECEIVER LED should go back to solid red.

> Before riding, it's better to test the fail safe functionality again. Leave the board powered on and switch the REMOTE off: if the motor isn’t moving, the fail safe function is working, if the motor is moving fast or abruptly braking while throttle is applied: you have to repeat step No.1- No.6
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-25T18:46:20.633Z Reads: 157

```
I've made sure binding was fine on mine, but still continued to have problems. There was definitely something not working 100% right with the remote. 99% of the time everything was fine but occasionally my brakes wouldn't work or my throttle would get stuck acceleration for 2~ seconds; enough time to make me a bit nervous. After that it would intermittently respond/not respond for 5-10 seconds or until I restarted.

I noticed it happened consistently after getting off my train, so perhaps it's more prone to external interference.

After switching to the benchwheel remote, I've yet to run into any signal related issues.
```

---
## \#15 Posted by: longhairedboy Posted at: 2016-08-25T18:57:32.594Z Reads: 146

```
i'm willing to bet this is what jason is resolving with his new remotes. Other than the same-channel issue, which really isn't an issue as it seems like a no brainer in hind sight, I'm happy with the steezes. Two things i don't like about them though is the price and the way they don't fit in a pocket very well.
```

---
## \#16 Posted by: Pantologist Posted at: 2016-08-25T20:35:16.287Z Reads: 133

```
@Jinra You think if we had a add a capacitor it will help with connection uses? Couldn't hurt I guess...

A small capacitor could easily fit across the battery terminals.
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-25T20:37:56.811Z Reads: 129

```
I'm no electrical engineer so I couldn't tell ya. Somehow, I think it'd be more complicated than that though.
```

---
## \#18 Posted by: Nordle Posted at: 2016-08-25T20:58:49.246Z Reads: 126

```
[quote="Nordle, post:5, topic:8317"]
really just want to discuss the battery here
[/quote]

thank you :pray:
```

---
## \#19 Posted by: Michaelinvegas Posted at: 2016-08-25T21:02:12.193Z Reads: 125

```
I have two

One def last for days the other one day
```

---
## \#20 Posted by: Nordle Posted at: 2016-08-25T21:02:57.081Z Reads: 128

```
[quote="Jinra, post:14, topic:8317, full:true"]
I've made sure binding was fine on mine, but still continued to have problems. There was definitely something not working 100% right with the remote. 99% of the time everything was fine but occasionally my brakes wouldn't work or my throttle would get stuck acceleration for 2~ seconds; enough time to make me a bit nervous. After that it would intermittently respond/not respond for 5-10 seconds or until I restarted.

I noticed it happened consistently after getting off my train, so perhaps it's more prone to external interference.

After switching to the benchwheel remote, I've yet to run into any signal related issues.
[/quote]

an better antenna could help maybe, the one in the winning remote looks very poor
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-25T21:07:07.108Z Reads: 112

```
All winning remotes have PCB antennas. I attached an extension myself. I highly doubt it's a signal reception issue.
```

---
## \#22 Posted by: TarzanHBK Posted at: 2016-08-25T21:23:38.838Z Reads: 114

```
same problem here. battery is empty after 1,5h ride. charging to full till the green light flashes and leave it there for 2 days and you´ll have to recharge again. so something is draining juice out of that thing. its still pretty low that it only lasts for 1,5h ride...
```

---
## \#23 Posted by: Mikenopolis Posted at: 2016-08-25T21:36:42.984Z Reads: 116

```
after reading all this I really scared. I just went out to the car where my board is and tested my winning remote (without being on the board). I turned the board and remote on, pushed half throttle and turned off the remote. the motor went on for  half and second then stopped. I turned the wheel with my hands and it was "locked up" as if I was holding the brake, turning the board off freed up the wheel.

I'm assuming this is not normal? I'm too chicken$hit to do this test while being on the board. What is that new remote @onloop is planning to sell? I really don't want a RC car remote
```

---
## \#24 Posted by: Jinra Posted at: 2016-08-25T21:46:15.447Z Reads: 112

```
You sure ya'll aren't switching the channel switch instead of the power switch on the bottom? :smile:

@Mikenopolis sounds like you have to re-bind for receiver record neutral. If you ever touch the trim screw, you have to rebind.
```

---
## \#25 Posted by: Mikenopolis Posted at: 2016-08-25T21:51:31.712Z Reads: 113

```
I did adjust the trim screw =( 

So what SHOULD happen when I turn off the remote while the motor is running? free coasting wheel right?
```

---
## \#26 Posted by: Nordle Posted at: 2016-08-25T21:58:01.088Z Reads: 111

```
you simply should look in the other thread
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-25T22:06:11.585Z Reads: 113

```
Yes, you should free coast in neutral if you run current on control on the VESC, or a hobby ESC.
```

---
## \#28 Posted by: TarzanHBK Posted at: 2016-08-26T12:20:01.146Z Reads: 104

```
when battery is low it start stuttering or going wildly forward, backward, brake.. when you turn off, it goes into neutral and you don´t have any problem - free coasting. if you turn the winning remote back on, it starts again doing random things. so i just shut it down and start pushing back home :smiley:
```

---
## \#29 Posted by: Pantologist Posted at: 2016-08-26T15:39:52.584Z Reads: 97

```
Here are some pics of the opened remote.

The little square pattern radio trace thing on the PCB can be extended. @Jinra did that.

<img src="/uploads/db1493/original/2X/3/3a0278ffda178ad276505c0936ad840a197924ac.jpg" width="690" height="388">

At the battery terminals "BAT" I was thinking of just adding a capacitor to help out. This PCB seems to have none. 
<img src="/uploads/db1493/original/2X/9/9f464b618e179ff15921a3acf0b8336ba7c40238.jpg" width="281" height="500">
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-26T16:26:25.423Z Reads: 94

```
keep us posted!
```

---
## \#31 Posted by: Mikenopolis Posted at: 2016-08-26T16:38:20.593Z Reads: 89

```
How would adding a capacitor help out? Sorry I know very little except that capacitor is like a rechargeable battery
```

---
## \#32 Posted by: Nordle Posted at: 2016-08-26T16:43:00.811Z Reads: 91

```
in this case i also can't immagine how it could help
antenna extension is a good idea
```

---
## \#33 Posted by: Jinra Posted at: 2016-08-26T16:52:07.602Z Reads: 92

```
It's been done, hasn't helped or changed anything.

http://www.electric-skateboard.builders/t/2-4ghz-nano-remote-in-stock-30-pcs-usa-50-free-priority-shipping-international-45-shipping/5017/229?u=jinra
```

---
## \#34 Posted by: dinodave Posted at: 2016-09-02T07:34:50.192Z Reads: 79

```
I've had this remote for a few days now. After about half an hour of use I thought it was probably time to give it a quick charge, so I plugged it in, and it's a green light. Huh.

The instructions say 'when the charging indicator turn to red, it shows charging, turn to green, it means fully charged'.

So, I thought I would check the actual voltage of the cell, by disassembling the remote and measuring it with a multimeter. It was just under 4v, it should be 4.2v when fully charged. So I left it plugged in for a while, with the green light displaying. Sure enough the voltage went up, and then eventually the light turned red.

So on my remote at least, it is green light when charging, red when fully charged. Just thought I should post that in case it might be confusing anyone else!
```

---

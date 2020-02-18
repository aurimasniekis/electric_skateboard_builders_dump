# Recommendation for adding hall sensors to motor

### Replies: 14 Views: 2572

## \#1 Posted by: Hummie Posted at: 2016-11-16T20:20:44.237Z Reads: 268

```
I've never bothered before as the vesc FOC program is so nice but none-the-less people want me to add them to their motor.  any suggestions?  its a 47mm diameter stator which is rare.
```

---
## \#2 Posted by: TheCheat Posted at: 2016-11-16T20:35:20.118Z Reads: 264

```
If we're talking from the ground up, the easiest way is to mount the hall sensors on a PCB and then internally mounting the pcb on top of the stator. Of course hot glue is the preferred dirty fix for those unwilling to use PCBs.
```

---
## \#3 Posted by: Monte Posted at: 2016-11-16T20:49:55.028Z Reads: 259

```
The Hot Glue King says DO IT!
```

---
## \#4 Posted by: Monte Posted at: 2016-11-16T20:50:08.547Z Reads: 253

```
Where can i buy hall sensors?
```

---
## \#5 Posted by: Hummie Posted at: 2016-11-16T21:03:57.484Z Reads: 235

```
hot glue sounds risky   there's high heat epoxy I have labeled for such a job.  I'm also looking where to buy them.  they're out there but not sure which is best suited.  
 It seems mounting them is pretty straight forward and they just have to be positioned correctly: able to pick up the magnet's field but not close to to any stray fields.
```

---
## \#6 Posted by: chinzw Posted at: 2016-11-17T00:35:51.776Z Reads: 219

```
I believe PCB mounted sensor would be best, you can buy the sensors from digikey/mouser, unless you're after premade sensor pcbs?
```

---
## \#7 Posted by: TheCheat Posted at: 2016-11-17T01:29:28.646Z Reads: 218

```
I said quick and dirty , never said reliable :wink:. Here's a link of a guy going the whole 9 yards. Math and BOM included... 
 http://makeatronics.blogspot.com/2014/05/bldc-hall-effect-sensors.html?m=1

P. S. looks like he even used a 48mm motor!
```

---
## \#8 Posted by: Jinra Posted at: 2016-11-17T01:29:59.284Z Reads: 208

```
make sure you use jst-ph 2mm headers if you want it to easily plug into the vesc. I haven't seen a single vendor who uses them by default yet
```

---
## \#9 Posted by: mccloed Posted at: 2016-11-17T04:49:04.355Z Reads: 199

```
I have added sensors to a lot of motors. I usually shave a little out between the stators to fit the sensors in between. Then they are epoxied in. Sensored FOC is the best!
```

---
## \#10 Posted by: Hummie Posted at: 2016-11-17T05:17:29.462Z Reads: 197

```
@mccloed I thought I had the best wth foc! What's great about w sensors?  . Thanks for your help all. I'll be doing it. And excited to see how it rides and hear the sounds. I imagine the take off from still.  I guess that's nice but in the interest of saving battery I push a bit from still. Isn't it some extreme force needed to go from 0 to 3 or something. I'm more interested in the sounds I think because I like to push once regardless I think.
```

---
## \#11 Posted by: mccloed Posted at: 2016-11-17T05:33:51.140Z Reads: 192

```
Ha. I still push, also. I would still get slight hesitation without sensors from a stop. With the sensors, no hesitation and a silent smooth start. Haven't tried on hubs, yet.
```

---
## \#12 Posted by: SageTX Posted at: 2017-01-02T02:01:45.446Z Reads: 161

```
I have the sensored 6354 190kv motors from @JLabs group buy. Any idea of the order of the wires? I have the jst plugs, just can't get the wiring right I guess.  I cant get the motor detection to successfully read the sensors.
```

---
## \#13 Posted by: Jinra Posted at: 2017-01-04T15:57:44.828Z Reads: 151

```
black = gnd, white = temp, red = 5v, other three are sensors.
```

---
## \#14 Posted by: alindaniel93 Posted at: 2017-04-04T07:37:08.089Z Reads: 124

```
http://alienpowersystem.com/shop/brushless-motors/50mm/internal-pcb-with-hall-effect-sensors-120-degree/
here you go :+1:
```

---

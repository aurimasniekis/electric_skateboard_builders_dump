# Motor sensor plug doesn&rsquo;t fit on VESC..*SOLVED*

### Replies: 36 Views: 5936

## \#1 Posted by: flywithgriff Posted at: 2017-05-13T20:17:41.897Z Reads: 533

```
I am putting together my new build and have purchased a sensored motor. However, the plug on the sensor wire does not match a socket on my vesc. The motor came with an additional wiring harness and a socket. Do I just need to cut and solder on the new plug?

<img src="/uploads/db1493/original/3X/d/9/d9642ae18fa3ea748e5f8a7ca7e43ced964a8314.JPG" width="375" height="500">
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-13T20:20:44.835Z Reads: 513

```
Upload some pics of the adapters and plugs. Maytech makes a plug and play adapter if that's what you have.

Edit: is there a female end on the adapter?
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-05-13T20:22:05.993Z Reads: 512

```
The pic is what I have. The smaller is attached to the motor. The larger has 2" wires attached to it and are also a gauge or two larger.
```

---
## \#4 Posted by: JLabs Posted at: 2017-05-13T20:23:57.933Z Reads: 518

```
I don't have a VESC in front of me but I think the sensor port is 7 pins. 

If that connector fits the sensors port then yes, you can just cut the wires from you motor and solder to the wires of you adapter.

Check out @Jinra's tutorial 
https://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760/36
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-13T20:36:27.104Z Reads: 505

```
6 pins!

black = GND
red = 5v
white = temp
the other 3 = hall sensors

The VESC lays out sensor wires differently than how typical chinese motors come. Make sure your red, black, and white cables are in the right positions.
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-05-13T20:39:07.603Z Reads: 494

```
Does this layout look right coming out of the vesc? Just match colors with wiring the two together?

<img src="/uploads/db1493/original/3X/4/5/4576ce9de367fad5170fbe4d97224b1b7a252439.JPG" width="375" height="500">
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-13T20:41:08.924Z Reads: 481

```
Yep, unless the motor mfg decided to not follow typical electronics convention for whatever reason. Black, red, and white are standard. The sensors can be varying colors though.
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-05-13T20:43:04.979Z Reads: 475

```
I notice the colors in the connectors coming out the vesc are different for our connections. How do I know which order to wire in?

Im running a 6374, 190kv from @Kaly
```

---
## \#9 Posted by: Smorto Posted at: 2017-05-13T20:55:39.434Z Reads: 468

```
diy-electric-skateboard-kits-parts/vesc-sensor-wires/
```

---
## \#10 Posted by: Jinra Posted at: 2017-05-13T21:01:49.653Z Reads: 456

```
Kaly's motors are plug and play with VESC according to his post, shouldn't have to change anything.
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-05-13T21:02:36.170Z Reads: 441

```
Nope, I just got this one from him and the small plug is what comes attached.
```

---
## \#12 Posted by: Jinra Posted at: 2017-05-13T21:05:42.444Z Reads: 426

```
Then you'll have to take out the leads on the VESC plug and put Kaly's in. However they may not fit in which cause just solder the VESC plug leads into the motor, the colors seem to match on the pic you have.
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-05-13T21:08:55.449Z Reads: 421

```
Ok great, That's exactly what I am doing now. However, the color order in your photo for the vesc wiring does not match the color order on the plug that came extra with my motor that does for the vesc. So I need to rearrange the pins in my plug to make sure the plug into the correct pin in the connector on the vesc?
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-13T21:11:57.052Z Reads: 409

```
Yep just reorder to it match the colors. Like I said, red/black/white are critical to be in the right position, but the others dont matter as long as they're going in the hall pins.
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-05-13T21:43:24.169Z Reads: 411

```
Problem solved. Thanks guys!

<img src="/uploads/db1493/original/3X/4/5/4579ac875c1108277cbbec7b44fe17239fe7d61d.jpg" width="375" height="500">
```

---
## \#16 Posted by: Redfire1 Posted at: 2018-04-13T23:18:17.736Z Reads: 274

```
@Jinra I need a bit of help please,bout these motor for my vesc,the motor came with sensor connector but the are 5pin so I just ordered 6pin jst to used to connect but there will be one wire missing can you tell me how is it possible someone said leave the temp wire but I am new don’t know which one it is ![image|230x500](upload://eQqJ1ifraMalnH6PbeHneNnQFkG.jpg)![image|230x500](upload://7L3hP7FUgUJjsTsJAxZcM7gKRWi.jpg)![image|375x500](upload://6D7pbChsUFwpPcAb8jL3DMVOmoT.jpeg)
```

---
## \#17 Posted by: pat.speed Posted at: 2018-04-13T23:30:27.467Z Reads: 254

```
If you read @Jinra’s post he says temp is the white wire. Now look at @flywithgrif’s pic which pin is the white wire connected to. That should be correct as long as the motor manufacturer used the right pattern
```

---
## \#18 Posted by: Jinra Posted at: 2018-04-14T00:31:13.778Z Reads: 248

```
if you only face 5 pins it's fairly simple. black is ground, red is 5v and the rest are hall sensors
```

---
## \#19 Posted by: Redfire1 Posted at: 2018-04-14T05:32:06.536Z Reads: 243

```
In my case here black - red + and the orange would be temp so I would leave that one out ![image|690x425](upload://3ozsJGSV22YRm1vwf6ZhRirUNhX.jpeg)![image|375x500](upload://gh7YwPEYBtvARXwHhaw1T6GhBv3.jpeg)
```

---
## \#20 Posted by: Redfire1 Posted at: 2018-04-14T05:33:02.302Z Reads: 256

```
![image|375x500](upload://eO4tA5P6L4w8CLVabjziJRgXGUu.jpeg)
```

---
## \#21 Posted by: EvanWhy Posted at: 2018-09-09T07:39:41.936Z Reads: 183

```
Hi everyone, I just recently purchased a vesc from mboards and a torque boards 6355 260 kv motor. I was able to make an adapter to connect the bullet connectors but I am unsure how to wire the jst connector to my vesc since it is too small. The connector on my motor is a 6 pin.


![20180909_003717|281x500](upload://te0J1oQzpfUx3R6XJq5rMApcasF.jpg)![20180909_003721|281x500](upload://9F4JQYbsrFUcoDSt14ZZFiuXUu7.jpg)![20180909_003711|281x500](upload://wL4Mpt4KCVJDye8ejIRySloDftI.jpg)
```

---
## \#22 Posted by: EvanWhy Posted at: 2018-09-09T07:41:04.580Z Reads: 172

```
I was wondering if I need to by a different connector and solder it to the motor wires so that it fits with the VESC.
```

---
## \#23 Posted by: Andy87 Posted at: 2018-09-09T07:49:17.228Z Reads: 169

```
Get 2mm jst plugs and pins.
Cut the wires, crimp new pins and plug it in.
Ready to go.
If your sensor cables to short than just solder some 2mm jst extension on and good
```

---
## \#24 Posted by: EvanWhy Posted at: 2018-09-09T07:57:10.954Z Reads: 167

```
Are these the 2mm jst connectors you are talking about?
https://www.amazon.com/2-Pin-JST-XH-Balance-Connector-Adapter/dp/B00R1J91JY
```

---
## \#25 Posted by: EvanWhy Posted at: 2018-09-09T08:00:50.672Z Reads: 165

```
Or is it these 6 pin 2mm jst connectors.

https://www.amazon.com/2-0MM-Female-Single-Connector-Wires/dp/B01IZWYK7I
```

---
## \#26 Posted by: Andy87 Posted at: 2018-09-09T08:00:58.370Z Reads: 161

```
If you don’t want to make anything you can get some of them
https://eskating.eu/product/sensors-adapter-jst-2-0mm-6-pins/

If no than you need that one you choose but with 6pins not with 2
```

---
## \#27 Posted by: Andy87 Posted at: 2018-09-09T08:02:26.708Z Reads: 155

```
Looks good
```

---
## \#28 Posted by: EvanWhy Posted at: 2018-09-09T08:02:26.925Z Reads: 149

```
ahh I see thank you for your help. Is there any certain order I need to connect them in because the vesc didn't have any sort of instruction
```

---
## \#29 Posted by: Andy87 Posted at: 2018-09-09T08:04:22.323Z Reads: 142

```
On the back side of your vesc there should be written which pin is what.
Don’t mix + and - (red and black or better to say first and last pin)
Sensor wires don’t mind which place they are
```

---
## \#30 Posted by: EvanWhy Posted at: 2018-09-09T08:06:34.685Z Reads: 141

```
on the backside I see a 5v temp h1 h2 h3 and a gnd pin
```

---
## \#31 Posted by: Redfire1 Posted at: 2018-09-09T08:07:26.147Z Reads: 141

```
Normally you would get a adopter with it,if there is none,like I did buy a bigger jst connector and weld the wires ![image|230x500](upload://v5ofwHSo3bfPOizs7XTKCTFW4eZ.jpeg)![image|230x500](upload://3vuvVZ7AGv2sdtfDYN6v87bZp1S.jpeg)![image|230x500](upload://rTny6auwSn7XKDTFdnoJQQc3fWC.jpeg)![image|381x500](upload://3iwpKuugd6n00wbKgvQfaYFTUh1.jpeg)![image|354x500](upload://6i0Tp3KZChoU3BSBsWxshgOb5rG.jpeg)
```

---
## \#32 Posted by: Andy87 Posted at: 2018-09-09T08:08:02.247Z Reads: 128

```
That’s it.
Red is 5V black is ground.
```

---
## \#33 Posted by: EvanWhy Posted at: 2018-09-09T08:12:14.595Z Reads: 129

```
alright thanks andy, and so I just need to get the positive and negative in the right spot and the rest don't matter where they connect correct?
```

---
## \#34 Posted by: Andy87 Posted at: 2018-09-09T08:15:13.730Z Reads: 127

```
That‘s correct!
The sensors itself can be on any position on the plug as long as it’s not the plus or the ground.

To be not confused, the cable color from your torque board motors should have the right order already. The red 5V the black is ground.

If you have any other issues just let us know 😉
```

---
## \#35 Posted by: Josh2 Posted at: 2019-02-04T06:04:36.759Z Reads: 91

```
@Jinra Hi i have the same problem @Redfire1 had in that my sensor wire on my motor only has 5 pins and my vesc needs 6. How exactlt do i plug it into the vesc?
```

---
## \#36 Posted by: Redfire1 Posted at: 2019-02-04T06:28:28.183Z Reads: 88

```
On the Vesc look on the other side it should say 5v+, GN- ,temp hall etc,you don’t need the temp connection,try get a wiring diagram for you motor find the +and - and connect them the rest don’t really matter how you connect them,that’s what I did and it work.![image|230x500](upload://3vuvVZ7AGv2sdtfDYN6v87bZp1S.jpeg) ![image|230x500](upload://rTny6auwSn7XKDTFdnoJQQc3fWC.jpeg) ![image|381x500](upload://3iwpKuugd6n00wbKgvQfaYFTUh1.jpeg) ![image|354x500](upload://6i0Tp3KZChoU3BSBsWxshgOb5rG.jpeg)
```

---

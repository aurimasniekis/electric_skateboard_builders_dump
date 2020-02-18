# When I squeze the trigger the motor wont turn!

### Replies: 37 Views: 1518

## \#1 Posted by: dino15309 Posted at: 2017-05-19T23:12:16.200Z Reads: 78

```
Hello Everyone!
I have the Quanum pistol grip remote/ receiver and when I pull the trigger, nothing happens.
I am using DIY Electric's VESC and I have checked all the settings and nothing seems to be wrong. The radio/receiver are connected properly but the motor won't turn. The motor works (I have seen it using the arrow keys) but the throttle does not work.

Please help me! :cold_sweat: It is for a school project! :snowboarder:
```

---
## \#2 Posted by: dino15309 Posted at: 2017-05-19T23:16:07.172Z Reads: 76

```
Just a quick update, I have torn apart my remote as someone did in this linked thread but everything seems fine :cry:
Please help  :fearful:

Link to thread: https://www.electric-skateboard.builders/t/motor-wont-turn-when-i-turn-on-remote/6946
```

---
## \#3 Posted by: SageTX Posted at: 2017-05-19T23:23:26.626Z Reads: 74

```
Check on your ppm tab watt control (or current control) is enabled. Also be sure to check ppm pulsewidth settings.  
See here....

https://www.electric-skateboard.builders/t/snagglepuss-rebuild-to-arbor-highground-dual-6354-dual-ollin-vescs-mini-remote-dual-diyv4-mounts-diy-13-36-8s3p-9ah-zippys-44d-caliber-iis-97mm-abec11-78a-flywheels-kydex-box-enclosure/14482/20?u=sagetx
```

---
## \#4 Posted by: dino15309 Posted at: 2017-05-20T00:20:44.125Z Reads: 65

```
<img src="/uploads/db1493/original/3X/c/0/c034f96281fffceef1f255d487ae523ca1e3ed92.PNG" width="690" height="365">

So I did what the instructions told me but when I pulled the trigger to test stuff, nothing happens?
```

---
## \#5 Posted by: dino15309 Posted at: 2017-05-20T01:02:17.291Z Reads: 54

```
Okay, I did some further testing and I got scarry, almost expensive results...
When I press the "CH3" button on the side of the remote, the motor jumps and spins the wrong part of the motor.

Another thing was that I received diferent readings between channel 3 and 2/1
3 - about 1.4MS
2/1 - about 50.3MS

I nearly just broke everything so I REALY need some help :scream::scream::scream::scream:
```

---
## \#6 Posted by: mmaner Posted at: 2017-05-20T01:06:45.135Z Reads: 52

```
Sounds like you have the wrong channel from the RX to the VESC, trying connecting the VESC to ch3.
```

---
## \#7 Posted by: dino15309 Posted at: 2017-05-20T01:08:12.046Z Reads: 50

```
I did and it didn't work. I did find the instruction manual:
```

---
## \#8 Posted by: dino15309 Posted at: 2017-05-20T01:09:13.653Z Reads: 50

```
<img src="/uploads/db1493/original/3X/3/2/32d7430cb37f33ffb804eed0e28fefd5bb7b2272.PNG" width="537" height="500">
```

---
## \#9 Posted by: dino15309 Posted at: 2017-05-20T01:18:41.696Z Reads: 49

```
So, when I press the alleged "start button" on channel 3, the entire thing flips and twists and I am scared to re-assemble my rig.

I am 14 and I'm lost!!!
```

---
## \#10 Posted by: Titoxd10001 Posted at: 2017-05-20T01:21:07.097Z Reads: 48

```
On ppm tab make sure it's "disabled" for now and write configuration. Your servo wire should be on channel 2, is that what you had it at originally?
```

---
## \#11 Posted by: dino15309 Posted at: 2017-05-20T01:21:46.917Z Reads: 47

```
no it was on 3
```

---
## \#12 Posted by: Titoxd10001 Posted at: 2017-05-20T01:23:29.123Z Reads: 45

```
Change it to channel two. You should be on "disabled" and write configuration so nothing spins up.
```

---
## \#13 Posted by: dino15309 Posted at: 2017-05-20T01:23:43.971Z Reads: 43

```
Okay, now what? should I attempt to use the motor?
```

---
## \#14 Posted by: Titoxd10001 Posted at: 2017-05-20T01:24:48.975Z Reads: 41

```
No. When display box is checked. Is the green bar in the center 50%
```

---
## \#15 Posted by: dino15309 Posted at: 2017-05-20T01:25:17.292Z Reads: 44

```
It fluctuates at 53/54
```

---
## \#16 Posted by: Titoxd10001 Posted at: 2017-05-20T01:30:53.392Z Reads: 42

```
That's a good sign better than it was before. You can set it so it's exactly 50% on throttle trim later and change failsafe later also. 

Now with "disabled" mode. You can pull throttle and it should be close to or exactly 100% at max. Motor should not spin at the moment. Test it like that
```

---
## \#17 Posted by: dino15309 Posted at: 2017-05-20T01:31:45.142Z Reads: 41

```
it goes up to 100 and down to 14 and sometimes 13
```

---
## \#18 Posted by: Titoxd10001 Posted at: 2017-05-20T01:34:01.951Z Reads: 43

```
As long as you hold it, it stays at a hundred right? Do the same for brake/reverse to see that you get 0%.
```

---
## \#19 Posted by: dino15309 Posted at: 2017-05-20T01:35:26.864Z Reads: 47

```
full throttle is 100, full brake is 14 and maybe 13, rest is 53/54
how can I adjust my settings?
```

---
## \#20 Posted by: Titoxd10001 Posted at: 2017-05-20T01:44:04.672Z Reads: 47

```
To change the center you can change your throttle trim on your remote. To get 0% you change the minimum pulsewidth. If you change one thing the other changes. If you download @ackmaniac firmware you can change the center pulsewidth. You want the values to be as close to 0% 50% 100% as possible, but the most important you want it to be 50% when you turn off control. 

Test to see what the value is when you turn off control
```

---
## \#21 Posted by: dino15309 Posted at: 2017-05-20T01:52:15.543Z Reads: 40

```
Okay, i changed the settings on my VESC and controller and now it is 3% low, 50% mid, and 100% full. What next?
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-05-20T01:54:48.282Z Reads: 38

```
What happens when you turn off remote? What %
```

---
## \#23 Posted by: dino15309 Posted at: 2017-05-20T01:56:03.696Z Reads: 36

```
37% in total (I am now just getting those 10 chars)
```

---
## \#24 Posted by: Titoxd10001 Posted at: 2017-05-20T02:01:31.283Z Reads: 36

```
When the remote is turned off is the most important value. If connection is lost that's the value it will go to (brakes in this case). 

You need to set failsafe. Sometimes there is a button on the receiver that says "failsafe" that you press. If not the procedure might be to rebind so failsafe is set to 50% (netruel when connection is lost)
```

---
## \#25 Posted by: dino15309 Posted at: 2017-05-20T02:05:45.156Z Reads: 35

```
I rebound but it still goes to 37%
```

---
## \#26 Posted by: Titoxd10001 Posted at: 2017-05-20T02:10:31.711Z Reads: 34

```
Is possible your remote has no failsafe, but I doubt it. Did you remove bind plug while power was still on till you got solid lights, then turn off receiver/board power and turn off control
```

---
## \#27 Posted by: dino15309 Posted at: 2017-05-20T02:15:04.789Z Reads: 34

```
I think i did everything you said but remove power from the board. Could you give me slighly more clear instructions please? I am not fully understanding... :confused:
```

---
## \#28 Posted by: Titoxd10001 Posted at: 2017-05-20T02:20:45.195Z Reads: 35

```
Not sure if its same for you but...

Everything off... Insert bind plug in bind slot of receiver.. power up the receiver/turn on board... Hold bind button on controller and turn on... Lights should go solid... Remove bind plug.. then turn off board.. then turn off controller... Turn on controller... Turn on board
```

---
## \#29 Posted by: dino15309 Posted at: 2017-05-20T02:25:35.540Z Reads: 35

```
did not work, but shouldn't the bord just brake at 37%?
it is not a very heavy brake so I should be alright... Correct?
```

---
## \#30 Posted by: Titoxd10001 Posted at: 2017-05-20T02:33:22.568Z Reads: 35

```
You should check online for your specific remote. I would not use it with no failsafe if you're accelerating and go straight to brake due to loss connection you can hurt yourself. You can test on on bench to see if everything is working. When riding say 5mph turn off remote to see how bad it is without failsafe. If doesn't have failsafe I would look at mini remote as possible alternative.
```

---
## \#31 Posted by: dino15309 Posted at: 2017-05-20T02:35:05.199Z Reads: 35

```
I have the Quanum pistol grip remote in case you know where to look...
```

---
## \#32 Posted by: dino15309 Posted at: 2017-05-20T02:39:47.067Z Reads: 31

```
[Failsafe](https://www.electric-skateboard.builders/t/fail-safe-device/8390/9)

This article says that the VESC should have it built in
```

---
## \#33 Posted by: mmaner Posted at: 2017-05-20T02:50:23.544Z Reads: 30

```
Quality assist, good on ya 😀
```

---
## \#34 Posted by: Titoxd10001 Posted at: 2017-05-20T03:03:12.543Z Reads: 31

```
From my understanding the vesc has failsafe if all power is lost to receiver. Remote has separate failsafe if just connection is lost. Try Google how to set failsafe+ your remote or YouTube video. Busy at the moment. It is possible remote has no failsafe because it is a budget remote. Remotes aren't​ to pricey if new one is needed
```

---
## \#35 Posted by: Titoxd10001 Posted at: 2017-05-20T03:03:55.410Z Reads: 31

```
Thanks. 10 char
```

---
## \#36 Posted by: Ackmaniac Posted at: 2017-05-20T10:46:15.506Z Reads: 28

```
On my remote you have to remove the bind plug while the board is till switched on. Just switch it on with the bind plug in it. Leave the remote and the board switched on and remove the bind plug. Then the receiver should know where your idle position is. If that doesn't work then you should trim your throttle with the potentiometer until it shows at idle the same pulsewidth as when it is switched off. 

The problem is that when your board brakes when it looses connection it will send you flying. Imagine you accelerate hard and lean forward and out of nowhere your board brakes. 
The failsafe at the vesc is there if it looses the connection to the receiver. Like when the cable gets loose or the receiver breaks.
```

---
## \#37 Posted by: dino15309 Posted at: 2017-05-20T12:39:02.982Z Reads: 26

```
So, I don't think that my remote has a potentiometer. It is a cheap remote that I could afford. I was wondering if I could program the VESC's failsafe to make up for this. If I lost connection to the remote, it resorts to 37%, braking enough to hurt me at high speeds. Is there a way to program this using the BLDC tool?
```

---

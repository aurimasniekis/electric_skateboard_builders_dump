# Selecting an ESC for Mountainboard

### Replies: 15 Views: 1507

## \#1 Posted by: ppolis Posted at: 2018-03-13T11:25:40.000Z Reads: 175

```
I'm a beginner looking to build my first ever board and am looking for some advice on selection of the ESC. I'm planning on building a mountainboard running somewhere from 8S to 12S. My intended setup so far is:
2 of these batteries in parallel and either 2 or 3 in series, so 8S2P or 12S2P,
https://hobbyking.com/en_us/zippy-flightmax-5000mah-4s1p-20c.html?___store=en_us
and these motors, which list their max current as 70A
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-245kv-brushless-outrunner-motor.html?___store=en_us
In most threads I've read asking for ESC recommendations, VESC is mentioned, and I understand that it has great benefits as far as fine tuning performance, but unless I misunderstand the specifications listed, it can only output 50A continuous. I assume this won't be enough to work with the above motor, or perhaps any mountainboard, but I very well may be wrong in that assumption. Assuming the VESC is out, I located these potential candidates:

The AeroStar should provide way more current and is quite inexpensive, but I can't find anyone else on here that says they've used one, which is concerning.
https://hobbyking.com/en_us/aerostar-advance-120a-esc-opto.html?___store=en_us

Trying to keep the price less than $200 each, I found the Phoenix Edge, a 8S 100A ESC:
http://www.castlecreations.com/en/phoenix-edge-100-esc-010-0100-00

And finally, the FVT 120A "Sleeping Lion" ESC, which at least a few people on here have mentioned using:
https://szfvt.en.alibaba.com/product/60449510282-802501949/Newarrival_brushless_DC_motor_electronic_skateboard_12S_HV_120A_ESC.html

So basically my question boils down to this: I'd love to use dual VESCs for this project, but is the 50A max going to be insufficient for a reasonably fast mountainboard, and if so, do any of those other ESCs look like good choices?

Thanks so much for any help!
```

---
## \#2 Posted by: telnoi Posted at: 2018-03-13T11:28:31.966Z Reads: 152

```
How fast do you want go go?
Hilly or flat area?
```

---
## \#3 Posted by: ppolis Posted at: 2018-03-13T11:32:16.460Z Reads: 154

```
Ideally I'm looking to go 15-20 on flat ground, and be able to take on hills one would encounter on something like a motocross track.
```

---
## \#4 Posted by: telnoi Posted at: 2018-03-13T12:10:41.101Z Reads: 149

```
I'm taking that's 20 mph (or 32 km/h).


* If you are thinking about motocross tracks, you want sensored motors as sensorless will result in cogging if you try to move from a stand still on an incline. 
* At 32 km/h, you don't need high KV motors. It only causes issues, one being hitting the RPM limit of 4.12 based VESCS. The other, lack of torque. With a gear ratio of 1:5, you'll go around 36 km/h on 10S with 8'' wheels at 149KV.
* Consider going with 6374 motors for more power
* no reason to stick with 4.12 based VESCs. 6.4 based VESCs are almost as inexpensive these days (https://www.electric-skateboard.builders/t/hw6-4-based-esc-b-box/44375). The hardcore riders here are happy with their performance

The above only applies to a VESC setup.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-03-13T12:21:53.222Z Reads: 133

```
Two options in my opinion:

1. 8s Setup with Hobbywing Ezrun Max 6 Escs - bomb proof and so much punch :slight_smile:
2. Vesc 6 or clone and 12s
```

---
## \#6 Posted by: Acido Posted at: 2018-03-13T12:43:03.937Z Reads: 127

```
With 50a continious you would draw all the power from the battery within minutes
```

---
## \#7 Posted by: jbalint1122 Posted at: 2018-03-13T19:56:13.062Z Reads: 112

```
Hey man, I might have a perfectly fine Sleeping Lion ESC in a week or so. If all goes well maybe I can sell you that for the price of the shipping from me to you. But be aware! You probably want to install a fan on that as it is overheating on my setup. 
If you're on a budget this might be a good option for you. (But there's a small chance that I won't be able to let it go, so don't get your hopes too high.) :slight_smile:
```

---
## \#8 Posted by: Acido Posted at: 2018-03-13T20:44:37.405Z Reads: 103

```
They are up to 6s right?
I have a board that needs only an esc
Its nothing special tho..
```

---
## \#9 Posted by: jbalint1122 Posted at: 2018-03-13T20:51:05.228Z Reads: 99

```
This is a 12S 120A esc. It means it probably workes with 6s too.
```

---
## \#10 Posted by: ppolis Posted at: 2018-03-14T00:04:42.806Z Reads: 98

```
@telnoi Thanks for the input. I'll be honest and say my motor choice was somewhat arbitrary, sounds like a good idea to tend to one with higher torque for my application. Are you saying that you'd recommend a VESC 6 and not a 4.12? Looking through your posts I see you've built a mountainboard with dual VESCs, did you encounter any trouble with the 50A limit?

@TarzanHBK I considered the Max 6, but from what I can tell, the three ESCs I found have more or less the same capabilities for cheaper. Is there something about that one that outdoes the others?

@jbalint1122 I'd definitely be interested in that Sleeping Lion if it ends up not working out for you. If you don't mind me asking, what was your setup and what kind of performance could you get out of it?

@Acido You're right, perhaps assuming 50A continuous draw is a little much. That being said, as a beginner I have a hard time estimating what my power needs are going to be. Do you have any idea what kind of current draw I should plan for on a board like the one I'm planing on making?

Thanks again guys!
```

---
## \#11 Posted by: telnoi Posted at: 2018-03-14T05:08:08.189Z Reads: 79

```
50 is enough for me, though some say it's only 30 before it starts throttling due to heat. My cruising speed is usually 35 km/h, off-road around 20. 

I only have one issue. Overheating after a long continuous off-road hill climb, but I have no airflow around my boxes and it's a hell of a climb. 

Someone like nowind would notice a difference between 4 and 6 in performance. He likes pulling wheelies and wants rocket acceleration/switched to roxxies due to the lack of vesc 4 performance. Those went down in flames, now he rides vesc 6.

Take a look at his vids. If that's what you want to achieve, vesc 6. Otherwise, 4 will do.
```

---
## \#12 Posted by: pat.speed Posted at: 2018-03-14T06:36:01.079Z Reads: 71

```
The reason the max 5/6 is better is because it is an Rc car esc. Helicopter or plane escs won’t work very well as they generally have no brakes. The max 5 also can do 200 amps!
```

---
## \#13 Posted by: electrickiwi Posted at: 2018-03-14T06:41:16.744Z Reads: 69

```
I am have a max 6 ESC. Rated up to 8s. That I ran a single drive 190kv on a longboard up to 47kmh the other day. Tons of torque and what nowind runs on some of his emtb builds. Basically bulletproof. If you want to buy just send me a message and we can sort something out
```

---
## \#14 Posted by: Jebe Posted at: 2018-03-14T06:54:03.634Z Reads: 64

```
+1 for the Hobbywing max 6
```

---
## \#15 Posted by: TarzanHBK Posted at: 2018-03-14T07:38:39.505Z Reads: 61

```
the sleeping lion is a hit or miss esc, which works for you if you are lucky - others just went up in flames. So a no for that one.

I don´t know the other ESCs but seems like Aero ESCs which are made to drive a helicopter or fly-thing without brakes or brakes that suck. So a no for these.

The Max 6 is bulletproof and tested by lots of folks, me included. I haven´t destroyed it so far and it already took some abuse trust me ;)

For nicer and more configurations take the Vesc 6 or clone.

There might be other options out there, but these are only for people who like to experiment a bit are are not afraid to burn some monies in my opionion
```

---

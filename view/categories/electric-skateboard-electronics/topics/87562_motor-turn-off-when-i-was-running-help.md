# Motor turn off when I was running &ldquo;help&rdquo;

### Replies: 11 Views: 243

## \#1 Posted by: pedro Posted at: 2019-03-18T21:22:32.893Z Reads: 61

```
Hello guys, how are you all?

I want know why my motor stop working when I’m climbing. Happens two times already…I was running, and suddenly the motor “turn off” I couldn’t control with my remote, i turn off and next turn on, my remote and nothing… I turn off the safty cutoff from my board and put it again and nothing… after a 2/3 min is start working :).

the second time it was the same thing…

I thing is when I climb in full power the board turn off, because I climb the same hill, but the second time I was running slower, and nothing happened.

Do you know How I can fix?


My bms is this: http://www.batterysupports.com/36v-37v-42v-10s-45a-10x-36v-lithium-ion-lipolymer-battery-bms-p-266.html

My battery is 2s10p https://eu.nkon.nl/rechargeable/18650-size/samsung-inr18650-20r-2303.html

Vesc

![|16x16](https://cdn-global-hk.hobbyking.com/media/favicon/websites/1/favicon_hk.png) [Hobbyking ](https://hobbyking.com/pt_pt/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html?___store=pt_pt)

![|565x414](https://cdn-global-hk.hobbyking.com/media/catalog/product/cache/9/image/9df78eab33525d08d6e5fb8d27136e95/1/8/189672.jpg)

### [Turnigy SK8-ESC V4.12 For Electric Skateboard Conversion w/BEC ](https://hobbyking.com/pt_pt/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html?___store=pt_pt)

VESC is an open source, highly modifiable electronic speed controller ESC by Benjamin Vedder. It is designed with DIY electric skateboard conversions in mind.

Motor

![|16x16](https://cdn-global-hk.hobbyking.com/media/favicon/websites/1/favicon_hk.png) [Hobbyking](https://hobbyking.com/pt_pt/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html?___store=pt_pt)

![|565x414](https://cdn-global-hk.hobbyking.com/media/catalog/product/cache/9/image/9df78eab33525d08d6e5fb8d27136e95/legacy/catalog/18175.jpg)

### [Turnigy Aerodrive SK3 - 5055-280kv Brushless Outrunner Motor](https://hobbyking.com/pt_pt/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html?___store=pt_pt)

Turnigy Aerodrive SK3 - 5055-280kv Brushless Outrunner Motor


![imagem|690x360](upload://ddzj64Lwb7XbcpBnhDIRnqouLre.png) 
![imagem|690x387](upload://A5dDTAJ45vsp1hxVdi7tr0pOZUz.png) 
![imagem|690x421](upload://sge883fSZNaNSkTUVlGeLmRSHZe.png) 
![imagem|690x413](upload://gsbIvpFb9w6eKwQY8su41Zj8Idg.png) 
![imagem|690x415](upload://bNxjbgEHXyRNuZEa96gHiL3iDFd.png) 

This is all I have, if you know why my skateboard turn off when I’m running at full speed on a climb, please tell me why, and what I can do for not  happen anymore.

(I already have one topic with the same question, but with no answers, I will delete the older version)
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-03-18T21:45:48.181Z Reads: 44

```
Most likely something is to hot.  When you climb a hill it uses a lot of amps to produce the torque needed, what generates lots of heat in the ESC and motor.  Once the components cool off it will function normally.  Check the mosfets on the ESC and the can of the motor when it cuts out next, if both are cool enough to touch then look for the corresponding setting in the vesc tool and raise the limit

What diameter wheels and gear ratios are you running?  With a 245kv motor you may be stalling out on the hills because the board cannot provide enough torque to move your mass up the hill

I hope you meant 10s2p battery...
```

---
## \#3 Posted by: pedro Posted at: 2019-03-18T21:58:21.593Z Reads: 43

```
[quote="ZachTetra, post:2, topic:87562"]
you may be stalling out on the hills because the board cannot provide enough torque to move your mass up the hill
[/quote]

Yes is 10S2P
The ratio is 42T/14T 3:1 
wheels 83mm

 The motor was hot but not to hot, I can touch without burning my hand. I will check the Vesc on next time .
What you mean raise the limit? The amp? My BMS max current continuously is 45 AMP and my cells can discharge 22amp I have 2 parallels so it is 44 amp, they have a boost for short of time.

And Thanks for answer
```

---
## \#4 Posted by: ninTHIENdo Posted at: 2019-03-18T22:02:08.000Z Reads: 38

```
Your voltage cutoff seems a little high also, could possibly be hitting the cutoff on the hill climb due to voltage sag on those batteries.
```

---
## \#5 Posted by: pedro Posted at: 2019-03-18T22:07:20.829Z Reads: 35

```
[quote="ninTHIENdo, post:4, topic:87562"]
our voltage cutoff seems a little high also, could possibly be hitting the cutoff on the hill climb due to voltage sag on those batteries.
[/quote]

The cutoff 34 V is when your battery start dying and the vesc give less amp to motor and you know the battery is almost over. aT least is what a video on youtube say. correct me if I'm wrong!
```

---
## \#6 Posted by: ninTHIENdo Posted at: 2019-03-18T22:19:51.728Z Reads: 31

```
Yes, you’re correct. But does it sag past that point during the hill climb and sag to your hard cutoff?

But your board turns completely off, so it could also be hitting your bms cutoff shutting it down. Yes your bms is rated at 45amps and your setting is at 40amps, but it shuts down your board like a bms issue.

I’m just trying to help you come up with a solution one step at a time like I would do if it was my board.

I’m just trying to help figure out different solutions as to what’s going on for you and this current setup without any actual ride data numbers to go off of...
```

---
## \#7 Posted by: ZachTetra Posted at: 2019-03-18T22:50:46.515Z Reads: 23

```
There are sensors in the motors and ESC that will shut off if too hot...look for anything with a temperature unit
```

---
## \#8 Posted by: Skyart15 Posted at: 2019-03-18T22:55:38.406Z Reads: 23

```
Just out of curiousity how fast are you able to go with those motors? I have similar motors from propdrive 5060s 270kv and im thinking of using them forbmy build. And do you guys think 12s as to high for those motors?
```

---
## \#9 Posted by: ninTHIENdo Posted at: 2019-03-18T22:58:05.698Z Reads: 21

```
Too high for the motors? No.

Too high for the erpm limit, absolutely
```

---
## \#10 Posted by: pedro Posted at: 2019-03-18T22:58:11.884Z Reads: 24

```
To fast, I never get the max speed because is to fast, the max I can go safety is 25/28 km/h after that my skills can get
```

---
## \#11 Posted by: pedro Posted at: 2019-03-18T23:00:26.573Z Reads: 23

```
I thing next time I will run with the vesc outside from the encloser and see if turn off, if yes maybe is BMS is getting to hot
```

---

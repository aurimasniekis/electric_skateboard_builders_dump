# DIRT(y) Jones &#124; Fresh bulid&#124; Ground industries Patrol &#124; 6368 190kv &#124; dual FSESC v4.2 &#124; 9s15Ah &#124;chain and sprocket

### Replies: 9 Views: 351

## \#1 Posted by: jonez Posted at: 2019-06-17T16:49:13.564Z Reads: 107

```
Please tell me what do you think about that setup, I'm starting to build my own mountainboard, has to have speed and range, below I created a part list, is mainly Chinese, but I guess is worth using, at least some of this parts

Board - Ground Industries Patrol 
![image|614x461](upload://xHQzA242MFCBBwJYFZqnnqzPchJ.jpeg) 

**Engines - sensorless, 190kv**
https://www.aliexpress.com/item/NEW-6368-BLDC-outrunner-brushless-motor-190KV-280KV-sensored-sensorless-22-48V-for-electric-balancing-scooter/32908081789.html?spm=a2g0o.cart.0.0.18943c00axPHOO

**VESC - Flpksky** 
https://www.aliexpress.com/item/FLIPSKY-FSESC-50A-V4-12-Multi-purpose-ESC-Electronic-Speed-Control-for-Electric-Skateboard-RC-Car/32916597684.html?spm=a2g0o.cart.0.0.18943c00axPHOO

**Anti-spark with switch - pro version**
https://www.aliexpress.com/item/Hglrc-FLPSKY-Anti-Spark-Switch-Smart-280A-13s-Wide-Application-for-Electric-Skateboard-Scooter-Robots-Accessories/32962668949.html?spm=a2g0o.cart.0.0.18943c00axPHOO

**batteries - 3 pieces**
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack-xt-90.html

**remote**
https://www.aliexpress.com/item/2-4GHz-Radio-Transmitter-Mini-Radio-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard-Longboard-Remote/32972578016.html?spm=a2g0o.cart.0.0.18943c00axPHOO

To convey power from motors to wheels I'm planning to use chains and metal sprockets

I'm still not sure about BMS tho, what do you think will be fine?

I'll create my own motor supports, from the block of aluminum

I was wondering and troubleshooting a lot, and as much as I've already got mountainboard set, I don't know if the setup I've chosen is right

I appreciate any help, sorry for missing parts if there are any 

Cheers!
```

---
## \#2 Posted by: Dirt_Bag Posted at: 2019-06-17T23:04:50.564Z Reads: 72

```
I would get lower kv motors and a 10s or 12s battery thats ATLEAST 10ah. A 5ah 9s battery will give you about 4-6 miles of range at most.


Those vescs might be the older version of the fsec 4.12 before they upgraded them.

You should try for 150kv or less with 12s while using a vesc 6. I recommend the flipsky dual 6.6. It runs 12s foc flawlessly

Also, you probably want sensors.
```

---
## \#3 Posted by: Rustedbucket Posted at: 2019-06-17T23:35:53.421Z Reads: 70

```
if you are looking at doing a chain drive system you could have a look at sprockets and chains on https://www.gearsandsprockets.co.uk/ i've found these guys to be a one stop shop for this type of stuff.

probably want a 04b chain and sprocket to go with it, would have to ask around about chain on mountain boards as i have no experience with building them.
```

---
## \#4 Posted by: jonez Posted at: 2019-06-18T14:51:12.910Z Reads: 60

```
Thanks!
Ok, lets say I'll get FSESC up to date, what's the difference between one and two devices, besides the number?

And 150kv will be good for small hills? I need speed but it would be usless when i'll not be able to go up the small, long hill

Sensors will make it go smoother?
```

---
## \#5 Posted by: jonez Posted at: 2019-06-18T14:54:44.976Z Reads: 53

```
Right, thanks!

Primarly I wanted to use sprckets and chains from minibikes 
![image|240x210](upload://zEh1xaiECUklmZGCJX6qhq9TDj4.png)
```

---
## \#6 Posted by: Dirt_Bag Posted at: 2019-06-18T18:55:10.816Z Reads: 49

```
You need to balance kv and voltage to get you good speed and torque balance.

The difference is that the vesc 6 uses better hardware and is more reliable at higher voltage. It also has higher current abilites which you really need for a mtb
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-06-18T19:43:37.304Z Reads: 45

```
Don't forget that the 4.2 flipsky's and the 6.6 flipsky's have a voltage drift of -0.6/+0.6v...
```

---
## \#8 Posted by: jonez Posted at: 2019-06-24T14:37:07.182Z Reads: 25

```
What does it mean?
```

---
## \#9 Posted by: jonez Posted at: 2019-06-24T14:40:13.419Z Reads: 26

```
Made few changes
went for
https://www.aliexpress.com/item/HGLRC-FLIPSKY-Dual-FSESC-4-2-100A-ESC-Electronic-Speed-Control-for-Electric-Skateboard-RC-Car/32953409487.html?spm=a2g0s.9042311.0.0.4bec5c0fjPF1sw

Do you think that going for two of 5Ah 5s 25-50c will be good idea?

 https://hobbyking.com/en_us/turnigy-nano-tech-5000mah-5s-25-50c-lipo-pack-xt-60.html will be good idea

Antispark made out of the xt90S connector will do?
```

---

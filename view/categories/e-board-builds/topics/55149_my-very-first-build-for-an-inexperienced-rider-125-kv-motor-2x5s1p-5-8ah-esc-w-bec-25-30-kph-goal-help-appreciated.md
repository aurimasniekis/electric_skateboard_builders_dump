# My very first build - for an inexperienced rider. &#124; 125 KV motor &#124; 2x5s1p 5.8Ah &#124; ESC w/BEC ~25-30 kph GOAL &#124; Help appreciated!

### Replies: 8 Views: 1272

## \#1 Posted by: Hoaz Posted at: 2018-05-11T21:08:47.999Z Reads: 178

```
_Hi!_

I'm quite new to this sub and have been lurking  and trying to navigate the forum for the past few week(s). I utilized this lurking time by studying, for a lack of a better word, how to build an E-SK8board. I do not really have a budget, other than that I wish to spend the least amount of money, while not skimping on quality parts.

My goal is to achieve a stable 25~30 Kph ride with around 15 km range, and easy charging. From what I have gathered, by studying on this site alongside other means of research,  the _three_ most important parts are the _motor, battery & esc/vesc_. I _believe_ I have selected parts which should meet my goals. Nevertheless, let's get right to it.

Starting off with what will drive my board forward, the motor: 
Turnigy D5035-125KV Sensored Brushless Motor
https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html

Note: From my understanding, this motor has great torque, but lower speeds.Further, I believe the torque also helps with climbing hills and such and keeping stable speeds overall.  Which is why this is my pick. (*Suggestions for other, better, motors are appreciated*)

Next up, the battery:
ZIPPY Flightmax 5800mAh 5S1P 30C x2 in serial (so 10s at 5.8Ah - 37v)
https://hobbyking.com/en_us/zippy-flightmax-5800mah-5s1p-30c.html

Note: This will give me 5.8 Ah, and since it has an alright C-rating, I believe it to be a good fit for my motor (and ESC/VESC??). To be honest, I am not sure what 1P means in the name. I picked this because I thought I'd want one with an alright C rating, and because my motor says it's capable of 8 - 12S batteries.
(*Again, suggestions for other batteries are appreciated*)

Followed by the last important part, the ESC w/ BEC or VESC:
Turnigy SK8-ESC V4.12 For Electric Skateboard Conversion w/BEC
https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

Honestly this topic is the one in which I am the least knowledgeable about. I am not entirely sure exactly what to look for, other than that it needs to be capable of driving the motor and receiving from battery. I also know that the BEC is necessary for actually controlling the skateboard. I have looked at VESC, but they are almost doubled the price sometimes. Maybe there are ones that I have missed and are better than ESC, if you know of some, then please don't hesitate to suggest.


Now for the smaller bits and bobs, starting off with the drivetrain & pulley-kit and so on. 
https://www.banggood.com/DIY-Electric-Skateboard-Kit-Parts-Pulleys-And-Motor-Mount-For-80MM-Wheels-p-1146629.html?gmcCountry=SE&currency=SEK&utm_source=googleshopping&utm_medium=cpc_elc&utm_content=vivian2&utm_campaign=pla-all2-se-pc&gclid=EAIaIQobChMI4Kmk8pjX2gIVEhsYCh0VEACBEAQYAiABEgKnaPD_BwE&cur_warehouse=CN
This one's quite cheap, but I am not entirely sure about the amount of teeth for the Pinion and spur (which is arguably important for achieving high torque and speeds ) . I hope it's metal, but it could be plastic. I want one which is stable. I am not entirely sure if it's entirely compatible with my motor (shaft size and all). Also, how do I know if it fits with my trunk? Is the size standardized?

Note: Would love your input here

Next up, wheels:
I have not selected any wheels. Other than I know I want 83/90 mm wheels. And from what I know, the size will also dictate which motor mount & pulley that I should purchase.

Skateboard: I am looking for one on the cheap. I am certain it is going to be a longboard, however.

Trunks: Again, I am not entirely sure about this area. I would think that the shaft size matters and the shape of it, other than that, I don't think much else matters. Hopefully I can keep the trunks that comes with the longboard.

Controller: Bluetooth & Phone - is this possible? (Coding dedicated software), could really save on the build this way.


The total build price, the longboard aside, is around: ~300 euros (likely to be more).

On another note: I have never skate before, so I am not sure how fast is _fast_. I reckon a bike to ride at around 15~25 Kph. I would not need to skate faster than a bike. 

Also, am I right in thinking that higher torque = stable speeds in hills and normal roads alike?

**Any input, any suggestion etc is and will always be appreciated. 
I am here to learn, to build and to skate. Hopefully this build with satisfy my skateboarding needs.**

Thanks, kbye

Yours truly,
a fellow eskatebuilder.

EDIT: After some _very intense_ , discussion with my friend. We thought this motor: 
https://hobbyking.com/en_us/turnigy-sk8-6374-192kv-sensored-brushless-motor-14p.html 
might be better suited

what are the thoughts on this motor/ new edited setup?
```

---
## \#2 Posted by: Zertax Posted at: 2018-05-12T06:13:03.130Z Reads: 129

```
Trunks :smile: you don't need much storage on a skateboard you might want to consider trucks :slight_smile: you're definitely going to need a Bluetooth module, Android should work with Arduino without I don't know, also Android controller might be dangerous. You will also be needing a charger and BMS/balance charger.
Motor and battery's seems fine, vesc I don't know.
1p means how many sets in parallel.
```

---
## \#3 Posted by: bloke900 Posted at: 2018-05-12T08:14:56.558Z Reads: 126

```
I have used this motor with 10s battery, 15/36 pulleys and a 97mm wheel.  This had more than enough torque, bit no way will you get more than 25kmph with it in this gear ratio.   I was considering running a 20t motor pulley - picked up a 192kv motor instead.
```

---
## \#4 Posted by: E1Allen Posted at: 2018-05-12T08:26:22.301Z Reads: 132

```
Congrats on wanting to do your first build.  It looks like you have done some homework, much appreciated.  I would suggest a vesc for a speed controller but it's a little more expensive.  Maybe a mini remote because they work well and are cheap. Search for one of the hm10 Bluetooth modules such as metr.at they are fairly inexpensive.

Diyelectric has a combo kit with wheels (not the best) for a single motor setup.  Or search for that bangood one on the forum for a review because I'm not sure if it's quality.

Use this for calculating your setup

http://calc.esk8.today
```

---
## \#5 Posted by: 257 Posted at: 2018-05-12T08:42:07.291Z Reads: 126

```
I'm still working on my first build as well, so my opinion may not carry much weight but from what I've absorbed from my own "lurking around" I'd recommend a Focbox rather than a less reliable copy, which @longhairedboy has here 

https://longhairedboy.com/collections/all/products/focbox-electric-skateboard-motor-controller?variant=1796552294411

If you are looking for sufficient hill climbing power I'd say go for a 6355 or 6374 over a 5035. 6355's might be up your alley if you're hoping to keep the stock trucks on your deck. If you don't mind going in on some wider trucks for 6374 motors, torqueboards makes a nice set of 218mm trucks here

products/torqueboards-218mm-trucks

The turnigy Sk3 6374's are popular on here as well as torque boards, alien power system or build kit boards by @jlabs 

https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
products/electric-skateboard-motor-6355-190kv
http://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-200kv-3200w/
https://buildkitboards.com/collections/motors/products/6374-190kv-motor

If you are going for a LiPo battery over Lithium ion you may want to check out @Namasaki's thread that has tons of info and an excellent step by step guide for putting together a powerful 10s battery with a BMS for simplifying charging and reducing the risk of overdischarge 

http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014

For your pulley kit I'd say check out @johnny_261's stuff as his seem to be much higher quality than bang good's. 

http://www.electric-skateboard.builders/t/15mm-wide-pulley-kits-wheel-motor-pulleys-belts-and-hardware/17131

If you need a more complete mounting kit look into torqueboards stuff as well. 
In terms of wheels I've seen lots of people go for MBS's 100mm all terrain wheels

https://www.mbs.com/parts/13401-mbs-all-terrain-longboard-wheels-black-4

But if you're set on 83/90mm maybe check out some Orangatang's, Evolve's wheels, or even an Amazon search brings some up for around 20 bucks

https://orangatangwheels.com

https://evolveskateboardsusa.com/collections/wheels/products/evolve-gt-street-wheels-black-83mm-76a
```

---
## \#6 Posted by: pat.speed Posted at: 2018-05-12T08:45:14.167Z Reads: 97

```
The turnigy esk8 motor is not a 5035, it is a 6374(?). The 5035 is the stator size, which is quite large
```

---
## \#7 Posted by: Hoaz Posted at: 2018-05-28T18:51:34.156Z Reads: 73

```
So, I've decided I probably want to go for this motor instead:
https://hobbyking.com/en_us/turnigy-sk8-6374-192kv-sensored-brushless-motor-14p.html

Would this be a good decision? 

Also, thank you all for the responses, I will look at the VESC and the pulley kit that you guys have mentioned
```

---
## \#8 Posted by: Hoaz Posted at: 2018-05-30T20:31:51.848Z Reads: 62

```
So,what would the range be on this setup?

With the motor and with the battery? I weigh 65 KG.

this site http://calc.esk8.today/ gave me  19 km. Would this be right?
```

---

# Expert review needed!

### Replies: 10 Views: 1500

## \#1 Posted by: D3rax Posted at: 2017-07-16T18:17:38.603Z Reads: 189

```
Hello everyone,

First let me start off with a big thanks to the community on this site! This site is packed with lots of great info that helped me a long way.

I've recently started my own electric mountainboard build. I finished restoring and upgrading my old MBS atom 85 board by reinforcing the deck and replacing the tires and bearings. Also my 3d printed drive gears and motor mounts are nearly finished. 

Here are some pictures of my progress so far:

<img src="/uploads/db1493/original/3X/a/4/a469de01dd68e4ae39ac72d254f478e775be92aa.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/f/5/f5c8562f2dcb8c141944740091726f7ebd354996.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/e/8/e88106dec52a3fb724147a768f42fd8ec1b2fb6c.JPG" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/1/d146dd07e18848c0f986e135a999a3e4cc4d5a3c.JPG" width="666" height="500">

I'm now at the point that I want to order all the electronics for my board, like the motor's, vesc's, batteries etc. Based on the informatie on this site I've made a selection of the parts I want to order, but before I do I hope I can get some good advices for you guys to see if my setup is correct or that I'm about to make some mistakes!

I've calculated the following setup with ESK8 Calc:

<img src="/uploads/db1493/original/3X/9/7/97908ac237fcdad92967377932e3be71629706f4.jpg" width="649" height="500">

I'm looking for a top speed of about 30 - 35 km/h (my weight is about 70 kg). I'm not planning to use this board on offroad terrain, mainly regular roads or light gravel roads. Is my gear ratio correct? Is the motor KV correct, or should I use a higher KV of 192? Could I decrease to 6s with a 20 teeth pulley? I'm not sure which combination is better, I hope you guys have some tips or suggestions.

Based on the above calculation I want to order the following parts:

* [2x Turnigy Aerodrive SK3 - 6374-149kv Brushless Outrunner Motor (€69.30 per motor)](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html?___store=en_us)

* [2x FOCBOX Motor Controller ( €150.77 per vesc)](http://www.enertionboards.com/electric-skateboard-parts/vesc-x-programmable-brushless-motor-controller/)

* [2x ZIPPY Flightmax 5000mAh 5S1P 20C (2 packs wired to 10S, €38.15 per pack)](https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html?___store=en_us)

* [HobbyKing® ™HK-GT2B 3CH 2.4GHz Transmitter and Receiver w/Rechargable Li-ion Battery (€20.45)](https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html?___store=en_us)

I really would like to know what you guys think about the usability of this setup. As I said i'm not looking for a very high top speed, about 30 to 35 km/h is good enough. I do want a board that has enough torque and that has the ability to climb slightly medium hills.

Thanks for all your input and suggestions. I will report the progress of my build in this thread!

Best regards,

D3rax
```

---
## \#2 Posted by: Cobber Posted at: 2017-07-16T19:50:16.612Z Reads: 158

```
A couple of things, I'm not a expert but...
You have your wheel size as 120mm on you calc, but your mbs wheels have 200mm written on them. 
I think people have been getting better results with the "[gt2b](https://hobbyking.com/en_us/hobbykingr-tmhk-gt2b-3ch-2-4ghz-transmitter-and-receiver-w-rechargable-li-ion-battery-1.html)" controller. Thats what I've gone with.
I'm not sure if anyone has got that esc to work on a esk8 before, you do realize it has no BEC so you will need to work out how to power your receiver?
```

---
## \#3 Posted by: wafflejock Posted at: 2017-07-16T20:06:22.533Z Reads: 159

```
Why this ESC over a VESC?  Configuration on these things is a PITA you have to hold buttons while powering things on and wait for the right number of beeps then pull the trigger, or buy some extra programming hardware and use their proprietary (likely windows only) software to configure the ESC.

VESC by comparison, open hardware, open source software for configuration, used by I'd say at least 80% of people here so lots of experience and people here who can actually do repairs on them as well (if you do blow the DRV chip).  You plug it in via USB (a standard all computers have) and use the configuration tool to set everything you want it to do or not do by just typing values into the boxes and writing the configuration (hitting a button).  I bought and fried a few cheaper ESCs before getting a VESC but really just save the money and get a VESC in the first place.
```

---
## \#4 Posted by: D3rax Posted at: 2017-07-17T13:59:50.510Z Reads: 120

```
Thanks for your suggestions. I indeed entered the wrong wheel size....I changed it to 200mm. And I changed the teeth of the motor pulley to 15T, because my top speed became about 50 km/h.

I used this esc on advise of hobby king, but I as you guys suggest buying a VESC makes more sence. So I changed the esc to FOXBOX vecs.
```

---
## \#5 Posted by: D3rax Posted at: 2017-07-19T13:59:28.380Z Reads: 99

```
I hope somebody also can give some advice regarding gear ratio, motor KV and battery volts. Will my current setup give a board that has enough torque and will not draw to many amps?
```

---
## \#6 Posted by: Cobber Posted at: 2017-07-19T19:48:24.538Z Reads: 98

```
10s is a good middle ground for vesc reliability and gets the volts up but the amps down. I'm going 12s on my build but you need to be careful with your (v)esc at 12s not to have problems with both selection and settings.
For example the older vesc have a max erpm limit of 60K. Your under that though so you should be fine in that regard with current specs.
```

---
## \#7 Posted by: D3rax Posted at: 2017-07-21T12:55:34.951Z Reads: 86

```
Alright good to know! 

One thing I was wondering about is the motor RPM. I have it now calculated on 5513 RPM and 4686 RPM (weighted). Regarding this [thread](https://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53?source_topic_id=215), the motor RPM shoud be aroud 8000 - 9000 RPM.

> HOT TIP: The general theory of efficient drive train design is to aim for the highest possible reduction ratio, whilst keeping the motor in the 8000 - 9000rpm range where the motor losses are at minimum. 

Is my RPM to low or is this still okay? I could increase the RPM by using a higher KV motor. A 260 KV motor in this setup results in a RPM of 9620 and 8177 weighted. But as I understand correctly is a lower KV better for getting enough torque?

What is the best option to choose? A lower KV motor with a lower RPM or a higher KV motor with a RPM around 8.000?
```

---
## \#8 Posted by: wafflejock Posted at: 2017-07-21T18:42:26.575Z Reads: 69

```
http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125

^^ that might help.  In general lower kv with the same power means that power is being used for torque instead of RPM (otherwise where is it going? turning power is a product of torque and rpm) but like he explains in the write up there it's not a direct correlation it depends ultimately how much copper is in the motor and how many windings there are what the trade off with torque and/or RPM will be.  Keep in mind you can also adjust the torque/top speed trade off by adjusting the gearing and/or wheel diameter, it basically comes down to what target top speed do you want given the components you want to use (perhaps preferences on wheels or other things drive some of the choices).
```

---
## \#9 Posted by: D3rax Posted at: 2017-07-23T14:21:16.273Z Reads: 50

```
Very helpful information, especially the artikel from vedder!

Based on this information I need to aim at a 8.600 RPM. With a 10s battery I think the best Turnigy SK3 option would be the [213 Kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html?___store=en_us) model. This gives me 7.881 RPM, that should be close enough right? 

I don't want to get a 245 KV. This gives me 9065 RPM, but over shoots the 60.000 ERPM limit and gives a top speed thats way to high.

This is my revised calculation:

<img src="/uploads/db1493/original/3X/c/3/c31ffbb79b07c3446aa165a1b4ecd9c4cccb8f7c.jpg" width="646" height="500">

What do you guys think?
```

---
## \#10 Posted by: Dameshh Posted at: 2017-11-25T04:52:10.694Z Reads: 26

```
what if i use dual 270kv alien motor on a 18 to 36 gear ratio with 10s lipo and a set of focboxes. would i blow the focboxes? how fast do you think i would go?
```

---

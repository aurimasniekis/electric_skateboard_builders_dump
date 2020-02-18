# Need some help with parts

### Replies: 14 Views: 389

## \#1 Posted by: Louismxopen Posted at: 2018-10-08T14:51:29.682Z Reads: 73

```
Hey guys,
i want to upgrade my latest Mountainboard build. Actually I got 2 Esk8 Controllers, and my plan was to use the following other parts. What do you guys think about this?

Motors: https://hobbyking.com/de_de/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html

Battery two 6s in series so 12s: https://hobbyking.com/de_de/multistar-high-capacity-16000mah-6s-12c-multi-rotor-lipo-pack-w-xt90.html

BMS for the 12s: https://alienpowersystem.com/shop/bms/battery-bms-with-switch-for-12s-lipo-battery-l16s50/

happy for any answer or help!
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-10-08T15:24:21.590Z Reads: 67

```
the motors you've chosen are good but unsensored. you'll find that you'll struggle a bit off the line without pushing first. if you want sensored go for the sk8 range. Also, those batteries i have heard nothing but bad things about them
```

---
## \#3 Posted by: Louismxopen Posted at: 2018-10-08T15:56:23.824Z Reads: 59

```
https://hobbyking.com/de_de/turnigy-sk8-6374-192kv-sensored-brushless-motor-14p.html

Are 192kv to much for 12s Power what do you think?
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-10-08T16:03:38.901Z Reads: 50

```
What are the specs of your current board? Battery, motor size and kv, gearing, wheel diameter, esc?

@mynamesmatt is right, those batteries are terrible and completely unsuitable for esk8 applications. Save yourself the headache (and unquenchable fire) and get higher quality lipos or liion packs. 

https://hobbyking.com/de_de/turnigy-4000mah-3s-40c-lipo-pack-xt-60.html

I am using 4 of these in series. WAY more punch. It won't last as long on a charge, but they won't explode either.

https://hobbyking.com/de_de/turnigy-sk8-6374-149kv-sensored-brushless-motor-14p.html

Here is the 149kv version of that motor.

I am using 190kv on my 12s battery without problems. I just limited it to 60000erpm in the bldc tool.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2018-10-08T16:10:43.927Z Reads: 38

```
I run 8000mah turnigy FlightMax in a 5Sx2 config at 10s.they also have a 4s version of this. 3 in series will get you around 35km on that motor (single drive). Its got a continuous rating of 30c (240a) and peak of 40c (320a)
```

---
## \#6 Posted by: Louismxopen Posted at: 2018-10-08T16:10:54.164Z Reads: 38

```
Actually im using: 
Motors: APS 2,2kw 270kv dual
ESC:APS Dual motor esc 
Motors and esc are the 4,4kw set from Alienpowersystems.
Battery:6s 16000mah 35C Alienpowersystems battery
Wheels:8 inch Hypa wheels
Gearing is 66 and 14 tooth belt drive

I know its a really weired electric setup but it was my first build. I think i will just buy another APS battery for the 12s setup or what do you guys say?
```

---
## \#7 Posted by: mynamesmatt Posted at: 2018-10-08T16:15:13.143Z Reads: 37

```
i say scrap the motors and batteries (sell them on here wink wink) and go for what we just said. they're much better options. if you can afford a vesc based speed controller you'll be very happy with that too
```

---
## \#8 Posted by: TheFluffiest Posted at: 2018-10-08T16:15:28.290Z Reads: 38

```
It's not bad at all!

That seems like the safest option, although I would be wary of connecting a new lipo battery to an old one. I haven't seen a reason not to trust APS products, so that will probably be the best route. You will definitely need new motors for that though, unless you get the vesc 6.6 which can handle 120000erpm (don't quote me on that, i could be wrong)
```

---
## \#9 Posted by: TheFluffiest Posted at: 2018-10-08T16:16:02.674Z Reads: 38

```
Does the battery still charge to full capacity?
```

---
## \#10 Posted by: Louismxopen Posted at: 2018-10-08T16:17:50.623Z Reads: 36

```
Yea new motors are safe, and as I said I got also 2 Vesc based Controllers:
https://store7570530.ecwid.com/#!/VESC-made-in-Germany/p/56097898/category=15255004

And the Battery still charges up to 25,2 Volts and all Cells going up to the Cutoff Voltage 4,2 Volts or something like that.
```

---
## \#11 Posted by: TheFluffiest Posted at: 2018-10-08T16:28:05.380Z Reads: 31

```
It should be safe to wire in series then... I would wait for more input on that thought before ordering. 

Those look like focboxes! Very cool! The specs on it are very good as well. 

I would go max 190kv on motors, you should be ok in that range. Just be sure to limit the erpm to 60000 or it will kill the vescs.

Do you have pictures of your current setup?
```

---
## \#12 Posted by: Louismxopen Posted at: 2018-10-08T16:32:26.588Z Reads: 28

```
![image|666x500](upload://1agPQYtX2cVuTVVZZinthDhIxKB.jpeg) ![image|375x500](upload://A6Ba8w5no5S4LYjqoOPbGiMabvH.jpeg)
```

---
## \#13 Posted by: Louismxopen Posted at: 2018-10-08T16:34:31.668Z Reads: 28

```
![image|375x500](upload://eoiRSlQwToMzAZxLUXSr6utbMT3.jpeg) ![image|666x500](upload://ezHU6Ca4OUDRqxcXq7ZnEgkeMwd.jpeg)
```

---
## \#14 Posted by: Louismxopen Posted at: 2018-10-09T17:48:09.930Z Reads: 24

```
So I think I will buy following Motors: 
https://hobbyking.com/en_us/turnigy-sk8-6364-190kv-sensored-brushless-motor-14p.html?___store=en_us

all the other motors are selled out up to January 2019... 190kv at 12S would work or what do you guys say? Just limiting in BLDC tool to 60000 right?
```

---

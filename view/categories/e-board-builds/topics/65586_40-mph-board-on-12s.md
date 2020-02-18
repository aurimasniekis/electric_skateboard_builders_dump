# 40 MPH Board on 12s

### Replies: 13 Views: 501

## \#1 Posted by: KeivanM Posted at: 2018-08-21T12:30:41.992Z Reads: 173

```
Hello to everyone, I have just finished building my 40 mph board and I am toying with the bldc tool for my dual foc boxes, and I have no idea what to do here.

Something that I want to fix is the fact that my controller is super sensitive for breaking and accelerating and I wanted to see if anyone knows how to fix that. 

![image|690x388](upload://mslxdAwjCvYyHifFnNugPgnscZT.png)


Here is what I have so far on my tool configuration. For reference I am running 12s4p on dual 6347 192kv SK3's on dual focboxes, on a 20/36 ratio on 97mm's. I just want my board to be fast and not fry this thing, any tips will be appreciated! & also yes I did read the beginner thread on VESCS and what not.
```

---
## \#2 Posted by: KeivanM Posted at: 2018-08-21T12:31:07.961Z Reads: 157

```
I also want to make sure regenerative breaking works well too!
```

---
## \#3 Posted by: rey8801 Posted at: 2018-08-21T12:41:01.865Z Reads: 151

```
I would suggest to dowload the new vesc tool and follow the wizard for motor detection and ppm (remote) configuration. It will cover most of the steps automatically. You only need to know the max motor amp (datasheet of the motor on HK website), motor min start with the same value of motor max but negative (like max 60, min -60). Battery max depends on the cells you used, so which one? same for battery min. Although keep in mind that if this one is your first esk8 since you do not know how to configure a dual 6374 is gonna fly so maybe start low with the value anyway and then increase later on. If you installed a bluetooth module it can be done via your phone without open the enclosure anymore.

EDIT: Checked your motors. They are rated 80A max current. So this one is the max value. I would say that 60A you won't be able to stay on the board, so start with 40A maybe, and -60A motor min for nice brakes.
```

---
## \#4 Posted by: mixedcreation Posted at: 2018-08-21T12:45:57.709Z Reads: 138

```
Values look low for a 12s build.  Besides that, I can't tell you how many threads there are about 12s dual 6374 build.  Search VESC settings for 12s.  I guarantee you will find information.  Also search Ackmaniac's thread as he has provided help to many folks on values to set.

It also worries me you are building a board that is capable of high speeds, but you don't know how to configure it.
```

---
## \#5 Posted by: KeivanM Posted at: 2018-08-21T13:02:05.242Z Reads: 127

```
I am using samsung 30q cells, should i do battery current max 60a and max regen -60a?
```

---
## \#6 Posted by: KeivanM Posted at: 2018-08-21T13:02:28.381Z Reads: 121

```
ok will do
```

---
## \#8 Posted by: KeivanM Posted at: 2018-08-21T13:04:35.275Z Reads: 114

```
I am also using the battery from diyelectricskateboards, it has a built in bms too
```

---
## \#9 Posted by: rey8801 Posted at: 2018-08-21T13:09:19.385Z Reads: 123

```
No so 30Q is rated at 15A but by real test it performs good at 20A, so 20A x 4 you have 80A total so on single vesc is 40A max bettery ( I see that your battery has a 60A discharge BMS, so if you didn't bypassed it the value are **30A max battery** on each VESC and not 40A! It's important or the BMS will shout down the board). Battery min is 4A x 4p = 16A so -8A each vesc for battery min.
I really advice you to use the VESC tool, but anyhow read about value meanings because you called them wrong. Motor max and min is the current at the motor level. Battery max and min is the current at VESC level and it depends on your battery. The BAttery max and min has to be divided by 2 if you run dual vesc.
How did you connect the two vescs? CAN BUS or splitted PPM?
```

---
## \#10 Posted by: KeivanM Posted at: 2018-08-21T13:17:18.656Z Reads: 113

```
I connected them with the can bus
```

---
## \#11 Posted by: rey8801 Posted at: 2018-08-21T13:36:58.420Z Reads: 112

```
ok perfect then i fyou use the VESC tool you only need to follow the wizard and it will do the job for you. I advice to remove the can bus. Connect the master VESC and to Wizard motor detection, once done, repeat the same for the slave vesc. Remember to give VESC ID 0 to master, adn 1 to slave. The VESC tool will do all the rest.
Then connect the can bus. Connec to the master the usb cable, run remote wizard, adjust the ppm signal ecc...it will guide you. Then disconnect it, connect to the slave and do it there. You will see that once you say that is the slave it's done automatically. Done! Remember never never connect the can bus to the two vesc if one is not powered. turn off the board. connect the can bus then turn on the board with both of vescs being powered.
Watch this video and repeat https://www.youtube.com/watch?v=v1glLDO-EjA&t=1130s. Of course applying the values that we discussed before.
```

---
## \#12 Posted by: dareno Posted at: 2018-08-21T19:22:03.484Z Reads: 81

```
[quote="rey8801, post:11, topic:65586"]
Remember never never connect the can bus to the two vesc if one is not powered. turn off the board. connect the can bus then turn on the board with both of vescs being powered.
[/quote]

This is invaluable advice my friend!!!!
```

---
## \#13 Posted by: rey8801 Posted at: 2018-08-21T19:32:16.197Z Reads: 75

```
The new Flipsky vesc6 seems able to handle it but I would avoid anyway :grin:
```

---
## \#14 Posted by: dareno Posted at: 2018-08-21T19:36:30.424Z Reads: 71

```
Apparently all 6 variants can but yeah, not willing to give that a go lol
```

---

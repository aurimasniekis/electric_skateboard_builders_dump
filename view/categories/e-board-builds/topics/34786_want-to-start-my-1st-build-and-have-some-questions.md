# Want to start my 1st build and have some questions!

### Replies: 13 Views: 750

## \#1 Posted by: Gloostik Posted at: 2017-10-04T20:50:12.384Z Reads: 105

```
so after read a lot of stuff on here and around other sites I've decided I want to build an eboard. I've read a lot of posts over the last few days and feel fairly confident in my choices for parts but I would feel better if someone looked them over just to double check that they all work together etc. 

My goal for this build is a board that will cruse in the 25mph range and have about 10 miles as I want to ride it to school/around town and its about 7mi to school and I like having room to spare. I would also like it to have a single charging port that will charge the whole battery bank so I can charge it while in class without taking it apart.

**parts list:**
[Trucks](https://www.amazon.com/Caliber-Trucks-Cal-50%C2%B0-Longboard/dp/B072J845HD?th=1): Caliber II
[Wheels](https://www.amazon.com/Longboard-Flywheels-Wheels-Bearings-Spacers/dp/B00IO5D5XW?th=1): 83mm flywheels
[Battery](https://hobbyking.com/en_us/zippy-flightmax-5000mah-2s1p-20c.html?___store=en_us): Zippy flightmax 5000mah 2s1p X 5 for a 10s bank
[Motor](products/electric-skateboard-motor-6374-190kv-3150w): torque boards 190KV 6374
[Motor mount/pulley kit](products/single-bolt-on-motor-mount-w-drive-wheel-kit): torque boards bolt on w/ 16T/36T pulley kit
[ESC](products/torque-esc-vesc-bldc-electronic-speed-controller): Torque VESC
[Controller](https://www.amazon.com/XCSOURCE-Transmitter-Controller-Receiver-Skateboard/dp/B073GX83NH): XCSOURCE 2.4GHz Radio Transmitter Remote Controller

This is the specs I got using a calculator:
<img src="/uploads/db1493/original/3X/0/4/04f6117b47bb2811dec1b99767ec0e4782a8ef6c.jpg" width="666" height="500">

Now my main questions (as long as the parts work together) have to do with the battery bank. So from what I can tell, I would take 5 of the 2s1p batteries and wire them in series to get my 10s bank. However I want to wire them to a BMS so I can charge it as a single bank instead of each battery individually. I read [Connecting a BMS Quick Guide [How-to]](http://www.electric-skateboard.builders/t/connecting-a-bms-quick-guide-how-to/6122) and it was extremely helpful however I can't seem to find where to get a BMS and I want to make sure that this will even work before I start buying parts. From what I can read it seems like if done properly you can have a single charging port and plug it right into the wall with the right charger? (like this one? [Charger](https://miamielectricboards.com/shop-1/12s-charger)). Also would it just be easier/cheaper to make my own banks with say, these? ([Batteries](https://www.amazon.com/dp/B00NUI44N8?tag=mike0939-20))

I'm no master at any of this, just some hours of research so excuse my ignorance but if anyone has any tips or advice on how to make it better/cheaper or anything it would be greatly appreciated.
```

---
## \#2 Posted by: Shahar9320 Posted at: 2017-10-04T20:56:33.593Z Reads: 92

```
DONT GET TORQUEBOARDS' MOTOR PULLEYS !
the wheel pulleys are fine but the motor ones break in a second, it's a design flaw.. happened to me twice
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-10-04T20:58:18.704Z Reads: 89

```
that charger is a 12S charger, LiPOs are 4.20v per cell at max charge so you are looking for 42V for 10S LiPOs. But yes something like that should do the trick.

Building a pack won't be cheaper or easier but it might be a worthwhile investment in the long run. To DIY you will need a spot welder and to learn how to build the pack safely. They are available premade with a BMS, LCD and even some with USB ports if you want to save the hassle of building yourself.
```

---
## \#4 Posted by: Gloostik Posted at: 2017-10-04T21:10:40.615Z Reads: 87

```
Thanks for the heads up! are there any alternatives you would suggest?
```

---
## \#5 Posted by: Gloostik Posted at: 2017-10-04T21:15:04.674Z Reads: 80

```
Thanks for the info. I think for now ill stick with the packs and see how it goes. Maybe build my own for a different build at a later time then when i feel more confident about my eboard knowledge
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-10-04T21:16:50.854Z Reads: 76

```
that makes a lot of sense, it will add a lot to the time it takes to build the board and a lot of complexity. If it were me I would wait till the lipos are getting towards their end of life and then see if you fancy building a pack.
```

---
## \#7 Posted by: Shahar9320 Posted at: 2017-10-04T21:32:37.544Z Reads: 73

```
I'm using just a Chinese one that I bought from some website, its really good and sturdy but it doesn't have a keyway, it still works fine with the 2 hex screws but i think you'll be better if you find something with a key way, just make sure it seems like it's built well and thick enough on the sides.
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-10-05T03:50:08.348Z Reads: 65

```
I have no idea what you're talking about,  my steel ones from TB (16T) have been running for about 60 miles now with 12mm belts and they're still perfect.  Not even any tooth wear?  Maybe you got a bad batch
```

---
## \#9 Posted by: BigBoyToys Posted at: 2017-10-05T04:04:25.185Z Reads: 62

```
I don't think you will hit 27mph with a 10S pack 20C 5ah packs. I recommend 12S and voltage and higher C rated lipos, but thats just my 2 cents.
```

---
## \#10 Posted by: Gloostik Posted at: 2017-10-05T04:16:39.192Z Reads: 59

```


[quote="BigBoyToys, post:9, topic:34786, full:true"]
I don't think you will hit 27mph with a 10S pack 20C 5ah packs. I recommend 12S and voltage and higher C rated lipos, but thats just my 2 cents.
[/quote]

I also thought that was a little off. im really just aiming for the 20-25mph range. think it will do that?
```

---
## \#11 Posted by: Preston Posted at: 2017-10-05T04:59:01.899Z Reads: 55

```
Your board will definitely hit speeds of 20mph+. I suggest buying/building a 10s Li-Ion pack as they are more reliable and have better longevity if you plan on riding it to school, etc everyday.

And the motor/motor mount, pulley kit your using I've had on my setup for the past year with no problems.
```

---
## \#12 Posted by: BigBoyToys Posted at: 2017-10-05T05:12:14.923Z Reads: 51

```
Yeah 20-25mph shouldnt be a problem. +1 on @Preston suggustion to use a 10S li ion pack for ease of use and reliability.
```

---
## \#13 Posted by: Gloostik Posted at: 2017-10-05T16:53:35.661Z Reads: 33

```
alright, ill look into buying/building a li ion pack. thanks for all the input everyone
```

---

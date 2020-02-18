# Skateboard without BMS? Is it safe?

### Replies: 17 Views: 958

## \#1 Posted by: Morxy49 Posted at: 2018-07-22T21:52:24.224Z Reads: 187

```
So when building my first skateboard i accidentally short circuited my BMS and it basically want up in flames. Not literally flames, but it is definitely broken so i can't use it anymore.

However i also noticed that i simply _don't have any space for a BMS in my enclosure at all_, so even if i bought a new one i will have to modify my board drastically to make everything fit, which i don't want to do...

So, my question is, can i just don't use a BMS? 
* What are the dangers with doing this? 
* Can i charge without a BMS?
* Can i drive without a BMS?
* Will my FOCBOXes be enough to detect under voltage and shut off before the batteries get damaged?

This is my charger. I believe it should automatically shut off at 50.4 volts.
[Link to store](https://eskating.eu/product/4-amp-fast-charger/)

![IMG_20180722_234435|280x500](upload://ovGK5g04m1kGecsXMaj1zlGTGhy.jpg)
```

---
## \#2 Posted by: Grozniy Posted at: 2018-07-22T21:56:49.815Z Reads: 171

```
You can use the board without BMS.
You can't charge the batteries with that brick charger and without BMS. It only works with BMS.
Focbox should be enough to detect undervoltage.
That charger is for 12s
```

---
## \#3 Posted by: AutoItKing Posted at: 2018-07-22T21:59:51.311Z Reads: 168

```
The charger will cut off at 50.4V but it has no idea what the individual cells are doing. There could be one way over and another way under voltage. And you do NOT want to over voltage a lithium cell. A BMS is a very necessary piece of safety equipment. As Grozniy said, you can safely discharge without a BMS but do not charge without one.
```

---
## \#4 Posted by: davewood1982 Posted at: 2018-07-22T22:08:13.776Z Reads: 163

```
Yeah don't use that charger without a BMS, You could use a balance charger though i guess.
```

---
## \#5 Posted by: Morxy49 Posted at: 2018-07-22T22:12:16.879Z Reads: 159

```
So if i use for example [this charger](https://hobbyking.com/en_us/0620duo-600w-charger-300w-x2-version-2.html) it should work?

Are there any more compact options for this type of charger? I want to bring it in my backpack.
```

---
## \#6 Posted by: Grozniy Posted at: 2018-07-22T22:16:08.622Z Reads: 152

```
This one is only 6s. You need one for exact number as your S count
```

---
## \#7 Posted by: detroitwheelin Posted at: 2018-07-22T22:32:14.134Z Reads: 141

```
![makita|375x500](upload://vaTo0jSVN4HFxFEqhik3nl0xqpg.jpg)

Or you can go with a Makita 18vX2 setup like mine.  because they're running in series you need to ensure that both packs are at similar charge and then manage over discharge protection by the VESC.   Charging is super fast and managed by the Makita balance charger 

btw... i'll be making some dual makita mounts soon if anyone is interested
```

---
## \#8 Posted by: mmaner Posted at: 2018-07-22T22:44:11.341Z Reads: 125

```
I am in no way condoning the use of battery packs without a BMS... But...

I have a 10s4p 30q pack I've been running almost daily for over a year with no BMS and it's still perfect. I charge to 41.5v and discharge to 37v. My theory is that with 3p the outside series are balancing the inside series. 

I check the cells individually after a charge and 1hiur wait every day for the first couple if months. After that about teice a week. Now about once every 2 weeks. I've never had drift between cells more than . 1v. 

Just my experience...
```

---
## \#9 Posted by: Morxy49 Posted at: 2018-07-22T22:46:23.207Z Reads: 121

```
Yeah, i've seen many people on the forums doing it like this, so i'm kind of surprised that everyone say's i shouldn't do it now...
```

---
## \#10 Posted by: AutoItKing Posted at: 2018-07-23T01:39:51.071Z Reads: 114

```
Just because people do it doesn't mean it's okay.

If the battery pack is put together with good cells then you're usually okay since they're mostly well matched. But it's still good practice should you get a cell with slightly different ESR.
```

---
## \#11 Posted by: michaelcpg Posted at: 2018-07-23T02:07:27.121Z Reads: 115

```
It's certainly doable but I would never recommend going without a BMS to someone who's new to working with lithium ion batteries. 

If you're using brand new, high quality cells from Panasonic/Samsung/LG/Sony, are regularly manually testing cell voltages and are limiting your charge levels to only use part of the battery's capacity (in my case I limit charging to 4.1V max and around 3.5V min) then you should generally be ok...


BUT... even if you're doing all this, another big thing to keep in mind is that, particularly if this is your first build, you have to make sure that your battery is as robust as realistically possible. 

My early battery builds had a couple of cells in some P groups become disconnected after a fair bit of use just as a result from riding on some rough roads and my lack of skill and experience at the time with building batteries. 
This is one of those situations where everything may work perfectly for a while when you first put everything together and then something goes wrong down the road once you've got a false sense of security.

Thankfully in my case, my packs had BMS's which had fail safes that handled situations where cells become disconnected. Without a BMS, disconnected cells will be much hard to pick up and will quickly cause your battery to become massively unbalanced which is when you can really start to have problems...


TLDR: If you don't have much experience with lithium ion batteries then I REALLY WOULD NOT recommend going without a BMS if don't want your house to go up in flames...
```

---
## \#12 Posted by: Holyman92 Posted at: 2018-07-23T02:16:45.348Z Reads: 107

```
To go without a bms u need a balance charger not a regular charge brick (more expensive)

I would also recommend using a battery monitor like the BM12 pictured below:

![tapatalk_1532312128751|300x177](upload://3UbLS4HYhj2P3J3RSQuvPSnV5ge.jpeg)

That helps you see every S connection and make sure they are discharging evenly
```

---
## \#13 Posted by: Wraith Posted at: 2018-08-10T08:46:32.678Z Reads: 80

```
Would balance charging Li-ions with an external power supply and lipo-balance charger be safer or at least have less room for error when charging?

@mmaner how are you charging up your packs? I am planning to go with a 12s4p 30q with a 12s lipo balance charger that @Hummie will be building along with his deck and enclosure. Trying to understand how you charge the whole thing without a bms/charge port unless going straight up power supply to an xt90 then just checking individual cell voltages like you said.
```

---
## \#14 Posted by: mmaner Posted at: 2018-08-10T11:53:42.962Z Reads: 68

```
Most of my packs have BMS and charge port. I have a 10s3p 30q pack that has no BMS and I charge the pack with a lab power supply. I still have a 6s lipo pack I charge with a MEB (@oriol360) vga port charge adaptor.
```

---
## \#15 Posted by: Hummie Posted at: 2018-08-10T12:43:19.604Z Reads: 59

```
if you look on endless-sphere its very common for people to bulk charge lipos without a bms.   yes it can be very dangerous if a cell goes over 4.2 but YOU become the battery management person and have to make sure that isn't happening.  Ive never heard of a cell that when first put to a charge and showed a good balanced voltage then would later while charging go rogue.    Not that it couldnt happen but I watch for that.  its part of the fun really.

here's an entertaining read about the harbor freight drill and blower that comes with no bms and no way for the user to know whats going on to put things in perspective:
http://www.etotheipiplusone.net/?p=4187
and i know there are a lot of people who make a board with 18650s where they dont know what the cells are doing and they aren't balancing.  i think that is a very bad idea despite harbor freight doing it or anyone else!!

 actually going over 4.2 is not a disaster and done often too.  cells will often drop their voltage within moments once off the charger and people will charge to 4.3 or a bit higher.  and then there's some lithium cells that are intended for charging to a higher voltage.
```

---
## \#16 Posted by: Wraith Posted at: 2018-08-10T12:49:34.445Z Reads: 57

```
Thanks hummie! I’ll look up the link, looks to be quite the interesting read. Though balance charging now a days will cut off and manage the charge right? So if not going with a bms then you could always balance charge it so you can be fairly certain it would cut off at 4.2v? 

Then probably check the packs or cells every now and then?
```

---
## \#17 Posted by: Hummie Posted at: 2018-08-10T13:01:14.891Z Reads: 55

```
i attach the balancer to the (2) 6s balance wires before charging.  just one of those balance chargers is enough and i check the cells then start charging.  while charging leave it on.  you can check both 6s sides moving the balancer to see and you dont even need two of them.   (you can leave them on to see the cell's state and balance at any time though.)   there's much more of a voltage spread when the cells are depleted and then they come together towards full charge.  then it depends if i want to go fully to 4.2 and i need that range, unlikely, or i can just go to 4.1 a cell and maybe 49 volts or even just 48 volts.  pull it from the power supply when i want and ride then.   you could argue this is much better for the cells as youre not having cells sitting around at 4.2 which is more likely with a slow charger where people will leave it for days on the charger maybe and then discharge.   the less time your cells spend at 4.2 ...much better for them.  if you bulk charge you can possibly do the max recommended charge rate.  theres a lot of control with just a bulk charger and dischargers on the side.
```

---

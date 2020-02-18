# First build! Advice wanted

### Replies: 14 Views: 913

## \#1 Posted by: Jaseum Posted at: 2017-06-10T23:42:45.018Z Reads: 101

```
Whats going on everyone? Im sure this is going to be like a broken record, but i'm new to this esk8 thing and i'm not 100% sure on how to do a few things, or what to do i should say.

I'll start with the things I already have.

Torque boards VESC 
Torque boards 6355 190 kv motor
Torque boards motor mount and 36 tooth abec drive system
Caliber ii trucks 50 degree
83mm flywheels
Zealous bearings
Basic longboard deck

What i need and think i still need..

Battery/batteries
Receiver and remote 
power switch/antispark (dont know whats best)
id like some kind of power meter for the batteries but i dont need that right away

i really dont know what i need to do for the batteries and how much my vesc can handle or what. ive never dealt with lipos.  i just need something basic for now to get the thing going. 

i should also mention that im not a small person, big and tall about 270 lbs. the area ill be skating at will mostly be flat with some slight inlines, nothing to crazy.  

Any information will be greatly appreciated! thank you all in advance!
```

---
## \#2 Posted by: Namasaki Posted at: 2017-06-11T00:45:07.701Z Reads: 91

```
For your size and and if your building a single drive, you should get the 6374 motor instead of the 6355 which is great for dual drives but the 6374 is about 1 1/2 times as power full as the 6355.
Also, if you go 90mm wheels with 40T wheel pulleys, you'll have a smoother ride and more ground clearance for your batteries and electronics under the board.
The motor KV should be determined in accordance with the voltage you plan to use.
190KV is good for 10s.
And you probably should go 10s for extra power.
```

---
## \#3 Posted by: Ryel Posted at: 2017-06-11T01:36:13.068Z Reads: 80

```
Could I do a dual 190kv SK3 build with a 10s battery? Would that have a high top speed and/or have the torque to take on hills?
```

---
## \#4 Posted by: Jaseum Posted at: 2017-06-11T02:29:01.982Z Reads: 78

```
could i do 2 5s batteries as apposed to a single 10s?  and will the vesc i have be able to handle that much power? i think it says it has a built in bsc... if thats what its called
```

---
## \#5 Posted by: Namasaki Posted at: 2017-06-11T02:40:14.513Z Reads: 77

```
You can do 2 5s lipos in series to make 10s and the vesc determines how much current is drawn from the battery so the vesc can handle any battery up to 12s.
If you use 2 5s Lipos in series, you'll need at least 5000mah packs to achieve an apx 10-14 mile range which will also depend on your weight, riding conditions and gearing.
And make sure your packs have at least a 25C discharge rating but the higher the C rating the better.
For example, I use 5000mah Lipos with a 60C discharge rating.
You want the battery to be able to handle more amps than the vesc will draw. Leaving plenty of headroom will reduce voltage sag which in turn will improve performance and range.
The vesc does have a built in Bec that supplies 5v for the receiver.
```

---
## \#6 Posted by: Jaseum Posted at: 2017-06-11T02:58:37.735Z Reads: 69

```
so what does the discharge rating do?

and would you recommend doing a bms?
```

---
## \#7 Posted by: Namasaki Posted at: 2017-06-11T03:58:33.206Z Reads: 62

```
The capacity x the C rating = the battery's discharge current
example 5ah x 25C = 125a discharge rate

**Update:**
Note: it has come to my attention that C ratings are being totally blown out of proportion by the battery industry.
so 125a is not the true discharge capability of a 5ah 25C battery.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-06-11T04:03:50.069Z Reads: 61

```
[quote="Jaseum, post:6, topic:25066"]
would you recommend doing a bms?
[/quote]


That depends.  If you want to be able to charge your board without taking the batteries out using a simple brick charger, then you will need an onboard bms.

If you don't mind taking the batteries out to charge them then you can use a hobby balance charger.
I use to have a system with 2 lipos that I removed to charge. I used a dual bank hobby charger and I had a quick access enclosure.
The benefit of this setup was that I had 4 battery sets and could carry extra batteries in my backpack and swap them out while on the road increasing my range 4 times.
```

---
## \#9 Posted by: Jaseum Posted at: 2017-06-11T19:39:38.442Z Reads: 50

```
so i higher discharge rating means its discharges slower or more stable? is that correct?
```

---
## \#10 Posted by: Namasaki Posted at: 2017-06-11T20:14:38.671Z Reads: 51

```
Well, higher discharge rating means  that you will have less voltage sag. So your voltage will be higher when accelerating or going up hills. When the voltage is higher, less amps are required to produce sufficient power because Power in watts is equal to voltage x current.
And the less current you draw form the battery the longer it lasts or the slower it drains.

This is why it's best to build your battery to be more than what is needed. And the more the better.
This is also why I use Lipos and not Li-ions.  With Lipos, you can get more power out of a smaller package
```

---
## \#11 Posted by: Blitz Posted at: 2017-12-06T20:30:17.088Z Reads: 36

```
Would 3  5000mAh 3S1P 20C li-pos battery be good for single motor Want speeds like 34-40 KMH
```

---
## \#12 Posted by: MysticalDork Posted at: 2017-12-06T20:33:02.629Z Reads: 35

```
20c is a little low. I'd go at least 25c. Speed is determined by things other than the battery voltage.

Also, way to necro a thread. Why not just ask in the general chat, or read other build threads, where they have all the info about what they used, and what performance they got.
```

---
## \#13 Posted by: Namasaki Posted at: 2017-12-06T22:31:07.819Z Reads: 30

```
[quote="Blitz, post:11, topic:25066, full:true"]
Would 3  5000mAh 3S1P 20C li-pos battery be good for single motor Want speeds like 34-40 KMH
[/quote]

Sorry for the late reply, just got home from work.
Assuming you mean three 3s in series for 9s.
I think it would be possible to get 34-40kmh with 9s and say a
 200-230kv 6355 motor 
90mm wheels
15/36 pulleys
5000mah would be good for about 10 mile range but I would highly recommend getting a higher C rating 
Actually I use and recommend at least 60C for minimum voltage sag which means better performance and better range.
Also as I stated in my update to the previous post, C ratings are not accurate for measuring real discharge capability.
They are only good as a relative rating.
```

---
## \#14 Posted by: Blitz Posted at: 2017-12-07T09:09:47.255Z Reads: 15

```
OK sorry for bombarding you with questions But i have another one What about these  lithium-ion  battery's 

https://hobbyking.com/en_us/turnigy-icr-18650-10c-2000mah-3-7.html

and then spread them around my deck something like this?
http://www.electric-skateboard.builders/t/building-your-own-36v-8-7ah-lithium-ion-battery-video/62/2
```

---

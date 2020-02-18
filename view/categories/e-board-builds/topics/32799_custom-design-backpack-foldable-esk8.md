# Custom design: Backpack foldable esk8

### Replies: 7 Views: 1062

## \#1 Posted by: spiderdab Posted at: 2017-09-10T16:35:50.116Z Reads: 183

```
Hi, I'm 40, new here, never been on a esk8, but I'm ok in rc, electronics and diy.
What I want to achive is something inspired to this:
https://www.youtube.com/watch?v=PCxSfIVZtao&feature=youtu.be

It should be cheap, and not too powerful, looking to around 10-15 km/h and 10km autonomy, and go over cement and normal uneven streets.
I want to build this upon a IKEA trolley:
<img src="/uploads/db1493/original/3X/7/5/75237ffb77d9db6524e381156d887b27f93852e8.jpg" width="500" height="500">

using a wide truck fixed to the bottom of the bag, and a single e-wheel on the back, so that one could use the handle to help standing while driving.
The board should be kept inside the bag if not riding, and someway mounted in place to ride.

I'm trying to find the right components and I need some help to avoid stupid choices! :sweat_smile:

My known numbers are: front wheels should be something like 80mm-100mm scooter style, mounted on a wide truck to have the wheels outside the trolley-bag.
So maybe wheel like this?
<img src="/uploads/db1493/original/3X/9/a/9aca2fe8c98bb7fcc4aaa360760264de6d541974.png" width="500" height="500">
and this truck:
<img src="/uploads/db1493/original/3X/8/d/8db3208118eba6784f05c49d39f01252306f0f4d.png" width="640" height="500">

this truck is cheap and 15inches wide, which can be ok, but I don't know if I can mount scooter wheels on that. what I read essentially is that it has 10mm axle, so should I change the bearings, or can I find wheels with 10mm bore?

Driving wheel can be smaller, like 80mm maybe.. and the mounting frame will be designed and 3D printed by me.
After that I made my calculations, and found out that with:
driving wheel diameter: 80mm
battery: 6S , 22-24V(I'm still not calculating power..)
ratio: 3:1
motor: 160kv
realistic max speed should be around 15km/h

Do you think a 160kv motor can be a right choice? what should you suggest to change in case?
Thank you for your interest and suggestions.
```

---
## \#2 Posted by: Rinzler Posted at: 2017-09-10T20:26:51.893Z Reads: 121

```
This is a useful tool http://calc.esk8.it/
```

---
## \#3 Posted by: spiderdab Posted at: 2017-09-10T21:45:50.128Z Reads: 116

```
Yes thank you, that tool is well done.
I've made my OpenOffice Calc page to do my calcs, and I have similar results.
But since you can have the same speed whit different configurations, I would like to know what is better to have, higher kv? higher volts? higher Ratio?
thanks.
```

---
## \#4 Posted by: Rinzler Posted at: 2017-09-10T22:20:31.001Z Reads: 101

```
Lover kv motors are more efficient, higher voltage reduces the amps-less heat in all of the electronics.Higher gear ratio means more torque and a cooler motor.All these things are positive, usually one is your compromise and you "fix it" by doing the other two.
```

---
## \#5 Posted by: Rinzler Posted at: 2017-09-10T22:25:22.806Z Reads: 92

```
There is an equilibrium, but you will have to be way more specific about the weight, gradient climbing, budget you have in mind for your board.
```

---
## \#6 Posted by: spiderdab Posted at: 2017-09-11T02:35:07.199Z Reads: 82

```
I'm 85kg. Plus i think 5 kg always inside the backpack.
I'm going to use it in urban situations, like from train station to the hotel or little transferts in the city. I travel a lot for work.
Nothing extreme, but it should be simple to ride. That's why i was thinking about 100mm diameter or similar for the front wheels.
Budget is low. Let's say around 50€ for the motor, what needed for the esc (or vesc?) Few € for the wheels, and what needed for the battery. I already have a charger/balancer for 4s batteries.
I'm going to cut my board from flat plywood, due to the custom shape. And build my custom motor frame.
```

---
## \#7 Posted by: spiderdab Posted at: 2017-10-28T20:29:01.086Z Reads: 60

```
Hi, I've finally built something, but before making a difficoult foldable backpack, i've made a esk8 to understand the electronics.
76mm wheels on a cheap amazon longboard, 1:3,75 ratio (16t / 60t) 3mm htd belt, a ebay cheap mount for a cheap hobbyking KD53-30 190kv motor.
A torque vesc driven by 2*4s 5000mah turnigy lipos in series (8s) turned on by a selfmade mosfet switch.
Remote was made with 2 handmade atmega328 boards comunicating through radio nrf24, following info found on this site, enclosed in a 3d printed handle.
It runs to 21 km/h for about 8 km on a charge, and it's ok for my needs.
I've found an error on the tx/rx code (i've no link now, sorry..) on using the rf24 library, which gave me a lot of transmission errors. Corrected and i've very few errors now. If interested i will give details.
```

---

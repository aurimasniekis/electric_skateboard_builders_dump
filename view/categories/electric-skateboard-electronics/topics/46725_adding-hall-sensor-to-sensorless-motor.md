# Adding hall sensor to sensorless motor

### Replies: 5 Views: 1630

## \#1 Posted by: Winfly Posted at: 2018-02-18T05:21:55.821Z Reads: 210

```
So I bought these Turnigy sk3 5055 280kv way back about 2 years ago. Back when belt and pulleys were the standard. I didn't have much time back then so I never completed my build. Got to get back to this project recently and decided to add hall sensors to this motor just for the heck of it. See picture:
![15189305029171798299889|690x388](upload://qET4Fajsv1FV1Z0m5sHFUGTJxzs.jpg)


There's plenty of space on the inside for wires but there was no room for the hall sensors to sit flat to between the metal thingy (what's the term for it) of the stator. So i had to dremel some corners:
![1518930319035809267144|690x388](upload://e2BVc1XPwwa0NTp4ENGd35tr7BP.jpg)

Got everything wired up and temporarily secured the hall sensors with blue tape. 
![20180217_202826|281x500](upload://4pIQ2vwcDP0te7R7CB1z3t50Dwh.jpg)

I tested my wiring with an arduino and it seems to be working perfectly. 

Now, my questions are:
    1. What epoxy should i use to glue it down?
    2. Do I need the 10k resistors when i plug them to my VESC 4.12? They are A3144 hall sensors.
    3. Was it worth it? Idk how necessary I need the sensors but I was thinking why not. What can I get out of these sensors? 
    4. Can I run FOC on these? Afaik, its kinda skeptical to run FOC on the VESC 4.12. Or was that only for 12s setup.

P.S. I am planing to do 10s3p with my bulk sanyo 2200mAh 20A batteries. I am basically doing most of the work myself: Battery Pack, nRF controller, enclosure, etc. 

I have bought most of my parts already but I figure I can do another post when I get more progress.
```

---
## \#2 Posted by: Josiahreece Posted at: 2018-06-26T14:11:32.426Z Reads: 136

```
Did you get success with the sensors?
How did you wore it to work with a vesc?
```

---
## \#3 Posted by: Winfly Posted at: 2018-06-26T22:53:40.464Z Reads: 130

```
Didn't put much work into completing the motor. But I will wrap this up once I'm done with vacuum forming an enclosure for the Hummie wood carbon deck. I'll probably make an update after that.
```

---
## \#4 Posted by: Cobber Posted at: 2018-06-27T04:32:52.799Z Reads: 121

```
I'd go with a encoder chip

I got one for my mountain board from e-toxx

http://www.electric-skateboard.builders/t/my-vesc-with-as5047-sensor-setup/6568
```

---
## \#5 Posted by: Holyman92 Posted at: 2018-06-27T07:44:49.630Z Reads: 97

```
APS sells pcbs in 42, 50, 63, 80, 120 mm sizes, u just epoxy in place and voila, u have a sensored motor.

https://alienpowersystem.com/shop/brushless-motors/50mm/internal-pcb-with-hall-effect-sensors-120-degree/
```

---

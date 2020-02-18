# Confirmation on electric parts build

### Replies: 8 Views: 578

## \#1 Posted by: TehAtheist Posted at: 2017-06-05T08:48:15.672Z Reads: 78

```
Before buying my parts I'd like to have it confirmed to work properly by some more experienced builders.

**Requirement:**

*  **Real Max Speed:** 30 km/h (Higher is not a problem obviously, but definitely not necessary)
* **Range: 15 km** (idem dito)

* **Power:** Should be able to get on hills rather decently
(No idea what the incline is, but going on them with a bicycle is annoying and quite exhausting.)
* **Acceleration:** Decent, as my city will require lots of starting and stopping.

**Current build (electrical):**

* **Motor:** SK3 6364 245kv (€63)
* **Battery:** ZOP 6S 8000mah (€52)
* **BMS:** 12A 6S BMS China (€11)
* **ESC:** MayTech VESC (€99)
* **Transmitter/Receiver:** Nano remote 2.4Ghz "award winning" (€34)

The main question is: Is this decent & will this perform how I want it to? I believe after some reading that my kV is rather high, is this correct? If I'd lower the kv and up the voltage, will this result in more torque and acceleration?

Thanks in advance!
```

---
## \#2 Posted by: astread Posted at: 2017-06-05T09:15:41.833Z Reads: 71

```
calc.esk8.it/ this should give you an estimate
```

---
## \#3 Posted by: TehAtheist Posted at: 2017-06-05T09:22:54.355Z Reads: 70

```
I've used that website to determine these specs :slight_smile:.
That's why I'm hoping some people may know if this setup will perform like I want to, I have no idea how this would perform on hills etc. That's information a calculator cannot give me. But thanks!
```

---
## \#4 Posted by: Rory Posted at: 2017-06-05T09:35:06.031Z Reads: 68

```
I'm also trying to do a similar build as my area is quite hilly and from reading through the forum I have decided to use 8S with a 190Kv motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html?___store=en_us 
I believe this will be significantly increase your torque for those hills whilst still being able to go around 30km/h however I'm not an experienced builder so please correct me if I am wrong.
```

---
## \#5 Posted by: Rinzler Posted at: 2017-06-05T13:42:33.998Z Reads: 52

```
The VESC has a safe amp rating of 50A, on a full 6s lipo that would give you 1260w of power with **a lot of heat** because it is using a lot of amps.You would be stressing the vesc a lot with your amps.On the other hand if you would use 10s lipo for the same wattage you would use 30A and it will be a lot cooler running drive train motor and esc.If you decide to go the 6s+ voltage way you have to be careful not to overpass the vesc ERPM limit with the kv of your motor. If you ask me running a vesc on 6s is wasted potential, up the voltage.On 6s i would go with a car esc but that depends on your decision and if the smooth ride and features of the vesc are important to you.
```

---
## \#6 Posted by: TehAtheist Posted at: 2017-06-05T20:31:38.616Z Reads: 38

```
Thank you for your reply, exactly the thinking about my build that I needed!
You're right, it seems wasted potential. If I can get that current to 50% my losses in the VESC would decrease to 25%, which is a great thing. I feel stupid for not thinking about it ;).

I've taken these things into consideration and will most likely change to a setup with 10S & 190kV, having better torque for the hills in my city.

@Rinzler Do you think that  5000mah 5s x 2 for a 10s setup will have a decent range or should I opt for a 8s 10000mah setup?
```

---
## \#7 Posted by: Rinzler Posted at: 2017-06-06T01:05:49.094Z Reads: 31

```
Range depends on the total energy your battery has, it is measured in watt hours.The 10s lipo 185Wh divide by 9-12wh per km and you get your range, simple :sweat_smile: .The 8s one is 296 Wh also divide by 9 or 12 to get your range in km.The Wh per km depends on your riding style, weight, surface, hills ect. :wink:
```

---
## \#8 Posted by: saul Posted at: 2017-06-06T03:17:44.961Z Reads: 29

```
[quote="TehAtheist, post:6, topic:24599"]
Do you think that  5000mah 5s x 2 for a 10s setup will have a decent range or should I opt for a 8s 10000mah setup?
[/quote]

I have a board that has split personalities. sometimes its 8s245. others 10s200kv.
with the same wheels/gearing. top speed is the same. hills about the same. noise is louder on 245kv.
and the 8s also needs higher current settings.

the real difference is in the acceleration. the 8s has more on the topend. but the 190/200kv kicks hard off the line.
```

---

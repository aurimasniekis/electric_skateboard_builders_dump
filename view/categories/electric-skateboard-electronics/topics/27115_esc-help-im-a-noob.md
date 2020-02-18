# ESC Help, I&rsquo;m a noob

### Replies: 6 Views: 748

## \#1 Posted by: FMS Posted at: 2017-07-09T02:20:33.446Z Reads: 54

```
What is the difference between an ESC like this:https://hobbyking.com/en_us/hobbyking-red-brick-125a-esc-opto-version-11.html?___store=en_us

and one like this:
diy-electric-skateboard-kits-parts/single-motor-120a-6s-esc/

Why is 1 more than double the cost of the other?
They both can handle ~120 A and 6s voltage but to me(A noob) all I need is something that can control speed, work with 6s and handle 80A continuous.

Side question, is the electricity generated from the motors when going downhill or coasting a problem? The last thing I want is a battery fire or fried electronics mid-ride.

Side question #2, Is the white red and black cable coming from the ESC a pwm cable? might be obvious but not worth the risk of ending up with very expensive paperweights.
```

---
## \#2 Posted by: JdogAwesome Posted at: 2017-07-09T02:30:41.742Z Reads: 52

```
That HobbyKing Red brick is interesting, never seen it before though I'd probably steer clear of it because it doesnt have an integrated fan and just seems to good to be true. You could go with the Torqueboards 120A ESC but I cant recommend the VESC enough. I originally started with a car ESC because I was trying to be as cheap as humanly possible, worst mistake of my life. Only ended up spending more money in the long run lol, anyways the VESC is better in so many ways and so worth. I think the biggest thing for me has been the WAY better braking. Before the braking with a car ESC was terrible and really dangerous, the VESC does a great job with it though.  

Side Question #1 No thats just regenerative braking and your batterys and ESC can handle it, otherwise they'd just die the second you started coasting. 

Side Question #2 Yes thats the PPM connection for the ESC, usually just connectors to your receiver like a GT2B or whatever.
```

---
## \#3 Posted by: FMS Posted at: 2017-07-09T02:47:16.131Z Reads: 41

```
What features does a VESC have over a normal ESC? I'm going the connect the ESCs to a computer like a raspberry pie or arduino. One thing I really want is a "smart board" as opposed to a reciver connected to a VESC. When you say dangerous, what exactly do you mean? For breaking I was just thinking of telling the motors to go backwards. Could that draw a bunch of torque and end up burning out the motor? How does a VESC handle breaking? Sorry if these sound like basic questions I could find if I used the search bar and looked harder.
```

---
## \#4 Posted by: JdogAwesome Posted at: 2017-07-09T02:52:17.603Z Reads: 42

```
[quote="FMS, post:3, topic:27115"]
What features does a VESC have over a normal ESC?
[/quote]
So many. First of all its totally customizable, in that you can change it to ride the way you want it to. You can limit battery current and rpm as well as a bunch of other stuff. I recommend you look up some more info on the VESC itself. 

[quote="FMS, post:3, topic:27115"]
When you say dangerous, what exactly do you mean? For breaking I was just thinking of telling the motors to go backwards.
[/quote]

What I mean by that is when im riding and I want to slow down the car ESC brakes, but it does so very slowly. Thats just because its a car ESC, not an electric skateboard ESC carrying a 130lbs person instead of a 10 pound car, it doesnt know how to stop a motor of that size properly. And by dangerous I mean well if you were in a car and you had really shitty brakes and couldnt stop coming to an intersection, I think that'd be pretty dangerous lol.
```

---
## \#5 Posted by: FMS Posted at: 2017-07-09T02:57:58.956Z Reads: 39

```
So I did some more reading on VESCs and it seems like I can add them myself if I add the right sensors and program it myself in the main computer. I might be wrong since I'm pretty new to this.
```

---
## \#6 Posted by: JdogAwesome Posted at: 2017-07-09T03:02:43.152Z Reads: 37

```
[quote="FMS, post:5, topic:27115"]
and it seems like I can add them myself if I add the right sensors and program it myself in the main computer.
[/quote]

Not sure what you mean exactly. Do you mean add the features of the VESC to the Torqueboards 120A car ESC? If so then yes I guess you could but t would be a great deal of effort and consume a lot of time. It would also probably never wok as well as the VESC which has been in development and use for years.
```

---

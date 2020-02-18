# Theorizing an Electric Motorcycle?

### Replies: 13 Views: 272

## \#1 Posted by: devilzangelz Posted at: 2019-05-14T05:17:30.570Z Reads: 136

```
I can't find anything posted on the forum, but has anyone tried an electric "motorcycle"? I have seen some ideas online using forklift motors and such, but nothing here. It ideally would be something slightly beefier than a standard electric bike, maybe say 60mph+? I've joked with a few people and it seems "feasible" under some conditions, but I would like some additional opinions to see if I am missing something!

Looking for a fun summer project for some of my engineering buddies and I. I haven't put a lot of thought into it, but the best projects start with limited planning (or something) haha

Potential components (subject to change a lot):
* [Batteries](https://hobbyking.com/en_us/turnigy-graphene-5000mah-4s-75c-lipo-pack-w-xt90.html) - with a decent discharge (claimed 75C continuous and 150C peak) (series/parallel configuration will depend on the ESC chosen)
* [800kV Motors](https://nl.aliexpress.com/i/32861750710.html) - seem to claim pretty good performance.
*  [Motor controller](https://flipsky.net/collections/electronic-products/products/high-current-fsesc-200a-60v-base-on-vesc6) - might need to go custom? 

Some less specific components:
* ~ 26" diameter Wheels
* Generic bike frame (with reinforcements)
* Geared for torque at nearly 30 to 1 (maybe higher)?
* Controller - some modified pull throttle such as the [Mini Remote](https://buildkitboards.com/collections/remotes/products/mini-remote) but in a more ergonomic shape for the handlebars. Alternatively something hardwired instead of wireless?

Some things that I still question:

* Would the battery be too much for the original ESC? I can't seem to find any that will go over 200A...
  * I did some reading a while back and I seem to recall 5mA = 5Amps. 5Amps * 75 C = 375Amps continuous, but that seems exuberantly high. Is there a more accurate way to convert the C rating to continuous amps? Seems like I am getting pretty far from the electric skateboard market with some of the ESCs I have researched.
* Seems like I would need a really high gear ratio to get any torque out of the motor at all. That being said, most [online calculators](https://calc.3dservisas.eu/?PY_BCsIwEET_JWeRNDatek2lJyUQsHfNoYKhgR7Ff3dnknp7MzuZzX7Uw83qrN6vvKidiJuIw74XXl0QbgzRC7Ykh4DVmmKAamxhZEzx2dkI5lAfZiTlGebZwzUkvwVZ1VsiTcvov-k5czPpInTUxDuaWnByNZkCx_T8ItyReEz5QHLLdlqcViQ62HG81oo4TlhGE8tOWn1_) theorize ~50-60mph at a 30:1 gear ratio. Given that I don't know how much the overall construct would weigh, or the mass of the rider(s), is there a way to find how much torque would in theory be required? 
* Charging hasn't been considered yet
* Battery size has not been considered yet (series/parallelly speaking) since too low of a series count will limit some of the ESCs. It may be better to go with a battery with a lower C rating? It seems like a LiPo setup will be better for this application.

There are definitely some additional things to consider. Any insight would be greatly appreciated! :)
```

---
## \#2 Posted by: pakue Posted at: 2019-05-14T05:26:51.830Z Reads: 123

```
I think most electric motorcycles use induction motors for their better efficiency at larger sizes.
Here is a project from a Germany university: https://www.gauss-project.com/project.htm 

At some point they even had regenerative breaking in the front wheel.
```

---
## \#3 Posted by: Vanarian Posted at: 2019-05-14T05:30:15.195Z Reads: 124

```
That's a nice and long project of you wanna build one ! If you want more ideas and parts options, check out Endless-sphere.com ✌🏽 lots of options and builds from e bike to e trike to e motorcycle. There are dragsters disguised as sheep out there !

You can start from a salvaged Moongoose cx450 and rebuild from there for example, it packs a motocross look with a solid steel frame.
```

---
## \#4 Posted by: devilzangelz Posted at: 2019-05-14T05:30:57.384Z Reads: 117

```
I will definitely have to read further into currently existing electric motorcycle technology!

From what I have seen so far, most people who make DIY electric motorcycles use Brushless DC motors, permanent magnet DC motors, or induction motors, but I have only searched for a few hours.

Thanks!
```

---
## \#5 Posted by: devilzangelz Posted at: 2019-05-14T05:31:46.230Z Reads: 112

```
Sure thing - I stumbled on the forum during a few of my searches. Might have to setup an account and ask around there for additional guidance.

Also was tempted to build a ground up frame or use a bmx/mountain bike for the frame and expand off that. But I did consider picking up a junker (seized engine or something) and converting it. Not sure what would be more of a hassle haha 

Thanks!
```

---
## \#6 Posted by: linsus Posted at: 2019-05-14T07:24:39.778Z Reads: 88

```
you didint specify what kW you're aiming for but anything from 15-30kW should be enough on a lighter MC.
https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26293.html

^ is a safe bet for a motorcontroller.

I've had the same idea brewing for a long time, I dont have a driverslicence for an MC however so should prob focus on that first :smile:

Second part is how you get it roadlegal. It's abit of a hassle here (Sweden), especially if you need to do any welding modifications. But I reckon getting a veteran bike and stripping it down and using the standard supports to build around would be the easiest. Its hard to get around the fact that you need a real strong motor mount, that'd have to be inspected and approved etc. 

I still think all this would be cheaper then buying the new harley electric MC :wink:
```

---
## \#7 Posted by: Leonhart Posted at: 2019-05-14T08:58:18.836Z Reads: 66

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#8 Posted by: devilzangelz Posted at: 2019-05-14T15:53:43.089Z Reads: 52

```
The motor is claiming around 12000W of power, so a bit less than your recommended.

The VESC you mentioned is indeed pretty substantial, but it is for 3 motors. Albeit not a bad thing, but I only really intend to use 1, maybe 2. I had looked into the other options they have (for single motors) and they just don't seem as capable in regards to current.

I have looked into road legality slightly. Here in America things are likely different. It definitely seems like picking up an existing bike and modifying it will be the easier way to go, especially if we want to get this done in a reasonable amount of time haha

Thanks for your insights!
```

---
## \#9 Posted by: olsonjus Posted at: 2019-05-14T16:32:00.252Z Reads: 42

```
This is the way to go for electric bike controllers:

http://accelerated-systems.com/powerful-electric-alternatives/products/
```

---
## \#10 Posted by: Der6FingerJo Posted at: 2019-05-14T16:36:19.217Z Reads: 40

```
Well, if you're serious about motorcycles you should check out Motenergy Motors, like the ME1507 and Sevcon controls. Or a really really beefy VESC. 

Then again, your plans sound like a really beefed up ebike, which is probably way more efficient to build and research than an  actual motorcycle.
```

---
## \#11 Posted by: linsus Posted at: 2019-05-14T16:37:48.107Z Reads: 36

```
Its not for 3 motors, for one. More cables to support amp draw.
```

---
## \#12 Posted by: Battosaii Posted at: 2019-05-14T16:40:08.964Z Reads: 34

```
Yea its for one motor they went with smaller wires in paralell other than using a thick wire cause its easier to bend and handle smaller wires in an enclosure.
```

---
## \#13 Posted by: MD84 Posted at: 2019-05-14T16:58:39.392Z Reads: 31

```
You could buy a cheap or used pit bike and convert it
```

---

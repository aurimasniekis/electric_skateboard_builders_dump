# Brake lights, what do people know of these?

### Replies: 22 Views: 447

## \#1 Posted by: Ineedspeed Posted at: 2019-08-25T01:53:00.538Z Reads: 164

```
Looking for full functionality brake lights that brighten when actually pulling throttle back...  the brightness will be insufficient for improving vision for the rider moving forward but for a break light to help with safety behind u I think it would do quite nicely....  what do people think??

https://eskating.eu/product/6w-waterproof-led-light-kit-with-rear-brakes-control/
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-08-25T02:02:52.552Z Reads: 153

```
I haven't used that kit, but I built a similar setup from scratch on my last board. High/low beams in front, and tail/brake lights in back, all controlled by the remote. (You need an aux channel for the high/low beams.) Worked like a charm.
```

---
## \#3 Posted by: Grozniy Posted at: 2019-08-25T04:16:57.260Z Reads: 138

```
What I use
€ 7,68  43%OFF | Xlite100 Usb Bike Tail Light lantern Smart Brake Sensor Taillights MTB Road Cycle Rear Led Waterproof Bycicle Back Lights
https://s.click.aliexpress.com/e/4sZzOYg0
```

---
## \#4 Posted by: Ineedspeed Posted at: 2019-08-25T06:44:40.983Z Reads: 122

```
Ya but like why?  I was bringing this one to light cuz it actually functions like a brake light is suppose to, getting brighter as u go slower so cars are aware of your adjustment, which can be hard for cars to recognize in the dark.  Keep them RearEnders away from ending your eskate career.   That bike light, what does it do that makes it smart other than turn on and off on its own?  Sounded rude but I don’t read Chinese so I couldn’t tell what all the captions in the video said....   I just really like the idea of making an eskate a formidable form of reliable safe transportation, and functional brake lights controlled by your remote is definitely a feature bringing us a bit closer to mainstream...
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-08-25T08:00:58.279Z Reads: 110

```
@Ineedspeed I'd guess it has an accelerometer in it that can tell when the vehicle it's attached to is decelerating. Given how vibration-heavy an esk8 is, it doesn't sound like a very good idea. Let me know if you're interested in building your own lights system - I can share the source code and parts I used.
```

---
## \#6 Posted by: b264 Posted at: 2019-08-25T08:31:25.715Z Reads: 99

```
I would not use that vendor.
```

---
## \#7 Posted by: Ineedspeed Posted at: 2019-08-25T08:41:26.002Z Reads: 94

```
The original light post I made correct? Euskate...com whatever it is.    Why is that?  Faulty experiences with them?
```

---
## \#8 Posted by: Ineedspeed Posted at: 2019-08-25T08:45:27.628Z Reads: 90

```
I would love to, I have zero experience building anything like that before.  I’m preparing for my second build coming up so no electrical work other than really minor soldering...   are there kits or anyone that sells functional pre assembled systems similar to this?  Really like the idea of power on off by remote and a fully functional brake light that runs like a cars would. always when braking and when lights are on solid red on cruise and bright when braking.....
```

---
## \#9 Posted by: b264 Posted at: 2019-08-25T08:46:26.076Z Reads: 87

```
Yeah the euskate place.  If you want customer service, try elsewhere.  Or maybe ask around on the new builders forum.  Most of the cutting-edge innovation is happening over there.
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-08-25T08:50:17.443Z Reads: 83

```
I don't know of any versions other than the euskate one. The electrical design is pretty simple and it wouldn't be too big of a deal to put together a basic kit. It's basically a little microcontroller, an LED driver, an LED, a switch, and some wires/plugs - pretty basic really. The microcontroller gets its power from the vesc, and the LED driver runs straight from the battery.

No difficult soldering or coding required - just some wires, and a basic install of the code with the arduino IDE.
```

---
## \#11 Posted by: Ineedspeed Posted at: 2019-08-25T09:06:31.882Z Reads: 78

```
I can definitely do that.  Will that have a functional break-light as opposed to just plain flat tail lights?   Also do you have any knowledge of how to be able to control the power of the lights by remote (feather or something like that)?
```

---
## \#12 Posted by: Ineedspeed Posted at: 2019-08-25T09:07:25.650Z Reads: 74

```
Disregard.  I see you already said remote controlled...
```

---
## \#13 Posted by: MysticalDork Posted at: 2019-08-25T09:08:15.206Z Reads: 71

```
Yes to the brake lights. On-off control will depend on whether the remote you're using has a second PPM channel - I was using a GT2b which had a wheel on channel 2 (unused) and an aux button that toggled channel 3. I used ch3 to control hi/low headlights, but it could easily be adapted to just turn off the tail lights.
```

---
## \#14 Posted by: MysticalDork Posted at: 2019-08-25T09:16:31.253Z Reads: 74

```
I just had a button on the bottom of the board for lights on/off, and controls for the lights *while on* were on the remote but to turn them off you had to stop and pick up the board.

You could always put the button on top of the board for easy access though.
```

---
## \#15 Posted by: esk8jpn Posted at: 2019-08-25T09:46:42.232Z Reads: 75

```
I use it.  To be honest, the exterior is a rough 3D print, so it may break.  I reinforced with acrylic glue.
https://www.instagram.com/p/BwwUr9uhqve/
It works properly with the brake. I like it.
```

---
## \#16 Posted by: evoheyax Posted at: 2019-08-25T13:05:24.840Z Reads: 70

```
Just to make sure everyone understands how these lights all work.

When going 30 mph, you are traveling 44 feet per second. That's 132 feet in 3 seconds, which is the minimum amount of time you need to react and actually do something besides falling.

That means if you can't see over 100 feet ahead of you, the light is not doing it's job.

Now you could say well, "I only ride at 15 mph". And in that case, your still traveling 22 feet per second. That's 66 feet in 3 seconds, That's around 4 cars in length.


**My whole points:**
Anything in that 250w or 500w range is just too weak to really light up more that a few feet in front of you.

These lights are great if your only goal is to be seen, as you will be seen. But they are not going to let you safely operate in pitch black or very dark areas. You need overhead street lights and even then, you won't get great detail 60+ feet down the road.

I have used 2000 lumen lights on my eboard that did light up the road enough to see 3+ seconds ahead. These are not nearly that bright.
```

---
## \#17 Posted by: Jamie42 Posted at: 2019-08-25T16:35:45.418Z Reads: 67

```
Which forum do you mean?
```

---
## \#18 Posted by: Lazea01 Posted at: 2019-08-25T16:54:28.345Z Reads: 66

```
https://forum./
```

---
## \#19 Posted by: MysticalDork Posted at: 2019-08-25T21:03:13.198Z Reads: 62

```
We're mainly talking about tail lights here. You know, the ones behind you, that you don't see by? 

And the lights on my last build were roughly 1w of red in the back and 8.5w of white in the front focused through a nice elliptical pattern TIR optic for around 800 lumens out the front - plenty to see and be seen. (they were obnoxiously bright to oncoming vehicles, I admit. Couldn't get a proper horizon cutoff using stock optics.)
```

---
## \#20 Posted by: evoheyax Posted at: 2019-09-14T05:11:48.138Z Reads: 39

```
I've ignored this post for a while cause you seem pretty condescending and confrontational. All I was doing was bringing some math in to provide information for those who care about actual math.

The link you posted was a kit for both the brake lights and headlights, thus why I mentioned about headlights.

[quote="MysticalDork, post:19, topic:100820"]
We’re mainly talking about tail lights here. You know, the ones behind you, that you don’t see by?
[/quote]

There's no need for this kind of response. Your acting like a child.

As for your claim that 800 lumens is bright enough, it really depends on your speed again and how much you want to light up. if you want to see 132 feet ahead of you (as that's 3 seconds ahead at 30mph), you will be visible with 800 lumens, but you will not be able to see a small pothole or some big stones or a big crack 132ft ahead of you with 800 lumens. You just won't get enough detail. You may be able to see where your going, but if you live in a city where the streets are not nice, your not going to be able to see enough.

I run 4000 lumens on my ebike, which is ideal to see 100+ ft ahead. And that is with a better angle. Because we mount lights super low on an eskate, the angle makes it even harder to project far ahead. You can use a focuser, but your fighting trigonometry here.
```

---
## \#21 Posted by: Darkie02 Posted at: 2019-09-14T08:13:37.582Z Reads: 30

```
My issue is that system only runs on PPM. Most remote are now useing the more reliable UTAR 

Only option iv come acros so fare is

https://www.electric-skateboard.builders/t/teltail-lights-ttl-interactive-eskate-lighting-system/86912

Hoping @Ricco will fined some time to possibly build a light version for the tail light so it can be used with the new generation of remotes coming out.
```

---
## \#22 Posted by: visnu777 Posted at: 2019-09-14T09:17:49.719Z Reads: 29

```
I did something like that recently: https://forum./t/grunstern-mov-e-shortboard-12s3p-nese-hummie-hubs-hammock-baseplates/2409/144

Only an Arduino Nano and short piece of LED strip needed, connects to UART of the VESC and reacts to throttle.
```

---

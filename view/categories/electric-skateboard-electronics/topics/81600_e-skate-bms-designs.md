# E-Skate BMS Designs

### Replies: 28 Views: 1020

## \#1 Posted by: Andy87 Posted at: 2019-01-21T11:50:46.986Z Reads: 230

```
This one is for @dannychan as he can´t create his own topic.
Here you go!
Tell us more about your plans ;)
```

---
## \#2 Posted by: Jc06505n Posted at: 2019-01-21T12:43:47.567Z Reads: 221

```
Awesome! I emailed them around 3AM in the morning in a *very* long winded letter for them to join the forum after a few days of researching their BMS. 

They’re been pretty active on the Endless Sphere Forum engaging with the Ebike community and taking their feedback: 

https://endless-sphere.com/forums/viewtopic.php?f=14&t=73354

https://endless-sphere.com/forums/viewtopic.php?f=3&t=22919

https://www.speedict.com

Right now the forum is still searching for a reliable and compact way of monitoring and balancing cell packs: 

https://www.electric-skateboard.builders/t/monitoring-individual-cell-voltages/80340?u=jc06505n

I believe , with some community input the Neptune 15 can be it. 

Now for my US brethren waking up please **play nice**

Thank you @dannychan for heading my advice. 

 @Adstars you’re the only one in the forum at the moment that has a Neptune 15, how do you like it? How’s the app? The Balancing ?
```

---
## \#3 Posted by: Adstars Posted at: 2019-01-21T16:09:26.243Z Reads: 180

```
Not yet tested it, 

The cells are almost ready to hook up.

I’m off on holiday for a week so will update you when I return. Good to see Speedict on the forum. Welcome @dannychan

I’ll be putting the Neptune through a few stress tests shortly. Ease it in with 3amp charging, moving up to a fast 10amp charger. Video review and feedback to follow.

The app looks promising and it will be nice to keep a close eye on the individual cells. 

The build will also include new tech from maytech, their new waterproof remote. I’m also planing to integrate a wireless charge transmitter into the build for this remote. @EileenMaytech.
```

---
## \#4 Posted by: akhlut Posted at: 2019-01-21T16:22:30.306Z Reads: 173

```
Ok, this looks promising.  

Subbed!

Peak discharge = 60A

@dannychan bypass ok?
```

---
## \#5 Posted by: banjaxxed Posted at: 2019-01-21T17:23:29.859Z Reads: 169

```
Hi @dannychan, thanks for joining!

In the muddle of a 13s build, I’ve moved from one cheap bms to another, discharge only of course 

https://www.electric-skateboard.builders/t/selkie-haya-deck-hummie-hubs-13s-proton/78254/18?u=

Can the Neptune 15 cater for any voltage 12s-15s depending on connected balance leads?

I’ve been trying to not buy one!
```

---
## \#6 Posted by: Indiangummy Posted at: 2019-01-21T17:25:37.185Z Reads: 164

```
Yes it can, they sell adapters.
```

---
## \#7 Posted by: akhlut Posted at: 2019-01-21T18:08:12.315Z Reads: 159

```
It's all in the balance lead wiring.  check the PDF.

https://drive.google.com/file/d/1QbI5GLSYC-aGV3IZZKtiuMf3rk_v9MjC/view

![image|690x279](upload://5WzabqyFgxYWDAlxZd4dxEa9WYf.png)
```

---
## \#8 Posted by: janpom Posted at: 2019-01-21T19:56:01.231Z Reads: 156

```
@dannychan I looked at the products you offer and I really like the features and the polishing on both the hardware and the mobile app. I'm particularly interested in the Neptune Lite. A few questions:

You mentioned in the thread on endless sphere that you don't want to focus on iOS. I believe that was some 2 years ago. Has anything changed in that respect?

Have you considered documenting the communication protocol to allow third party solutions for iOS or even for devices other than mobile phones, e.g. custom gadgets with bluetooth and display?

In the Android app, I can see you can set the maximal cell voltage and get a visual indication if it's exceeded. Is there a sound alarm as well? That would be very handy to know that it's time to disconnect the charger since the Neptune Lite is a monitor only and doesn't control the charger.

I believe that a BMS that people here would love would be something inbetween the Neptune Lite and the Neptune 15. One that monitors the cells and has charge control as well and yet is much smaller than the Neptune 15. The smaller size could be achieved by leaving out the discharge control circuitry.
```

---
## \#9 Posted by: Jc06505n Posted at: 2019-01-22T03:01:30.094Z Reads: 132

```
[quote="janpom, post:8, topic:81600"]
Have you considered documenting the communication protocol to allow third party solutions for iOS or even for devices other than mobile phones, e.g. custom gadgets with bluetooth and display?
[/quote]

This , when I was looking over the Endless Sphere forum i thought about how creating at least an API would allow people like @rpasichnyk (though it would probably only work by switching the Bluetooth module) and @Deodand to tailor their software applications to suite the Neptune 15. 

Imagine loading up the VESC tool and having it connect to the BMS module to see pack voltages while knowing your not compromising much on space.
```

---
## \#10 Posted by: banjaxxed Posted at: 2019-01-22T09:50:38.583Z Reads: 120

```
Also interested in any iOS plans, iPhone user

I'd buy the Lite too if I had an Android device, but can't justify without
```

---
## \#11 Posted by: Friskies Posted at: 2019-01-22T10:28:14.515Z Reads: 118

```
If you make an API that @rpasichnyk could potentially integrate into metr; I would buy it instantly.
```

---
## \#12 Posted by: dannychan Posted at: 2019-01-22T12:38:00.066Z Reads: 106

```
yes it can bypass discharge circuit by connect discharge wire to loading directly, and charger connect to neptune's charger wires
```

---
## \#13 Posted by: dannychan Posted at: 2019-01-22T12:47:44.555Z Reads: 106

```
we would like to spend time and effort on next coming model MERCURY 15, therefore we don't have schedule for iOS app as well as open API for further development, sorry about that. 

add alarm or buzzer to neptune lite is easy but take out discharge circuit on neptune 15 can not save some space because most of the space is occupied by balancing circuit.
```

---
## \#14 Posted by: Jc06505n Posted at: 2019-01-22T12:55:28.695Z Reads: 107

```
[quote="dannychan, post:13, topic:81600"]
we would like to spend time and effort on next coming model MERCURY 15,
[/quote]

What is the Mercury 15? Is it a BMS as well?
```

---
## \#15 Posted by: Vanarian Posted at: 2019-01-22T13:01:29.175Z Reads: 105

```
Yes looks like it from website ! Pretty cool HW. Welcome @dannychan !
```

---
## \#16 Posted by: dannychan Posted at: 2019-01-22T13:12:11.995Z Reads: 106

```
BMS + speed regulation 

https://www.youtube.com/watch?v=illTs_WQnNs&t=48s
```

---
## \#17 Posted by: banjaxxed Posted at: 2019-01-22T13:35:34.086Z Reads: 103

```
[quote="Jc06505n, post:14, topic:81600"]
Mercury 15
[/quote]

Weird, I can only find references to a model by this name released in 2012!
```

---
## \#18 Posted by: janpom Posted at: 2019-01-22T13:39:34.474Z Reads: 103

```
[quote="dannychan, post:13, topic:81600"]
we would like to spend time and effort on next coming model MERCURY 15, therefore we don’t have schedule for iOS app as well as open API for further development, sorry about that.
[/quote]

Thanks for the answer. I understand that you have other priorities than iOS. As for the open API, I suppose that documenting it is a pretty simple task that could be done in a day or so. I guess it's rather the question of whether you want to allow third party solutions or you prefer to deliver your own. I believe that opening the ground for third parties could be beneficial for you.
```

---
## \#19 Posted by: dannychan Posted at: 2019-01-22T13:39:44.983Z Reads: 99

```
that's obsoleted, the new Mercury has combine BSM with output control
```

---
## \#20 Posted by: dannychan Posted at: 2019-01-22T13:42:51.491Z Reads: 99

```
the problem is we don't have API, the client and hardware connect and handshake is hardcoded unless we've change our code.
```

---
## \#21 Posted by: janpom Posted at: 2019-01-22T16:38:52.210Z Reads: 95

```
I'm sorry but that doesn't make sense. There must be a communication protocol that the BMS and the mobile device use to exchange information. It may be messy; it may be difficult to explain or document, but I can't see how it could be "hardcoded".
```

---
## \#22 Posted by: Jc06505n Posted at: 2019-01-28T03:45:41.758Z Reads: 85

```
I’m expecting my 11s battery pack to become unbalanced in the foreseeable future and when that happens I’m thinking of converting to the Neptune 15 since it’s a similar size. 

Questions: 

Are the speed and temp sensors necessary ? 

I think most people would like if the BMS stayed as a BMS and only did stuff relating to the battery. Temperature wise , we never really worry about the temp of the batteries (more so our motors) and use the motor sensors to get info about motor temp. Same thing Speed wise as we limit our ERPM and other settings. 

Would it be possible to have a discounted price group buy for the Neptune 15? I’m sure with a discounted price and pending testimony from @Adstars , we would be willing to buy
```

---
## \#23 Posted by: Pedrodemio Posted at: 2019-01-28T04:00:30.788Z Reads: 85

```
@dannychan I’ve been following the Neptune for some time

My suggestions for a ESK8 version

* as compact as possible 
* ditch all discharge controls and maybe even current sensing, integrate everything with VESC via CAN bus, more on the next point 
* no Bluetooth, focus on CAN communication and firmware integration, most boards already have a Bluetooth module from @rpasichnyk and that already proved to work really well with a BMS, all done via CAN

Looking forward for what comes from this

The truth is that there is no good choice for BMS, we have one or other amazing designs, but they are just too big, meaning on most builds sacrificing significantly battery capacity, or they are dumb BMS’s that most of times are cheap and of doubtful quality
```

---
## \#24 Posted by: banjaxxed Posted at: 2019-01-28T08:22:34.105Z Reads: 74

```
Like Meatloaf says, I'd do anything for love, but I won't do that.

iOS non-fanboy, just cannot be bothered going to time/trouble/money. Even a desktop app to connect would be fine.
```

---
## \#25 Posted by: Komamtb Posted at: 2019-02-03T20:08:49.150Z Reads: 64

```
I would love to not have to bypass a bms, and I like this litlle thing, but 60 will not cut it.
```

---
## \#26 Posted by: conquerco Posted at: 2019-05-27T15:49:37.064Z Reads: 48

```
Im looking at the site but having trouble understanding what the Neptune 15 has that the Lite doesnt. What am I missing?
```

---
## \#27 Posted by: banjaxxed Posted at: 2019-05-27T16:04:06.939Z Reads: 46

```
The website has poor product detail for the lite version, I would imagine it’s discharge current is lower but you’d have to download the user guide and give it a detailed read/compare
```

---
## \#28 Posted by: Jc06505n Posted at: 2019-05-27T16:35:52.778Z Reads: 44

```
I’m pretty sure the lite version is only for battery monitoring while the full version has discharging capabilities.
```

---

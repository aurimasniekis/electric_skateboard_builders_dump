# What products/solutions do you want for electric skateboards? (designing a remote)

### Replies: 37 Views: 2857

## \#1 Posted by: VladPomogaev Posted at: 2016-09-12T05:15:35.117Z Reads: 295

```
Hello,

I was wondering if you guys had any ideas for controllers or accessories for electric skateboards. I recently finished and sold my first [smartphone controller units](https://www.youtube.com/watch?v=W1b1Y-LHR4g) (shameless plug there), but a lot of people exclaimed their interest in a handheld remote solution. I still stand by the integrity of what I made, but I was just wondering what kind of remote you guys are looking for, and how much it would cost.

I've been experimenting with components, and the things I can include in a remote include a voltmeter, RPM counter, speedometer, range remaining, etc.. I was thinking of making a product that completely emulates the Boosted Board setup, minus the Low Power Bluetooth (so a proper, high power 2.4Ghz module). I was wondering if there still is a demand for such a device, what kind of features it should have, and what it should be priced at. 

Cheers,

Vlad
```

---
## \#2 Posted by: smurf Posted at: 2016-09-12T05:21:16.885Z Reads: 281

```
A switch for headlights and a button for a horn. Maybe turn signals
```

---
## \#3 Posted by: VladPomogaev Posted at: 2016-09-12T05:22:54.251Z Reads: 273

```
For real? I always thought the lights looked cool, but a horn? My eboard is already loud enough :P
```

---
## \#4 Posted by: lox897 Posted at: 2016-09-12T05:30:57.779Z Reads: 256

```
Different modes such as beginner, intermediate, pro
```

---
## \#5 Posted by: saul Posted at: 2016-09-12T05:46:09.894Z Reads: 253

```
I was just thinking of something like this, but no time for more projects.

make sure its nice and small, rechargable.... multiple styles....
```

---
## \#6 Posted by: harpie Posted at: 2016-09-12T06:07:46.818Z Reads: 235

```
Those winning remotes with proper hardware to support openlrs would be great. Should only be some pcb design. No need for mechanical or software effort. would love to do this myself, but just too little time.
```

---
## \#7 Posted by: FlashNova Posted at: 2016-09-12T06:23:10.882Z Reads: 230

```
A simple solution for a working brake light would be the coolest thing ever. I want a tail light that actually gets brighter when i pump the brakes.
```

---
## \#8 Posted by: kampfhahn Posted at: 2016-09-12T06:51:26.395Z Reads: 226

```
+1

Especially when friends or family are testing my esk8, i can´t stop saying: "Careful with the remote!!!" :D
```

---
## \#9 Posted by: Monte Posted at: 2016-09-12T07:15:42.649Z Reads: 220

```
It would be nice to have a remote like the new one from evolve. With a tiny display, and enough customon buttons for lights and cruise controll. Usually micro usb port for updates.
```

---
## \#10 Posted by: GeorgeKing Posted at: 2016-09-12T08:56:58.193Z Reads: 225

```
Speedometer
Battery Level
Thumbstick operated
Very sturdy
Compact enough to fit easily in a pocket
And most importantly, reliability.
```

---
## \#11 Posted by: Pantologist Posted at: 2016-09-12T13:36:12.410Z Reads: 209

```
Is Bluetooth Low energy really that unreliable?

How hard would it be to implement the same Bluetooth receiver and a Bluetooth remote like Boosted's? Bluetooth would be easier to implement an on remote volt meter and different speeds settings.

I don't think adding a LCD is really necessary. A speedometer is also not that important.
```

---
## \#12 Posted by: treenutter Posted at: 2016-09-12T13:58:01.190Z Reads: 211

```
The number one feature should be 100% reliability with zero dropouts. Everything else is nice to have, but a luxury compared to reliability. The number of people that have SYF'd because of a controller\signal dropout is way too high.

In another thread about remotes, @chaka commented that a hybrid remote would be ideal; FHSS for throttle, AFH for everything else. I completely agree. I would prefer to avoid BT as the transmission protocol for throttle.
```

---
## \#13 Posted by: Dameista Posted at: 2016-09-12T18:08:23.164Z Reads: 196

```
maybe a remote like te one boosted board has, with a cruise setting so u just hold a button to go at a set speed. Also, a little LCD with some key information like speed, volts, and temp of your ESC and motor. also a few buttons to switch on front and rear lights would be nice to have. also range is a good thing. If you can make this and make it look nice etc and work properly i'd gladly pay 50/70 bucks
```

---
## \#14 Posted by: VladPomogaev Posted at: 2016-09-13T03:21:20.431Z Reads: 197

```
Alright, here's a little bit of my product brainstorming here for a remote:

1. Small, ergonomic
2. Rechargeable LiPo battery (what kind of battery life? how many hours?)
3. 100mW 2.4Ghz transmitter for ultimate reliability and anti-jamming
4. Small display
5. Battery level/voltage
6. Speedometer (speedometer functionality can be used to limit acceleration)
7. Cruise control

> Is Bluetooth Low energy really that unreliable?

> How hard would it be to implement the same Bluetooth receiver and a Bluetooth remote like Boosted's? Bluetooth would be easier to implement an on remote volt meter and different speeds settings.
> I don't think adding a LCD is really necessary. A speedometer is also not that important.

It's not that unreliable, but a lot of people hear stories and are deathly afraid of a remote dropping out. I'm sure the same functionality can be made available with a 2.4Ghz module. And I think an LCD is overkill as well.

I'm thinking of splitting up the functionality across a powerful 2.4Ghz transmitter remote, and a Low Energy BT module. The remote will have only four functions: control the speed, view the power remaining, set speed mode (maybe acceleration too), and a cruise control.

The Bluetooth part will allow you to set the settings, view statistics (speed, range, max acceleration, all those fun stats that you could later share on this forum ;)), and it should also allow you to control the speed, just in case you forget your remote (you might as well add this feature since you have the BT module). 

The hardest part right now is figuring out the actual mechanics of all of this... How do you implement a potentiometer into a remote that can snap back to the middle?
```

---
## \#15 Posted by: VladPomogaev Posted at: 2016-09-13T03:47:38.266Z Reads: 182

```
Also, do you guys think a xbox 360 joystick/thumbstick can do the job of controlling the throttle? Or will it be not sensitive enough?
```

---
## \#16 Posted by: Pantologist Posted at: 2016-09-13T03:50:13.779Z Reads: 184

```
I really like the Boosted thumb control or the TB Mini remote trigger style. 

I don't think a joystick will have enough travel to make for easy riding.
```

---
## \#17 Posted by: Dunmer Posted at: 2016-09-13T07:54:20.668Z Reads: 172

```
I would buy it for Sure :slight_smile:
```

---
## \#18 Posted by: Nordle Posted at: 2016-09-13T08:43:18.479Z Reads: 176

```
winning remote style with cruise control and reverse
that's all i need, no lights no horn! it's a longboard not a car
```

---
## \#19 Posted by: Okami Posted at: 2016-09-13T16:33:11.596Z Reads: 170

```
For TB mini there's a spring which pulls the trigger back into place.
```

---
## \#20 Posted by: Dameista Posted at: 2016-09-13T20:12:25.035Z Reads: 192

```
I like the ideas, but do you mean to make the bluetooth module seperate from the remote? 
because if you're gonna do that you might as wel just make an app for your phone to connect via bleutooth to the module on the board and don't even bother with a separate module with an lcd screen. So all you get is just a normal remote, this way, people can buy the normal remote an receiver, and if they want the advanced options etc, they'd have to buy the app for like 5-10 bucks. 
I do really like the idea of a cruisecontrol at a speed you can set yourself (maybe via the bluetooth?)

Another thought i had on this subject was to just give the receiver module some 5V outputs that you can switch on and off with the remote, this way, people can connect the stuff they want, (Horn, front and rear lights, a brake light even.)

The app could also be made to register where you rode the board, how fast you were going and all that usefull stuff. It shouldn't be that hard to make it work with google maps or something (One would need mobile data for this) 

If you haven't got experience in making apps, i've got a buddy who might be able to help you out. 
And try to give the remote a lanyard loop or atleast a hole to attach the loop to. 

for some building tips on the remote check out: ''greatscott elektric skateboard build part 3''. He did a really great build with a wii nunchuck and an arduino nano.
```

---
## \#21 Posted by: Pantologist Posted at: 2016-09-24T14:25:21.150Z Reads: 144

```
I think we should have a single system that acts as a receiver and information display with Bluetooth like Boosted.

On the board side: The receiver can have its own battery gauge and button to check voltage on the board itself. It will also be the Bluetooth receiver for a Bluetooth remote and Bluetooth connection to a phone app.

Remote side: Same battery voltmeter and controls. With Bluetooth it will be easier to add extra features like cruise control and lights. 

App side: Monitors battery voltage and can alert low battery or fully charged battery messages. Could also track distance we go with Mobile data and GPS. 

I'm not sure how easy it would be to connect this to the vesc and program and make changes to its config. But that would be awesome as well.

Vlad has figured out most of this with his receiver and Bluetooth app. If only it was in stock. 😉
```

---
## \#22 Posted by: VladPomogaev Posted at: 2016-09-24T17:15:25.247Z Reads: 142

```
You know, I am working on VESC integration right now! I'm at the designing hardware stage, and I pre-ordered a VESC in order to test the new setup. I totally agree; we need to continue imitating the Boosted Board because that's a proven design.

I fee like it's easier not to have a hardware voltmeter though on the board itself. It's nice to have like on the Boosted board, but it's not a necessity.

On the app side it's probable to add a distance meter and speedometer and even current through a UART connection. At first I thought that I should add more hardware to my controller so that I could support these features, but then I realized that you guys were almost exclusivly using VESCs (I was behind the times clearly), and that the VESC could support all of thee features already. 

And about that... THEY WERE SOLD OUT IN TWO HOURS! With the profit from those controllers I can probably prototype a new controller version even faster.
```

---
## \#23 Posted by: Pantologist Posted at: 2016-09-24T17:35:54.446Z Reads: 138

```
Sweet! I can't wait. 

Now that I think of it, having the voltmeter on the board is kind of a hassle to check. I'd rather check my phone or remote for battery voltage. 

@fraannk had an awesome app going. Maybe he can help out with the app design and programming.
Here's his build 
http://www.electric-skateboard.builders/t/the-iboard-loaded-vanguard-sk3-6382-168kv-10s-lipo-vesc-esc-83-mm-enertion-powerwheels/3341?u=pantologist
<img src="/uploads/db1493/original/3X/0/9/092ee642eb5826a0f7369a56ba5ee513b50a5bd6.PNG" width="281" height="499">
```

---
## \#24 Posted by: rodriguejoe1 Posted at: 2016-09-24T20:22:25.514Z Reads: 124

```
[quote="Dameista, post:20, topic:9423"]
The app could also be made to register where you rode the board, how fast you were going and all that usefull stuff.
[/quote]

Can you have an on/off toggle switch for the different options in the apps. For example I may want to know battery % and speed but not a gps register of where I rode. So those options show up on the phone screen.

Also I would like to see someone develop an emergency power cutoff device that can be used around the ankle or wrist. If someone were to fall or a board looses contact with the controller at full speed, a simple tug and maybe no head trauma or broken collar bones.  Boats and jet skies use this in case the operator is thrown into the water.
```

---
## \#25 Posted by: Pantologist Posted at: 2016-09-24T20:27:45.434Z Reads: 117

```
Could you link to how it is designed on a Jet Ski? How does it connect to the person and how does it detect if they fall off?
```

---
## \#26 Posted by: rodriguejoe1 Posted at: 2016-09-24T20:39:56.687Z Reads: 117

```
I don't own a jet ski, but my guess is that it is a PIN and that pin allows for a circuit to be completed. If the rider falls off then the PIN which is attached to the rider is pulled and pops out of the jet ski turning it off. We (esk8 guys) would need this PIN to complete an electrical circuit. I have ZERO electricity knowledge but a positive wire from the battery on one side...a pin in the middle of this circuit...and the wire from the other side to the motor for example.. and of course this would be attached to the rider.
```

---
## \#27 Posted by: rodriguejoe1 Posted at: 2016-09-24T20:44:00.521Z Reads: 116

```
http://i.ebayimg.com/00/s/MTA2NlgxNjAw/z/EF0AAOSwKrhVeaba/$_35.JPG?set_id=880000500F

ask and you shall receive!
```

---
## \#29 Posted by: EssEnn Posted at: 2016-09-24T21:03:52.508Z Reads: 116

```
Having a adjustible throttle curve would be nice as well
```

---
## \#30 Posted by: Dameista Posted at: 2016-09-29T12:07:39.313Z Reads: 109

```
Isn't the power cutoff the cruisecontrol button? Cuz you'll let that go if you fall off. So the board will stop. If you think this won't work, i just used 2 xt60 connectors for my board. Short-circutting the female plug and use that as a switch. I did this because i couldn't find a high current switch for cheap and my esc didn't have one. But if you do that you could just add a strap to the connector so if you fall off it'll disconnect and stop the motor. To me this is actually worse than the cruise control because you can set that to break whenever you let go of the cruise control, this way the board won't shoot off an hit something/someone at 25mph if you fall off.
```

---
## \#31 Posted by: SORRENTINO Posted at: 2016-09-29T13:31:28.980Z Reads: 105

```
Frequency hopping or somehow have the signal encrypted so no other 2.4 in area will effect it. I.E RC plane/drone radios. We can have up to 200 people flying at the same time with no issues all on the same 2.4ghz band.
```

---
## \#32 Posted by: rodriguejoe1 Posted at: 2016-09-29T21:30:22.856Z Reads: 103

```
[quote="Dameista, post:30, topic:9423"]
Isn't the power cutoff the cruisecontrol button?
[/quote]
I hear that if your controller looses contact with the receiver.. you are SOL!
```

---
## \#33 Posted by: VladPomogaev Posted at: 2016-09-30T03:30:34.519Z Reads: 95

```
Really? I never understood the application of this feature. I tried it out once and it felt too strong/weak depending on how I set it up. How do you use it?
```

---
## \#34 Posted by: VladPomogaev Posted at: 2016-09-30T03:33:02.836Z Reads: 96

```
Bluetooth does frequency hopping ;) Haha, there's a really strong negativity surrounding Bluetooth on these forums. The truth is, Bluetooth simply usually doesn't have as much power as an RC controller. But for eBoards this is still fine, since the distance is like a meter or so usually. Bluetooth low energy though...
```

---
## \#35 Posted by: Pantologist Posted at: 2016-09-30T03:41:44.156Z Reads: 92

```
Bluetooth Low Energy is even lower power I assume? I heard that it was made to be a lot better when it comes to interference of wifi and other similar frequencies. 

Boosted peeps only seem to have interference within largely populated cities.
```

---
## \#36 Posted by: EssEnn Posted at: 2016-09-30T10:21:22.820Z Reads: 91

```
I would like to have a controller that is not so sensitive at low throttle.
```

---
## \#37 Posted by: Okami Posted at: 2016-10-01T16:01:51.593Z Reads: 94

```
Can someone explain here how to include throttle ramping? Is it possible to make it without using arduino?

Throttle ramping

"Because sensorless R/C controllers can't really control how much current they send to the motor (and current is directly proportional to torque output), and low-speed starting can be erratic and hard to control, it is useful to have a "ramp" somewhere in the throttle chain. Without ramping or some other kind of control input damping, sudden jerk motions of your hand or foot can result in the vehicle responding unexpectedly such as a sudden application of power. This is not only hard to operate, but it can be outright dangerous if you are in traffic or around other people.Ramping can be accomplished either in hardware or in software."

Taken from instructable about escooter build
```

---
## \#38 Posted by: jrdweck Posted at: 2016-10-24T19:15:19.266Z Reads: 77

```
Why are we not taking speed control advice from the FPV drone world? 

 Control of a skateboard should be:

Thru 2.4 radio. Lowest power transmission 25mw is sufficient. 
telemetry feedback thru radio to lcd screen. 

Board has separate BT module for phone app and fancy mapping, theft prevention, etc. 

Trigger Finger control. They discovered 50 years ago that controlling a slot car was better with you finger. 

Hardware dial throttle/braking rate control. 
Hardware trim button.
Hardware middle position adjustable. 

So yes, this is an r/c contoller, but with 80% of the bulk and functions cut out of ths transmitter. 

Just a thought.
```

---

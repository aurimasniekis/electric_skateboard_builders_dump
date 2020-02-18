# How does the torque curve change with voltage?

### Replies: 32 Views: 6492

## \#1 Posted by: Leav Posted at: 2017-06-20T09:22:09.359Z Reads: 265

```
Hi,

I'm currently sourcing parts for my first build and am learning along the way.
The biggest design constraint for me is climbing a fairly steep hill on my commute (10-15%), and my weight (~115kg)

I have decided to go with the [Tacon Big Foot 160](http://www.hobbypartz.com/96m608-bigfoot160-5335-245kv.html), and have built a small spreadsheet calculator to understand what kind of pack I want.

However I'm stumped when it comes to understanding the motor specs... I'm much more familiar with brushed DC motors where you are given some nice parameters to work with:

* Stall Torque (at given voltage)
* Free speed (at given voltage)

You can pick your gearing ratio to get close to peak power at ~50% stall torque, **and you can assume that both free speed and stall torque scale linearly with the voltage (ball park estimate).**

I feel like I'm missing a bunch of data for the Tacon:
* Sure, it's 2600W... but at what torque and voltage?
* Does a BLDC motor have a stall torque?

Is there anyway to estimate these? Do BLDCs have entirely different characteristics that make the calculations vastly different?

How do I approach this?

Thanks
```

---
## \#2 Posted by: mmaner Posted at: 2017-06-20T15:18:15.509Z Reads: 229

```
If I understand correctly, you are looking for the formulas that will give you values on performance, consumption and limits.  Most of that can be found here...

https://longhairedboy.com/pages/esk8-resources

Or check out this thread for a discussion on the formulas...

http://www.electric-skateboard.builders/t/im-building-an-esk8-resources-page/21453
```

---
## \#3 Posted by: Leav Posted at: 2017-06-20T17:27:35.101Z Reads: 209

```
Actually, that's not really what I'm looking for. I'm less concerned with max speed, and more concerned with actual power and torque.

Here's a mockup of the data I'd expect to find on a DC motor. Is it unreasonable to expect this sort of data fot BLDCs for some reason? maybe the way they are controlled doesn't result in these sort of graphs?

<img src="/uploads/db1493/original/3X/e/6/e68082a5ad4076276728b21beff91c8924134866.png" width="667" height="500">

Here's a full mockup of a DC motor graph, lots of info to be used from it:
<img src="/uploads/db1493/original/3X/1/4/14b8ef14bf9e24fbd686fb021b45efea7da90401.jpg" width="500" height="390">
```

---
## \#4 Posted by: oldguy Posted at: 2017-06-20T17:30:20.039Z Reads: 188

```
I was told there would be no math...
```

---
## \#5 Posted by: mmaner Posted at: 2017-06-20T18:12:26.723Z Reads: 188

```
They lied to you brother :slight_smile:
```

---
## \#6 Posted by: Leav Posted at: 2017-06-20T20:17:05.543Z Reads: 179

```
So I'm attempting to make sense of the table data... maybe giving some more concrete questions will help get answers! :)

I see that the Internal resistance is 0.03ohms.
So let's say you stall the motor and apply a voltage.. you'd reach the "peak efficiency current" of 75A @ 2.25v (this doesn't mean anything really, just gives a ball park figure.

with a stalled 8s setup you'd get a smoke inducing ~1000A current.

**This seems to suggest to me that the battery voltage is NOT the limiting factor in a BLDC's ability to produce torque. **
**Is this true?**

Assuming it is true, and If torque is the goal, is there any advantage with going with a higher voltage? will the current be lower for a given torque? Does Kt change with voltage? 

<img src="http://www.electric-skateboard.builders/uploads/db1493/original/3X/4/8/488044c8ce0f07958b18f46f214ce5a6adcaaede.png">
```

---
## \#7 Posted by: Challlsss Posted at: 2017-06-20T20:50:39.965Z Reads: 160

```
Hiya I'm gonna take a stab at this... So my understanding is that voltage is not effecting our torque. Unless you account for how it effects your gear ratio.... ie 12S is around 160kv wheras 6S is closer to 200kv typically. These changes will effect torque throughout the sytsem however. So lets leave that alone.

Torque is effected by current. That is why when your motor is unloaded it spins up to full speed at only a few amps... but when you stand on it getting up to full speed take significantly more amps. (depending on your gearing of course)

Sooooooo: to answer what I believe you are asking....

- Yes voltage is important in deciding torque (but only because it effects which kv motor you use. lower kv = higher torque and lower speed

- No, kv does not effect voltage think of it as a gear ratio from voltage to the motor. A 300kv motor would spin 2x as fast as a 150kv motor with the same voltage, __but__ it would also have 1/2 as much torque (because it is a gear ratio)

- This wasn't a question but ill mention it, you also get more torque with higher current so if you still wanted more current but you weren't going to change batteries or motors then you could adjust max current settings to get more torque. (this is also how you control brake strength.)
```

---
## \#8 Posted by: sprocket12 Posted at: 2017-06-20T21:21:09.510Z Reads: 140

```
Nice.  I appreciate your clear explanation.  And *very* little math @oldguy
```

---
## \#9 Posted by: Boardnamics Posted at: 2017-06-20T21:43:19.049Z Reads: 141

```
Voltage itself does in fact gain more torque naturally. Assuming all other parameters are the same, feeding more voltage to a bldc motor will generally increase its torque output. Ohms law tells us that a higher voltage with the same resistance will have a greater amperage. I found this out by datalogging rc cars as well, higher voltages seem to draw more current as well. The torque output of the motor is based on its load given/current draw. That graph you posted pretty much sums it up. It is hard to get an esk8 board to be extremely efficient. You do you, but in my opinion this calculation is rather unnecessary considering so many people have success with just the general kv gear ratio calculations. Any 50 or 63 size motor with the proper gearing satisfies many.
```

---
## \#10 Posted by: Leav Posted at: 2017-06-21T06:16:22.103Z Reads: 135

```
Thanks for the replies :)
I understand what you're trying to say, I'll try to follow up on your info with the following:

[quote="Challlsss, post:7, topic:25760"]
A 300kv motor would spin 2x as fast as a 150kv motor with the same voltage, but it would also have 1/2 as much torque (because it is a gear ratio)
[/quote]

It is my understanding that motors are all current limited, so a 150kv motor would not be able to supply 2 times the torque of a 300kv motor, because the windings are smaller and thus can carry less current...

Basing this on [Vedder's post](http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/)

[quote="Lionkev55, post:9, topic:25760"]
Ohms law tells us that a higher voltage with the same resistance will have a greater amperage.
[/quote]

Yeah it's just that a I feel like when it comes to torque you would be current limited even with a 4s.... so V=IR doesn't really apply if you have more voltage but the controller is lowering the PWM duty cycle (or however it works) to keep the current under the specified MAX CURRENT setting.
```

---
## \#11 Posted by: MoeStooge Posted at: 2017-06-21T12:25:06.187Z Reads: 120

```
It always involves math.   My inrunner is advertised at 3000w @ 50krpm. First find Horsepower.   1 Watt =.00134 hp. So 3000x.00134=4.02hp.  Ok to find torque plug in. Hp x rpm / 63025 = torque.  4.02x50000 / 63025=3.19ft lb of torque. I would knock off 20% for efficiency.
```

---
## \#12 Posted by: Leav Posted at: 2017-06-21T12:31:49.996Z Reads: 116

```
Found some corroborating info: [This lecture on youtube seems to 100% validate my understanding](https://youtu.be/ciLzUUDPgGE?t=379) that BLDCs are current limited.

[quote="MoeStooge, post:11, topic:25760"]
My inrunner is advertised at 3000w @ 50krpm
[/quote]

I wish Tacon would advertise the voltage at which you can achieve 2600W!
```

---
## \#13 Posted by: Challlsss Posted at: 2017-06-21T12:47:29.485Z Reads: 111

```
you are correct. BDLC is current controlled.
```

---
## \#14 Posted by: MoeStooge Posted at: 2017-06-21T15:20:08.890Z Reads: 107

```
Amp x volt = Watt.  Plug in your numbers.
```

---
## \#15 Posted by: Leav Posted at: 2017-06-21T15:34:16.238Z Reads: 105

```
[quote="MoeStooge, post:14, topic:25760, full:true"]
Amp x volt = Watt.  Plug in your numbers.
[/quote]


my numbers are 4.2Nm of torque @ 3200 RPM

Can you tell me how much amp that is? I found some suggestions that in general:
Kt=60/2*pi*Kv              (Kt [Nm/amp] & Kv [Rpm/v])

But I have also seen that Kv is only valid under no load so I have no real idea how to calculate or find the Kt without the manufacturer's specs or a Dyno...
```

---
## \#16 Posted by: Hummie Posted at: 2017-06-21T16:54:25.887Z Reads: 95

```
U can easily get the kv off the Vesc test looking at voltage and rpm and convert from there to kt if you can do math.  It would be at no-load. 
dont know if you know but getting amps to the motor at low rpm, low duty cycle, low speed is done through the Motor amp setting.  with the pwm at low speed there's  low effective voltage but you can have way more amps running continuously in the motor than have left the battery.
```

---
## \#17 Posted by: Leav Posted at: 2017-06-21T17:08:31.370Z Reads: 98

```
[quote="Hummie, post:16, topic:25760, full:true"]
U can easily get the kv off the Vesc test looking at voltage and rpm and convert from there to kt if you can do math.  It would be at no-load. 
[/quote]

Cool! Didn't know that (I have NONE of the parts yet, they are all on their way)

[quote="Hummie, post:16, topic:25760, full:true"]
dont know if you know but getting amps to the motor at low rpm, low duty cycle, low speed is done through the Motor amp setting.[/quote]
Actually I think I learned this from another thread where you were discussing it with someone else.

[quote="Hummie, post:16, topic:25760, full:true"]
 with the pwm at low speed there's  low effective voltage but you can have way more amps running continuously in the motor than have left the battery.
[/quote]

WTF? how is that possible?
```

---
## \#18 Posted by: Hummie Posted at: 2017-06-21T17:33:31.192Z Reads: 88

```
The data output from the Vesc you can see there's the motor amps and the battery amps and are two different limits you can set. The details on how you can practically have so many motor amps I don't know o remember but am hoping you can tell me again!  I envisioned it working somewhat like a transformer as the ultimate energy output from the battery and at the motor must be the same but at low speed u now have the low voltage through switching but very high current vs what registers coming from the battery.
```

---
## \#19 Posted by: snorren Posted at: 2018-03-03T20:25:52.068Z Reads: 74

```
That would be true if the motor was doing for example 3000w of _mechanical effect._

The easiest way to realize this is to start from stationary, apply 3000w of _electric effect_ and by using P[watt]=angular velocity [rad/s] * torque [Nm] we would get infinite torque. 

This is not the case. This is when the efficiency curves comes into place. Lets say the motor will draw 3000w of power standing still when you crank the throttle. The efficiency at a certain rpm will let you know how much mechanical power you get for the electrical power you supplied.

Realistically at something low like 1000 rpm, efficiency is perhaps 1-5% so you get 3000w*0.05=150w mechanical power and 2850w of heat. As the Rpms increase so does efficiency up to a certain limit. So the real torque would just be something like 1.4 Nm. But then again you have your smart ESC that will limit the current in this situation to avoid burning the motor.

To answer the main question. A higher voltage will allow more current to flow through the motor winding and therefor increase the torque.
```

---
## \#20 Posted by: MoeStooge Posted at: 2018-03-03T23:00:13.489Z Reads: 67

```
[quote="snorren, post:19, topic:25760"]
To answer the main question. A higher voltage will allow more current to flow through the motor winding and therefor increase the torque.
[/quote]

Your half there.  Raising Voltage will raise the Watts a motor will produce but will not raise the current or amps that it can handle or flow through it. Amps or current stays the same.   Some day I will put the raceboard on a Dyno. 3000w = 1.4nm or 1 ft lb of torque indeed.  3000w or 4hp= 1ftlb of torque nope sorry mate motors make better torque #s then that. ![Screenshot_20180303-145728|281x500](upload://niizCPGWEIl9l9pUnCjWFPeZTIn.png)
```

---
## \#21 Posted by: snorren Posted at: 2018-03-03T23:30:31.611Z Reads: 66

```
[quote="MoeStooge, post:20, topic:25760"]
Voltage will raise the Watts a motor will produce but will not raise the current or amps that it can handle or flow through it. Amps or current stays the same.   Some day I will put the raceboard on a Dyno. 3000w = 1.4nm or 1 ft lb of torque indeed.  3000w or 4hp= 1ftlb of torque nope sorry mate motors make better torque #s then that.
[/quote]

Ok so try to put 1000 v through a motor and see if the current doesn't increase and fry the motor. Of course more current will flow through a conductor the if voltage is increased, that is basic knowledge. U=RI

And you didn't understand the difference between electric effect and mechanical effect. You are saying 3000 w of mechanical work is more than 1.4 Nm at 1000 rpm, yes that is what i said as well. But if the efficiency of the example motor is only about 5% like at very low Rpms, drawing 3000w of electric power will only get you 150w of mechanical work. 

Look at the typical bldc characteristics below. At 500 rpm you will only get 10% efficiency. So feeding the motor 3000w of electricity the motor will produce 300w of mechanical power and 2700w of heat.

If you did the same thing at but at 4600 rpm where you have 95% efficiency you would get 2850w of mechanical power and 150w of heat.

http://www.mellorelectrics.co.uk/BLDC-performance-graph.jpg
```

---
## \#22 Posted by: snorren Posted at: 2018-03-03T23:35:38.891Z Reads: 61

```
Edit: Should be 70% efficiency at 3500 rpm transforming 3000w of electric power to 2100w of mechanical power and 900w of heat.
```

---
## \#23 Posted by: MoeStooge Posted at: 2018-03-04T00:05:15.941Z Reads: 60

```
[quote="snorren, post:21, topic:25760"]
Ok so try to put 1000 v through a motor and see if the current doesn’t increase and fry the motor. O
[/quote]

I'm afraid 1000v would flash over before you could get an amp read. Just make sure your wearing HV gloves and a blast shield. Amps still stay the same by the way. A conductor carries the same amps regardless of volts.  Like those copper windie things in an electric motor. Seriously kids don't play with high voltage
```

---
## \#24 Posted by: snorren Posted at: 2018-03-04T00:16:37.482Z Reads: 57

```
Are you trolling? 
"Ohm's law states that the current through a conductor between two points is directly proportional to the voltage across the two points."

It doesn't get more basic than this.
```

---
## \#25 Posted by: Cobber Posted at: 2018-03-04T00:20:29.999Z Reads: 55

```
I could be wrong here @snorren, but I think what is happening here is you are talking about what it says in a text book and @MoeStooge is talking about what happens in practice.

knowledge v's wisdom

By the way if you do decide to put 1000v through a small bldc motor, get that shit on video dude ;)
```

---
## \#26 Posted by: snorren Posted at: 2018-03-04T00:29:13.693Z Reads: 51

```
Well if the textbook would be different from reality I probably would have been fired years ago from my job as an mechatronics engineer. But I appreciate the peace gesture Cobber ;)
```

---
## \#27 Posted by: MoeStooge Posted at: 2018-03-04T01:03:22.926Z Reads: 50

```
Yup a #6 copper conductor is rated to carry 115a regardless if the voltage is 50 or 5000. If you knock the amps up to say 200 the wire will heat and burn regardless of voltage. Ft lb is a mechanical measurement and a motor that makes 3000w makes more than 1 ft lb of torque weather it is a 10v or 100v motor.
```

---
## \#28 Posted by: snorren Posted at: 2018-03-04T07:51:42.867Z Reads: 49

```
I give up.
```

---
## \#29 Posted by: Fungineers Posted at: 2019-03-14T11:24:10.182Z Reads: 34

```
Its interesting to see that the conversation came down to the very basics: Ohm's law. 
Both @snorren and @MoeStooge have a point. Ohm's law has to hold, obviously, so V=IR, and for a given resistance, if voltage is increased, current will definitely increase. 
But, @MoeStooge said that according to the formula Power=VI, as voltage is increased, current should decrease..hold on...FOR A GIVEN POWER! 
See, a motor has power (torque and speed) characteristics FOR A GIVEN VOLTAGE, for example, at 24V, as you give the motor more current, the power increases. But if you talk about changing the voltage, the motor no longer has the same characteristics, and has a different power curve. So now, with increased voltage, will come increased current, at an increased power, and if a motor is not rated for that, it will overheat and burn. That's why motors have a rated voltage. At that given voltage, as you increase the current, the power increases.
```

---
## \#30 Posted by: Okami Posted at: 2019-03-14T12:54:06.252Z Reads: 32

```
I think we should also look here about controller limits. Basically if u take 12s controller which can do 50A, then with higher voltage more watts produced. So in this case higher voltage better (unless u take lower quality vesc which might dye sooner because of 12s)

Also better for the wires and other parts, as less heating should happen.

I think motor power most of the time should be concluded from both amps and voltage, in our case I think maximum suggested would be around 12s anyways but then practical tests should be made to figure it out precisely.
```

---
## \#31 Posted by: MoeStooge Posted at: 2019-03-14T13:20:36.115Z Reads: 36

```
Here's a real world application. The motors I run are rated 60v at 200a. 12kw.
 I run at 30v. 200a 6kw.  
 If I tried to get 12kw at 30v at 400a the motor would quickly fail. 
 As long as you stay under your Volt and amp ratings your motor came with you will be fine.
```

---
## \#32 Posted by: Hummie Posted at: 2019-03-14T16:50:17.165Z Reads: 33

```
[quote="Leav, post:6, topic:25760"]
Assuming it is true, and If torque is the goal, is there any advantage with going with a higher voltage? will the current be lower for a given torque? Does Kt change with voltage?
[/quote]

Higher voltage won’t increase torque. The current in the motor won’t be lower. Kt won’t change w voltage

There isn’t really a voltage limit of a motor other than the enamel magnet wire and the bearing speed ability.

The esc bucks down the voltage so the pack may be 50v but the esc is sending much less through pwm and creating an effective voltage.  When going faster the motor produces its own voltage as a generator, the back voltage, and the esc will increase it’s output related to that so you would only maybe have the full 50v applied to the motors at top top speed where the back voltage is so high and needs be overcome. In that instance you’re subtracting the back voltage it’s fighting against and you’ll end up with still maybe only a couple of volts across the motor winding

The kv/kt of the motor and the amps put to it and the wheel diameter or gear ratio decide torque solely. Kv and kt encompasses a lot as it reveals torque produced per amp period
```

---

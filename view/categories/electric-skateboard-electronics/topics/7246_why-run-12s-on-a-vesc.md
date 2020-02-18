# Why Run 12s on a VESC?

### Replies: 145 Views: 10769

## \#1 Posted by: Workaround Posted at: 2016-08-07T03:19:22.418Z Reads: 727

```
Why do I keep seeing builds wanting to run 12S on a VESC?

I keep seeing people posing they want 12s and want to use a VESC. I'm sure the VESC can only handle 10s.

This is what I keep seeing
http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:10,%22motor-kv%22:230,%22system-efficiency%22:80,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:36,%22wheel-size%22:83}|

Why do people want to go that fast. Is everyone just running there systems on race tracks.
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-07T03:25:31.043Z Reads: 704

```
Higher voltage typically reduces current draw and heat. The VESC can handle up to 12S, but gets pretty close to hitting the voltage limit in some scenarios. It can also hit the eRPM limit if an inappropriate motor is used.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-08-07T03:27:51.226Z Reads: 698

```
First of all, that calculator is no where near accurate.
I know this because I have run 12s lipos for some time with both dual hub motors and dual 230kv motors with 16/36 belt drive. 90mm wheels
Both case using 12s opto Esc's
The highest speed I every got with the hubs on flat ground was 33mph
The highest speed I every got with the belt drive motors was 28mph
Still I agree with you that 12s is really pushing it.
With torque and acceleration that is hard to handle
And really pushing the electronics and motors to their limits causing extra heat.
I have recently rebuilt my system with 10s and 190kv motors.
Top speed is only around 20-23mph
because I feel that 20mph is fast enough.
```

---
## \#5 Posted by: barajabali Posted at: 2016-08-07T03:30:09.071Z Reads: 671

```
VESC doesn't handle super high amps either. The More voltage the  less amps
```

---
## \#6 Posted by: Namasaki Posted at: 2016-08-07T03:32:40.305Z Reads: 651

```
True but where do you draw the line?
I'm thinking that 10s is the sweet spot.
```

---
## \#7 Posted by: Jinra Posted at: 2016-08-07T03:33:02.380Z Reads: 636

```
The calculator merely calculates the values based on a perfect world scenario. It only says what the speeds would be if every component performed at their given ratings. Higher voltage doesn't necessarily mean more torque or acceleration either. FWIW the calculator is pretty accurate to what I get on my board at 29mph (calculated 31mph).

At 12S though, there may be some losses in efficiency depending on your system, which can lead to lower speeds. @Photorph has gotten 38mph on his board which has a calculated speed of 41mph. 

I'd say the calculator is pretty accurate for 10S and below.
```

---
## \#8 Posted by: barajabali Posted at: 2016-08-07T03:34:17.523Z Reads: 603

```
I agree with you. Only reason to run 12s is on hubs, or speed demons.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-08-07T03:36:25.657Z Reads: 589

```
I tested 12s vs 6s on the same dual 230kv belt drive system and there was a lot more torque and acceleration with 12s.
6s was much smoother and more controllable.
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-07T03:38:30.401Z Reads: 570

```
When you run 12s, the ESC can supply the power to the motor easier. With lower voltage, current can be bottled necked by BMS/ESC/cable size/etc. I don't doubt that you had more torque on 12s, but just saying this isn't always the case.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-08-07T03:39:14.939Z Reads: 559

```
I think that running 12s with high kv motors has a similar effect on car esc's and it does on the vesc.
More heat.
Isn't that what kills the Drv chip when you exceed the erpm limit, It gets too hot and burns up?
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-07T03:40:21.360Z Reads: 541

```
Yea higher speeds = higher heat as well. There's a point where higher voltage doesn't reduce heat from current anymore.
```

---
## \#13 Posted by: Namasaki Posted at: 2016-08-07T03:43:42.166Z Reads: 529

```
I think your right @Jinra  that more rpm= more heat. It makes sense because the Esc or Vesc has to switch the magnetism of the motor poles continuously as it spins so the faster it spins the faster the controller's switches have to work.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-08-07T03:45:23.408Z Reads: 510

```
I guess it's safe to say that there are multiple factors causing heat in the system.
```

---
## \#15 Posted by: Jinra Posted at: 2016-08-07T03:47:31.959Z Reads: 509

```
For sure! I think it's somewhat of a misconception that higher voltage = lower heat. That said I believe 10s is the best battery setup for the VESC in its current iteration. Hopefully with 6.0's release, it'll be more robust to handle higher voltages and current; not to mention FOC!
```

---
## \#16 Posted by: Namasaki Posted at: 2016-08-07T03:50:58.197Z Reads: 498

```
I agree with you, 10s seems to be the sweet spot. Now with my new setup, its very smooth and gradual acceleration at the low end of the throttle and fast at the top end of the throttle. waiting for my Vesc's to come so I can try that setup.
```

---
## \#17 Posted by: Photorph Posted at: 2016-08-07T03:51:05.278Z Reads: 483

```
Technical jargon aside...

All I can say is i have a 12s4p running on 16/33 with dual 190 kv r spec motors.  After doing runs of 30+ mph continuosly for like a mile straight, I can still touch my motors with my hands and they just feel warm.
```

---
## \#18 Posted by: Namasaki Posted at: 2016-08-07T03:52:06.049Z Reads: 471

```
are you using Vesc's ?
```

---
## \#19 Posted by: Photorph Posted at: 2016-08-07T03:52:47.508Z Reads: 465

```
Yes, Chaka VESCs
```

---
## \#20 Posted by: Jinra Posted at: 2016-08-07T03:52:49.156Z Reads: 465

```
You have 190kv motors which doesn't go much higher than the eRPM limit, so while you're motors aren't turning insanely fast, your gearing is much lower leading to the speeds you're getting. If you're going up a lot of hills or against a lot of wind, you're motors would be pretty toasty.
```

---
## \#21 Posted by: Photorph Posted at: 2016-08-07T03:54:03.990Z Reads: 458

```
No hills, either perfectly smooth and flat tarmac or slight downhill on that one mile run where I touched the motors.
```

---
## \#22 Posted by: Namasaki Posted at: 2016-08-07T03:54:06.059Z Reads: 427

```
what is your weight? that can be a huge factor
```

---
## \#23 Posted by: Photorph Posted at: 2016-08-07T03:54:34.276Z Reads: 424

```
135 lbs, prolly like 140 with my helmet and all my crap on.
```

---
## \#24 Posted by: Namasaki Posted at: 2016-08-07T03:55:33.572Z Reads: 415

```
ok, there you go. 140 is gonna give a huge advantage for top speed and less load or less heat
I'm a sorry 185
```

---
## \#25 Posted by: onloop Posted at: 2016-08-07T03:59:20.020Z Reads: 418

```
[quote="Namasaki, post:16, topic:7246"]
10s seems to be the sweet spot.
[/quote]

correct.....
```

---
## \#26 Posted by: Blacksheep Posted at: 2016-08-07T04:13:00.253Z Reads: 413

```
I'm building my first board and have 4 3s and @chaka vesc so that's not good ?
```

---
## \#27 Posted by: Titoxd10001 Posted at: 2016-08-07T05:11:08.620Z Reads: 406

```
@Namasaki tb motors are rated as 230kv but are really only 190kv you can calculate by checking in bldc tool they hit about 67000 erpm on 12s
```

---
## \#28 Posted by: Jinra Posted at: 2016-08-07T05:14:04.543Z Reads: 418

```
That's not the best way to calculate kv. Check this out.

http://www.electric-skateboard.builders/t/ollinboardco-om5065-200kv-sensored-motor/3409/351?u=jinra

I got 194 and 197 kv on my 200kv motors.
```

---
## \#29 Posted by: evoheyax Posted at: 2016-08-07T05:17:49.784Z Reads: 391

```
It does seem nice, but you draw a lot more amps than on 12s. I want to do more tests, but real world tests I did with a watt meter showed me drawing 50 amps from the space cell continuous, and same hill with 12s was only pulling 30 amps. 

12s seems to me to be the best if you can do it in terms of lowering heat in your vesc, and maximizing torque. You seem to have a higher chance of blowing a vesc (based on the experiences of those on this forum) running 12s.

The other thing is, why does everyone seem to ignore 11s? Wouldn't that bring the likely hood of blowing up the vesc down, while having some of the benefits of 12s?
```

---
## \#30 Posted by: Jinra Posted at: 2016-08-07T05:20:16.001Z Reads: 376

```
If the VESC 6.0 wasn't coming out soon-ish, I might've actually wanted to try that when I build my own pack.
```

---
## \#31 Posted by: Michaelinvegas Posted at: 2016-08-07T05:21:35.834Z Reads: 372

```
[quote="evoheyax, post:29, topic:7246"]
The other thing is, why does everyone seem to ignore 11s?
[/quote]



Lol I think it's like having a third nut... It's all about the symmetry lol
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-07T05:22:20.911Z Reads: 361

```
But 11 is symmetrical, almost as much as 8! :P
```

---
## \#33 Posted by: evoheyax Posted at: 2016-08-07T05:23:30.952Z Reads: 354

```
hahaha, good point. but with the 18650s, say you have 44 cells for a 11s4p, there's no oddness out that :stuck_out_tongue:
```

---
## \#34 Posted by: Michaelinvegas Posted at: 2016-08-07T05:27:38.326Z Reads: 352

```
Lol ... But seriously Is it a matter of wiring? Or maybe battery pack formation that make it unappealing?

It's easy to relate it back to LIPO packs ... Hard to justify that extra lipo on a 10s build...is that extra voltage worth it?
```

---
## \#35 Posted by: Michaelinvegas Posted at: 2016-08-07T05:29:47.745Z Reads: 344

```
[quote="evoheyax, post:33, topic:7246"]
hahaha, good point. but with the 18650s, say you have 44 cells for a 11s4p, there's no oddness out that :stuck_out_tongue:
[/quote]

No you're right...especially if we are talking abt symmetry.
```

---
## \#36 Posted by: Titoxd10001 Posted at: 2016-08-07T05:32:52.593Z Reads: 335

```
10s chargers are easier to find than 11s chargers
```

---
## \#37 Posted by: evoheyax Posted at: 2016-08-07T05:34:46.437Z Reads: 341

```
[quote="Titoxd10001, post:36, topic:7246, full:true"]
10s chargers are easier to find than 11s chargers
[/quote]

True, but you can find a charger for just about anything,it's just a matter of searching.
```

---
## \#38 Posted by: Titoxd10001 Posted at: 2016-08-07T05:38:08.972Z Reads: 335

```
True I like the cheap chargers whitepony found with "adjustable" voltage idk if any will work with 11s tho
```

---
## \#39 Posted by: torqueboards Posted at: 2016-08-07T05:44:37.749Z Reads: 332

```
I wonder.. if when VESC 6.0 comes out the responses would change.
```

---
## \#40 Posted by: SimosMCmuffin Posted at: 2016-08-07T06:39:29.466Z Reads: 334

```
[quote="barajabali, post:5, topic:7246"]
The More voltage the  less amps
[/quote]

This is with the assumption that either the gearing is changed or a lower kV motor is used with a higher voltage. If you don't change the motor, but just up the voltage, you will also pull more Amps. The reason why I point this out is that you didn't point it out.
```

---
## \#41 Posted by: Jinra Posted at: 2016-08-07T06:45:30.344Z Reads: 326

```
Not how I understand it. Assuming the exact same rider, board, and hill. If it takes 1200w of power to go up the hill, at 6s this requires 54 amps, and at 12s this requires 27 amps
```

---
## \#42 Posted by: barajabali Posted at: 2016-08-07T06:51:57.347Z Reads: 307

```
That's how it is
```

---
## \#43 Posted by: barajabali Posted at: 2016-08-07T06:53:10.688Z Reads: 302

```
not true

10 char
```

---
## \#44 Posted by: SimosMCmuffin Posted at: 2016-08-07T06:55:07.022Z Reads: 297

```
And if you're using the same motor kV in both situations, then you're running 100% duty cycle with the 6S and only 50% with the 12S, with the 12S you would be going at just half of the top speed. This is the problem with the "steady" terminology, which has been discussed in http://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910/142
```

---
## \#45 Posted by: Jinra Posted at: 2016-08-07T06:57:14.923Z Reads: 300

```
I stopped following the thread because it was such a mess. Why are you comparing 100% duty cycle to 50% though? We're comparing S count (voltage) so we should compare 100% duty cycle to 100% duty cycle.
```

---
## \#46 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:00:25.718Z Reads: 310

```
How about providing some maths that prove that it isn't so, rather than just saying "not true".

Let me demonstrate
[quote="Jinra, post:41, topic:7246, full:true"]
Not how I understand it. Assuming the exact same rider, board, and hill. If it takes 1200w of power to go up the hill, at 6s this requires 54 amps, and at 12s this requires 27 amps
[/quote]

Let's calculate the motor winding resistance with the Ohm's law:
R = U / I
6S battery motor -> 21,6 V / 54 A = 0,4 Ohms
12S battery motor -> 43,2 V / 27 A = 1,6 Ohms

They are two different motors, with different windings and therefore different kV!
```

---
## \#47 Posted by: Jinra Posted at: 2016-08-07T07:02:11.675Z Reads: 299

```
Sorry, I'm not sure why we're talking about two different motors now. My example assumed the same board, therefore same motor.
```

---
## \#48 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:04:38.509Z Reads: 286

```
But the math proves your example has two different motor winding resistances therefore different kVs. If you can't produce any math that proves your example, then what do you have to back it up? Your opinion that this is how it works?
```

---
## \#49 Posted by: barajabali Posted at: 2016-08-07T07:06:06.118Z Reads: 289

```
Sorry I shouldn't have even commented as I don't really care to argue tonight. Lol

No one is fighting you that's not how you make friends
```

---
## \#50 Posted by: Jinra Posted at: 2016-08-07T07:07:17.377Z Reads: 285

```
I know it's hard to read tone through text, but I mean no disrespect in anything I'm saying. I'm just a little lost on the logic. 

Let's refer back to my initial example and assume each motor is 190kv. I'm not sure what the battery voltage has to do with the kv of the motor.
```

---
## \#51 Posted by: barajabali Posted at: 2016-08-07T07:08:01.070Z Reads: 275

```
Yea maybe we're arguing the same point. I have to go and read this whole thread.  

@SimosMCmuffin
```

---
## \#52 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:09:25.969Z Reads: 261

```
I did not want an angry argument, but just wanted to point out that the math doesn't work out if both motors are the same kV.
```

---
## \#53 Posted by: barajabali Posted at: 2016-08-07T07:09:49.969Z Reads: 264

```
But we're curious how different voltage changes the kv of the motor...?

And understood I'm sure we're arguing the same point just misunderstanding each other. 
Physics only has one answer (most of the time)
```

---
## \#54 Posted by: Jinra Posted at: 2016-08-07T07:11:02.602Z Reads: 256

```
I mean.. I don't think it would. I did a calculation on my 200kv chaka motors at 6s and got 197 on one of them. I tested **another** 200kv chaka motor on 10s and got 194. So it doesn't seem to have any effect on kv, and if there is, it's very minor.
```

---
## \#55 Posted by: barajabali Posted at: 2016-08-07T07:12:39.092Z Reads: 253

```
Voltage isn't changing the number of turns on a stator. Or gauge of wire. Or winding pattern. So I don't see how it would effect kv
```

---
## \#56 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:16:11.667Z Reads: 266

```
Ok.

If we have a motor with a 190 kV, then we can easily see how fast it runs with the voltage.

12S = 43.2V * 190kV = 8208 rpm
6S = 21.6V * 190kV =  4104 rpm

so we are pushing 1200 Watts of power at 21.6 Volts and 54 Amps. Now we can calculate the winding resistance for the motor R = U /I = 21.6 V / 54 A = 0.4 Ohms.

Now, if we were to put that 12S = 43.2 Volts across the 0.4 Ohm motor winding _**full time**_, our power would be
P = U^2 / R = (43.2V)^2 / 0.4 Ohms = 4665,6 Watts!

This is why I said that the 12S motor would have to be run at 50% duty cycle so it's effective voltage becomes the same as 6S at 100% duty cycle; V = 12S * DutyCycle = 43,2V * 0.5 = 21.6 Volts and then the power would be same.

Did this help, or would you like more examples?
```

---
## \#57 Posted by: Jinra Posted at: 2016-08-07T07:25:48.271Z Reads: 256

```
But if the voltage and power are the same, how does relate to what we're talking about? We want the 100% duty cycle so we can compare 43.2 volts to 21.6, not so we can compare 21.6 to 21.6. running at 43.2 volts (100% duty) will end with about half the current draw on the same motor.
```

---
## \#58 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:27:44.098Z Reads: 260

```
Because the load's resistance must change if we want the same power with the voltage changing over the load.
I can provide a circuit example of this if needed.
```

---
## \#59 Posted by: Jinra Posted at: 2016-08-07T07:29:56.423Z Reads: 258

```
I guess I'm speaking in more real world scenarios. Keep the motor static, it does not change, and compare the same rider/board going up the same hill. You don't conceded that you'll draw less amps running 12s vs 6s?
```

---
## \#60 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:31:17.610Z Reads: 265

```
If you don't run the 12S at 50% pwm, so it behaves like an 6S would then it will use more power, and go faster up the hill.
```

---
## \#61 Posted by: Jinra Posted at: 2016-08-07T07:34:27.679Z Reads: 269

```
It may use more power (watts), but I'm talking about amps. I imagine it'd draw less. This is the basis for a lot of higher voltage setups.
```

---
## \#62 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:41:23.134Z Reads: 261

```
This has now become the http://www.electric-skateboard.builders/t/hummie-vs-devin-volts-conversion-to-amps/6910/142 topic.

But all in all it can be summarised in this
[quote="devin"]
[quote="SimosMCmuffin"]
DC side - AC side
Steady-Steady [terminology]
10V 1A - 1V 10A

Pulsed-Pulsed [terminology & reality]
10V 10A 10% - 10V 10A 10%
[/quote]

See how those values flip in the steady-steady example but stay the same in the pulsed-pulsed. The terminology confuses people.
```

---
## \#63 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:46:48.269Z Reads: 246

```
If you have the same battery energy capacity and the power stays the same, it will empty that battery in the same time without care for the amps if the power is the same.
```

---
## \#64 Posted by: Jinra Posted at: 2016-08-07T07:48:46.331Z Reads: 245

```
Then I guess we're assuming variable power as well. The main point of stating that higher voltage leads to less amps is so people don't burn out their components with heat. This is something I still believe.
```

---
## \#65 Posted by: SimosMCmuffin Posted at: 2016-08-07T07:56:08.501Z Reads: 251

```
Ok. This is only applicable with the MOSFETs heat loss and **not** the motor's heat loss. The ESC will run cooler with a high voltage battery and low kV motor. If you don't change the motor's kV, but up the voltage then you also increase the amperage and increase the I^2*R power losses in the MOSFETs because your load resistance stays a constant.

All in all, I don't understand why people don't use math to prove they're right... I am a student at a university in Finland, studying for my bachelor's degree to become an electronics engineer. I also have a long time of electronics hobbying under my belt so I know how to use the math to prove my points.
```

---
## \#66 Posted by: lowGuido Posted at: 2016-08-07T08:03:49.596Z Reads: 245

```
yeah @SimosMCmuffin is right. a lot of people throw around the "more volts is less amps" line around here and its not entirely true.

in most of our cases more volts does work out to be less amps because we also run lower kv motors with the more volts. and that is not to be overlooked.
```

---
## \#67 Posted by: Jinra Posted at: 2016-08-07T08:05:47.252Z Reads: 245

```
I mean, I did mention that it is somewhat of a misconception way earlier in the thread.
```

---
## \#68 Posted by: lowGuido Posted at: 2016-08-07T08:08:48.594Z Reads: 249

```
the equations become incredibly complex once you add variable throttle and wave duty cycle into the mix.

but it is safe to say as far as our build are concerned you can use the **rule of thumb** that more volts will lead to less amps.
```

---
## \#69 Posted by: SimosMCmuffin Posted at: 2016-08-07T08:13:40.468Z Reads: 260

```
Then why did you still use flawed examples, which I proved to be wrong?

[quote="Jinra, post:59, topic:7246, full:true"]
I guess I'm speaking in more real world scenarios. Keep the motor static, it does not change, and compare the same rider/ **board**_(<- same motor kV)_ going up the same hill. You don't conceded that you'll draw less amps running 12s vs 6s?
[/quote]

[quote="Jinra, post:57, topic:7246, full:true"]
But if the voltage and power are the same, how does relate to what we're talking about? We want the 100% duty cycle so we can compare 43.2 volts to 21.6, not so we can compare 21.6 to 21.6. **running at 43.2 volts (100% duty) will end with about half the current draw on the same motor.**

_(yes, but on a half a lower kV motor)_
[/quote]

[quote="Jinra, post:54, topic:7246, full:true"]
I mean.. I don't think it would. **I did a calculation on my 200kv chaka motors at 6s and got 197 on one of them. I tested another 200kv chaka motor on 10s and got 194.** So it doesn't seem to have any effect on kv, and if there is, it's very minor. 

_You would have also been pulling more power -> amps, as your winding resistance doesn't change_
[/quote]
```

---
## \#70 Posted by: SimosMCmuffin Posted at: 2016-08-07T08:44:31.044Z Reads: 249

```
I fully admit to being a dick, but I'm the _good_ kind.

If you have false understanding of how things work and you go ahead to a practical testing, you will not get the results you expect to get. I'm here to explain why you're wrong and I use example calculations to prove it. It's a dickish thing to do, but it will save you from unwanted monetary/time investments when you then have to buy the right components to get the expected results, or use time to setup your gear in the right way.

I'm being a dick, for your own good. If you can't think rationally and analytically enough and when someone argues with the correct math behind him/her. Do you get angry or do you thank the person for saving you from useless purchases or needless work?
```

---
## \#71 Posted by: onloop Posted at: 2016-08-07T10:09:30.186Z Reads: 252

```
[quote="evoheyax, post:29, topic:7246"]
12s seems to me to be the best if you can do it in terms of lowering heat in your vesc, and maximizing torque.
[/quote]

YES, higher voltage can = lower current! But just increasing voltage and ignoring other factors doesn't guarantee lower current or less heat.

Because high current/heat in the motor is determined by increasing load. So you must consider that the voltage, motor kv and gearing together decide what current you need for a given amount of torque. Higher gearing reduction mechanically amplifies torque, which reduces load & current & heat.

So actually what is most important is to design a drive system optimized for your desired max speed, which should be the maximum speed the motor can reach with the available battery voltage. Also, it's worth noting that simply running high voltage and only using half throttle doesn't help. 

if you gear for high top speed (or use high kv hub motors) the losses will be higher even at low speed since current is what causes the heat, and at low speed you will have higher current and lower motor voltage for a given torque than you would with gearing for lower top speed.

People need to start thinking about esk8 system not as sperate unrelated components, they must design and build complete system that are designed for optimal performance & ideally aesthetics and practicality too
```

---
## \#72 Posted by: jrpwit Posted at: 2016-08-07T10:20:05.038Z Reads: 240

```
Couldn't have said that better myself! For example, 8s and 245 kv with 14 and 36 teeth and 83mm wheels will give you the same top speed as a raptor (10s, 190kv, 15 and 36 teeth, 83m wheels) but at the cost of higher rpm. High rpm is inefficient and therefore the raptor would be the better setup. The only benefit to the 245kv setup would be that you would have the benefit of having a much higher top speed is you when 12s but again there is high rpm. In the end, the raptor is more efficient than the 8s 245kv setup.
```

---
## \#73 Posted by: SimosMCmuffin Posted at: 2016-08-07T10:36:22.090Z Reads: 239

```
Exactly!

It's too bad that people get confused with this stuff.

For example my current board specs are:
4S, 149kV, 19T MG, 30T WG and 80 mm diameter tires and I get about 21 km/h on flat at 100% duty

I have a metal MG (motor gear) planned with only 15T, so I would expect my top speed to drop to:
v = (15T / 19T) * 21 km/h = 16.6 km/h or a bit higher due to more mechanical torque due to higher gearing, but because ~17 km/h is too slow even for me, I'm going to upgrade the battery to 6S to get more top speed.

And then accounting the new battery voltage my new top speed would be:
v = (6S / 4S) * 16.6 km/h = 24.8 km/h or a bit lower as the needed torque increases. So I'll be using more power in total to run, but at higher speed.
```

---
## \#74 Posted by: devin Posted at: 2016-08-07T12:54:43.228Z Reads: 234

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#75 Posted by: Workaround Posted at: 2016-08-07T12:55:51.469Z Reads: 234

```
If that is true then that means 12s is not efficient for the VESC cause the difference in in efficiency because of heat dissipation is around 15-18%(only 65% efficient) slower speeds. It was off by 3 miles from what you said you got with 10s(this with 80% efficiency cause of load).
```

---
## \#76 Posted by: chaka Posted at: 2016-08-07T15:00:10.445Z Reads: 238

```
You will be fine if you have low enough KV.  I ride a 12s everyday on the om5065 200kv motors but they are actual 200kv windings. I have seen a lot of other motors with higher kv values than advertised so be sure your erpm does not get too high.
```

---
## \#77 Posted by: Blacksheep Posted at: 2016-08-07T17:01:09.805Z Reads: 232

```
Yes mine says it's a sk3 149kv or I could use the motors I got from you. Thanks
```

---
## \#78 Posted by: Namasaki Posted at: 2016-08-07T17:28:43.145Z Reads: 230

```
[quote="evoheyax, post:29, topic:7246"]
why does everyone seem to ignore 11s?
[/quote]

I don't think anyone makes a BMS for 11s
```

---
## \#79 Posted by: Jinra Posted at: 2016-08-07T17:33:34.333Z Reads: 232

```
bestech does! http://www.bestechpower.com/407v11spcmbmspcbforli-ionli-polymerbatterypack/BMS-D163.html
```

---
## \#80 Posted by: CSN Posted at: 2016-08-07T17:34:32.889Z Reads: 241

```
https://www.youtube.com/watch?v=KOO5S4vxi0o
```

---
## \#81 Posted by: Namasaki Posted at: 2016-08-07T17:37:14.767Z Reads: 245

```
[quote="chaka, post:76, topic:7246"]
I ride a 12s everyday on the om5065 200kv motors
[/quote]

You posted this chart previously based on the Vesc having a 60000 erpm limit.
8570 RPM
---------------/50v = 170kv - 12s
---------------/42v = 200kv - 10s
---------------/33v = 260kv - 8s
---------------/25v = 340kv - 6s
What changed?
```

---
## \#82 Posted by: Namasaki Posted at: 2016-08-07T17:45:24.010Z Reads: 245

```
Bestech is the best!
```

---
## \#83 Posted by: chaka Posted at: 2016-08-07T18:17:57.700Z Reads: 253

```
Those numbers are for maximum reliability. Personally I wouldn't go this high on 12s with larger motors, I was getting faults with 200kv maytech motors. 200kv at 12s is still risky business on smaller motors if you gearing is too low, it can be very easy to overrun the erpm on hills if you electrical top speed is only 20-25mph.

@Blacksheep 149 sk3's are great at 12s but you will want to keep your gear ratio low or you could overheat the VESC when climbing. What tooth # are you running on your pulleys?
```

---
## \#84 Posted by: Namasaki Posted at: 2016-08-07T18:22:45.185Z Reads: 255

```
Ok, Thanks for the clarification.
As for me, I'll stick to the chart and play it safe.
```

---
## \#85 Posted by: Blacksheep Posted at: 2016-08-08T08:35:32.301Z Reads: 248

```
I'm using 15/36
```

---
## \#86 Posted by: chaka Posted at: 2016-08-08T13:30:24.726Z Reads: 250

```
If you are running 83mm wheels you should be OK on moderate hills but you may overheat on 90's.
```

---
## \#87 Posted by: Blacksheep Posted at: 2016-08-08T16:55:41.530Z Reads: 259

```
I do have 83 wheels
```

---
## \#88 Posted by: hatsunearu Posted at: 2016-10-30T05:41:19.778Z Reads: 237

```
OK apparently you guys don't get why there is a disparity between the resistance calculations. You forgot to account for back EMF. 

21.6V @ 54A

43.2V @ 27A

since we don't know the rotational velocity we can't assume that the back emf for both test cases are equal, but let's just assume they are for the sake of demonstration. 

| Rdc + jw1L | = (21.6 - KB*w1) / 54A
| Rdc + jw2L | = (43.2 - KB*w2) / 27A

(KB*w) is the back EMF. You can probably solve that and obtain a value for |Rdc + jwL| and (KB*w) assuming w1 = w2. 

And on that related note. Higher battery voltages will do the following:

* For a given output motor voltage and current, a higher battery voltage will draw less *BATTERY* current. (Explanation for experts: the controller acts like a buck converter, and having a higher input voltage for a given output voltage and current means you will be drawing less source current) Another way of looking at this is if you are limited by battery current in a certain load scenario, higher voltages will solve this. 

* Higher battery voltages will let you achieve higher motor voltages. (maximum output of a buck converter is 100% duty cycle so Vout = Vin) Another way to look at this is if you are limited by motor voltage in a certain load scenario, higher voltages will solve this.

For the first case, the only time this will be an issue is perhaps at stall/startup or at some point in the acceleration profile. But this will likely be a very short transient in your acceleration profile so unless you're doing some crazy drifts or something will likely not affect you other than slightly slowing your 0-30mph time or whatever metric fancies you. And from what it looks like nobody is really limited by battery current anyways.

For the second case, whenever you hit 100% duty cycle, that's basically when you're motor voltage limited. If you're not satisfied with the performance you get when you put 100% duty cycle and whatever you get from your contraption, having a higher battery voltage will help.

It's infuriating to see how ignorant hobbyists are and base their understanding on extremely rudimentary electrical models like "P=IV". BLDC motors are extremely complex and what I described is barely opening the can of worms. 

People spend their entire lives optimizing motors, and some other people spend their lives making incredible VVVF drives. Electric skateboards combine those two together and there is so much to discover. Please don't limit yourself with "ohm's law" and call it a day.
```

---
## \#89 Posted by: Acidfie Posted at: 2018-03-30T19:05:54.453Z Reads: 156

```
sorry to geht this thread up here but im just curious about the 12S thing.

I am currently running 10S3P and just bought 50 30Q cells..

so i am thinking of 12S4P or 10S5P, and i really cant decide. Is it a safe option or is it really pushing the limits? i am suing esk8 VESC 1.1

maybe @esk8 did some testing with 12S? a 190KV motor should be fine or am i wrong?
```

---
## \#90 Posted by: Sender Posted at: 2018-03-30T19:28:21.135Z Reads: 158

```
I too would like to hear the latest thoughts on this, and am having similar internal debates. Especially now that people have been running 12s for a while now. I was also thinking about ordering a couple 11s D140 BMSs from Bestech amd splitting the difference.  I am using 190 kv BTW.
```

---
## \#91 Posted by: SORRENTINO Posted at: 2018-03-30T19:32:03.816Z Reads: 154

```
12s for the win. Less current more range...190kv perfectly fine in bldc and in FOC no need to worry about erpm limit :slight_smile:
```

---
## \#92 Posted by: Hummie Posted at: 2018-03-30T19:38:17.981Z Reads: 154

```
or probably less range as youre riding further from the no-load speed (if youre going faster you'll have less range as well), likely putting out more power at the slow speeds too (just cause everyone cant help themselves with more power potential), and while the true wiring may be a bit more efficient with less battery amps needed I think the esc will also be a bit less efficient as it's probably going to be operating also further from the no-load speed and have more switching.
```

---
## \#93 Posted by: bimmer Posted at: 2018-03-30T20:47:06.574Z Reads: 151

```
because I can run 57V without breaking mine.
```

---
## \#94 Posted by: DeathCookies Posted at: 2018-03-30T21:24:57.841Z Reads: 152

```
I am running since a year on FOC without problems. It is just better and i would not go any voltage lower :D
```

---
## \#95 Posted by: Acidfie Posted at: 2018-03-30T21:34:06.017Z Reads: 150

```
Which VESC using?
```

---
## \#96 Posted by: pat.speed Posted at: 2018-03-30T23:38:28.113Z Reads: 150

```
12s for the win. Just limit the erpm to 60k for 190kv and your all good. 

I will be using an extra cap bank to smooth voltage spikes. 63v 19800uf bank for the win
```

---
## \#97 Posted by: Deckoz Posted at: 2018-03-31T01:34:13.394Z Reads: 155

```
You've tried 14s Lion/16s LiFePO4?
```

---
## \#98 Posted by: b264 Posted at: 2018-03-31T02:21:31.451Z Reads: 153

```
[quote="Acidfie, post:89, topic:7246"]
so i am thinking of 12S4P or 10S5P, and i really cant decide.
[/quote]

Easy, 10S5P.  More range and less failures.  Done deal
```

---
## \#99 Posted by: Acidfie Posted at: 2018-03-31T09:44:00.469Z Reads: 147

```
The range will only differ about 2km if I use 12S or 10S.. that’s why I want 12S because my board feels very slow..
```

---
## \#100 Posted by: ervinelin Posted at: 2018-03-31T09:59:32.775Z Reads: 149

```
Does going from 10 to 12S only change top speed or does it change acceleration characteristics?

I too am planning between 10 or 12S for a MTB build.
```

---
## \#101 Posted by: pat.speed Posted at: 2018-03-31T10:02:25.066Z Reads: 151

```
Yes, I’ve heard it also increases acceleration and torque
```

---
## \#102 Posted by: b264 Posted at: 2018-03-31T11:45:16.480Z Reads: 150

```
[quote="Acidfie, post:99, topic:7246"]
The range will only differ about 2km if I use 12S or 10S
[/quote]

That's not entirely true.  That's only the electrical characteristics and not the human characteristics.  If you have more power it's a lot easier to waste more energy accelerating faster, which will cripple your range faster than anything else.  So the 12S will have a shorter range than the 10S range less 2km

It's easier to drive 10S more efficiently than 12S, though it's physically possible to drive more efficiently with 12S, if unlikely.  It's the difference between "possible" and "easy"
```

---
## \#103 Posted by: Acidfie Posted at: 2018-03-31T16:33:32.515Z Reads: 145

```
but the board will also be more efficient
```

---
## \#104 Posted by: Hummie Posted at: 2018-03-31T16:43:52.246Z Reads: 149

```
maybe could be more efficient but I think most of the losses are in the motor and if you ride around at 20mph with 10s and have a 20 mile range, and then ride around on 12s doing the same 20mph you'd have slightly less range.  you can look at the grin tech motor simulator and make an even comparison.  

if you want to go faster 12s makes sense but not if you want to stay the same speed
```

---
## \#105 Posted by: Acidfie Posted at: 2018-03-31T18:52:18.405Z Reads: 139

```
i want to go faster thats the thing of it. 

i also think that i can do 20km+ with 12S4P 30Q's. thats all i want to do.
```

---
## \#106 Posted by: professor_shartsis Posted at: 2018-03-31T19:11:30.275Z Reads: 140

```
[quote="Acidfie, post:105, topic:7246, full:true"]
i want to go faster thats the thing of it.

i also think that i can do 20km+ with 12S4P 30Q’s. thats all i want to do.
[/quote]

12S, 190kv, 97mm tire, 1 motor, 57a motor amp limit, 3:1 reduction should be able to top 30mph....

http://vedder.se/forums/viewtopic.php?f=6&t=1675

http://tppsf.com/48v-190kv-3.jpg
```

---
## \#107 Posted by: bigben Posted at: 2018-03-31T19:16:06.410Z Reads: 134

```
I think you need to get to the bottom of why your setup doesn’t go as fast as it should. 
You have 10s4p, twin 6365 motors. 83mm wheels 15/35 pulleys. You should be getting a lot more than 30kmh. 
Either your KV of the motors is way off or you’re losing power somewhere.
```

---
## \#108 Posted by: Acidfie Posted at: 2018-03-31T19:20:30.575Z Reads: 130

```
yeah it could be, it just doesnt feel as fast. i really need to check the kph. maybe i have the 36T pulley.. 10s3P but that doesnt even matter in this case. 



@professor_shartsis i meant range, not speed.
```

---
## \#109 Posted by: professor_shartsis Posted at: 2018-03-31T19:23:15.563Z Reads: 133

```
same **constant** speed should mean same constant motor amps and effective voltage from the controller, and same torque and rpm (mechanical power) from the motor, and therefore the same electrical to mechanical  conversion efficiency in the motor regardless of whether you choose 10S or 12S. on the battery side the higher amps from the 10S would lead to slightly greater power losses in the battery wires for the same **acceleration** performance, since losses are proportional to the amps squared times the resistance.

at 12S with the same battery and motor amp limits, the controller could allow more watts to the motor at the same rpm during acceleration (same battery amps at higher voltage is more watts), and faster acceleration lowers efficiency.
```

---
## \#110 Posted by: bigben Posted at: 2018-03-31T19:28:08.719Z Reads: 137

```
![image|281x500](upload://ywsnRuipzh1mO5OfPgQSFBAIlb9.png)
This should be the sort of performance you should get.
```

---
## \#111 Posted by: Acidfie Posted at: 2018-03-31T19:45:26.987Z Reads: 128

```
yeah this could be, speed is a thing someone gets used too very fast. i think 35 kph should be the right value.

still i want to get to 50 kph, thats why i think of 12S or 10S with other gearing but i think i might loose torque


like where do i make a cut when it comes to speed.. 12S with higher gearing ratio or 10S with lower gearing ratio? where is the line
```

---
## \#112 Posted by: professor_shartsis Posted at: 2018-04-01T18:05:02.156Z Reads: 112

```
you can increase the top speed of a 10S system with a couple extra teeth on the motor pulley and raising the battery & motor current limits, but this will produce more heat in the motor and esc.
```

---
## \#113 Posted by: Hummie Posted at: 2018-04-01T18:42:54.680Z Reads: 115

```
[quote="professor_shartsis, post:109, topic:7246, full:true"]
same constant speed should mean same constant motor amps and effective voltage from the controller, and same torque and rpm (mechanical power) from the motor, and therefore the same electrical to mechanical  conversion efficiency in the motor regardless of whether you choose 10S or 12S. on the battery side the higher amps from the 10S would lead to slightly greater power losses in the battery wires for the same acceleration performance, since losses are proportional to the amps squared times the resistance.

at 12S with the same battery and motor amp limits, the controller could allow more watts to the motor at the same rpm during acceleration (same battery amps at higher voltage is more watts), and faster acceleration lowers efficiency.
[/quote]
http://www.ebikes.ca/tools/simulator.html/?bopen=true&k=2&k_b=1&throt=100&hp=0&hp_b=0&throt_b=96
here two motors with one double the kv and not the same efficiency at the same speed

heres the same with a bigger load
http://www.ebikes.ca/tools/simulator.html/?bopen=true&k=2&k_b=1&throt=100&hp=0&hp_b=0&throt_b=53&grade=5&grade_b=5
way more motor amps needed by the higher kv

and here's with not changing the kv but changing the battery
http://www.ebikes.ca/tools/simulator.html/?bopen=true&k=1&k_b=1&throt=100&hp=0&hp_b=0&throt_b=56&grade=5&grade_b=5&batt=B3612_SLA&batt_b=B4812_SLA
closer but still the range shrinks with the higher battery

and heres a bigger load
http://www.ebikes.ca/tools/simulator.html/?bopen=true&k=1&k_b=1&throt=100&hp=0&hp_b=0&throt_b=42&grade=9&grade_b=9&batt=B3612_SLA&batt_b=B4812_SLA

don't see them as equal efficiency and everytime the higher kv or battery voltage is worse efficiency
```

---
## \#114 Posted by: professor_shartsis Posted at: 2018-04-01T18:57:41.759Z Reads: 117

```
[quote="Hummie, post:113, topic:7246"]
don’t see them as equal efficiency and everytime the higher kv or battery voltage is worse efficiency
[/quote]

for the same electrical to mechanical conversion efficiency at the same speed with the same # of motor amps with higher kv one would need to either decrease tire diameter or increase gear reduction for example by choosing a motor pulley with less teeth.

i suspect the lower efficiency in your simulation with higher voltage is caused by the higher internal resistance of a higher voltage battery pack and not caused by esc or motor losses.
```

---
## \#115 Posted by: Hummie Posted at: 2018-04-01T18:59:44.297Z Reads: 115

```
it also shows if you change just the kv
```

---
## \#116 Posted by: professor_shartsis Posted at: 2018-04-01T19:03:40.253Z Reads: 117

```
right, to compensate for the lower torque at the motor with higher kv (same motor amps), you have to adjust the gearing such that you end up with the same torque at the wheel for equal performance and efficiency with both kvs.
```

---
## \#117 Posted by: Acidfie Posted at: 2018-04-01T19:26:20.163Z Reads: 113

```
i want to move the discussion on here: http://www.electric-skateboard.builders/t/more-speed-12s-or-lowering-gearing-ratio/50859
```

---
## \#118 Posted by: lazerusrm Posted at: 2018-04-02T17:55:28.565Z Reads: 108

```
the higher voltage you run, the more efficient your setup will be because you draw less amps, and experience less loss through cables, batteries, motors, etc.

it's the same reason high voltage power lines exist, you can move more power, with less losses. 

The only issue is long wire inductance, voltage spikes, and whether your ESC can survive 12s daily.
```

---
## \#119 Posted by: Hummie Posted at: 2018-04-02T23:43:42.867Z Reads: 106

```
 the power lines use high voltage to transmit power more efficiently but you cant get a more efficient motor running higher and higher voltage.   in the motor the amps and volts it gets isn't even what would show on a watt meter coming from the battery.    if you were to run a motor at a much higher voltage you will end up using more "motor amps" to get the torque for the same performance.   The higher voltage will give you more inefficiency for the same performance as the lower voltage.   

but that's using grin motor simulator you can find and I'm not sure if it shows for the whole vehicle including all electronics in its output.  maybe its just the esc that creates the increased loss with higher voltage but don't think so
```

---
## \#120 Posted by: Blitz Posted at: 2018-04-02T23:59:37.068Z Reads: 107

```
I thought Powerlines use higher voltage because You would need huge wires to carry all the amperage.
```

---
## \#121 Posted by: Deckoz Posted at: 2018-04-03T00:06:33.343Z Reads: 108

```
First clue..

Power lines aren't 120/240v 

;)

That is a product of transformers...
```

---
## \#122 Posted by: Blitz Posted at: 2018-04-03T00:06:56.703Z Reads: 104

```
I know.

10char
```

---
## \#123 Posted by: lock Posted at: 2018-04-03T00:41:55.809Z Reads: 108

```
[quote="Hummie, post:119, topic:7246"]
maybe its just the esc that creates the increased loss with higher voltage but don’t think so
[/quote]

No, ESC is probably more efficient with higher voltage too. Provided you don't blow it up...

> A test bed able to record efficiency of an ESC was constructed with limitations. Data was
taken to observe the effects of torque, speed, voltage, switching frequency, and ESC size.
It was deduced that the greatest efficiencies are gained for low torque, low speed loads and
efficiency reduces significantly with torque. *It was seen that higher voltages have higher
ESC efficiency at all throttles.*

From [here](http://digitalcommons.calpoly.edu/cgi/viewcontent.cgi?article=2617&context=theses).

Slowly coming to the opinion we should all be running high RPM/low torque setups with some big gear reductions.
```

---
## \#124 Posted by: Battosaii Posted at: 2018-04-03T00:45:28.250Z Reads: 107

```
I've been running 12s on my focbox for a couple hundred miles now with no problems I like the power you get with 12s. 10s is not bad though though my old 10s board that I thought was too fast now feels slow.
```

---
## \#125 Posted by: lazerusrm Posted at: 2018-04-03T00:52:32.201Z Reads: 109

```
The point is 12s is going to be more efficient than any other (lower) battery voltage.

less amps means less losses through the power system, simple as that.

look at EVs.. they use hundreds of volts. My point is more volts is more efficient at transferring power which is exactly what you're doing in a esk8.
```

---
## \#126 Posted by: Hummie Posted at: 2018-04-03T06:00:25.156Z Reads: 112

```
if youre going 20mph TOP SPEED with 10s if you then switched to 12s and went the same 20mph with reduced throttle and power output it seems it will be less efficient according to the grin motor simulator.  @lock 's paper says running higher voltages is more efficient but at the same time if youre then forced to be running at a low throttle because your no-load speed is higher with the higher voltage, then there's the losses there from running at lower throttle.   if you were to change your gearing in the scenario above so then running 20mph as the top speed with the 12s then it would be most efficient.
```

---
## \#127 Posted by: Acidfie Posted at: 2018-04-03T07:10:41.662Z Reads: 108

```
still the question is where to cut the line between 12S and reducing gearing ratio?
```

---
## \#128 Posted by: professor_shartsis Posted at: 2018-04-03T07:22:48.194Z Reads: 109

```
100kv motor a - 900rpm:
(10v battery - 9v bemf) / 0.1ohm = 10a motor current

100kv motor b - 9900rpm:
(100v battery - 99v bemf) / 0.1ohm = 10a motor current

same motor current so both have the same torque, same copper loss & same ohmic heating. motor b has 11 times greater angular speed than motor a, and the same torque so motor b is producing 11 times as much mechanical power as motor a, but copper loss is the same. which is more efficient?
```

---
## \#129 Posted by: Acidfie Posted at: 2018-04-03T13:10:00.922Z Reads: 100

```
what about more motor kV? beside gearing ratio?

this problem is still questionable for me
```

---
## \#130 Posted by: Pedrodemio Posted at: 2018-04-03T13:37:07.434Z Reads: 95

```
For a given motor geometry with the same amount of copper used in the winding, the motor performance will be the same no matter how you wind it, more turns of thinner wires or less with thick ones, the only thing that changes is that the maximum efficiency and peak torque occur at different voltage/current  combination

This is due to the max current density( A/mm^2) being the same for different windings, more than that and you start to saturate the laminations and the efficiency drops a lot

What you need to do is to pair the winding with the available voltage you have for driving the motor, this way you can keep the flux at max (max torque production)
```

---
## \#131 Posted by: Acidfie Posted at: 2018-04-03T13:45:15.305Z Reads: 110

```
how to determine this?

see, i can easily go 12S4P but why should i if i can do a 10S5P with a higher kV and get the same result in speed.. thats what i am thinking right now
```

---
## \#132 Posted by: Deckoz Posted at: 2018-04-03T14:39:16.229Z Reads: 113

```
I'm just gonna say..

12s4p.. 48 cells, was averaging 21 miles of range on a 30q

Pshaw Evo, 13s4p, 52 cells, averages 27 miles, a third more milage almost, for 4 more cells...

My Evo 13s5p, 65 cells, - only 17 more cells not half more, I average 43 miles a charge.. double the range...

Both 190kv 6374

Math that....and tell me higher voltage is less efficient. I'll wait patiently lol.
```

---
## \#133 Posted by: Acidfie Posted at: 2018-04-03T14:53:04.081Z Reads: 112

```
I just did some research and i came to this conclusion:

I read all time about the fact that motors with a higher kv have lower torque, which is definitely wrong. So here are some facts about these kind of motors:

kv means RPM per Volt, which we all know. the reciprocal is km, were km = 9.55/kv, unit Nm/A.

km is the unit that determines how much torque (Nm) per 1A the motor produces. 
motors with **less kv** do produce **more Nm per 1A** than motors with higher kv

which means: **motors with high kv need more amps to produce the same amount of torque**

this is why high kv motors need more amps than motors with less kv. this is for every brushless motor regardless of the power output - 10W or 10kW.
a motor with more poles does not have higher torque than a motor with less poles (same voltage, rpm and amp)

example:

Kontronik Pyro 700-45, amp consumption 13A, 10 Poles, 0,3Nm approx. 16000 rpm. outrunner

Lehner 2230/40, amp consumption 13A, 2 Poles, 0,3Nm approx. 18000 rpm. inrunner

used with 10S 36V nominal

Torque cant be compared with the count of poles, torque originates from the air gap between rotor and stator. the distance for the leverage condition between rotor and stator is greater when it comes to outrunners which means more torque. (in case of winding construction)


straight to @Deckoz 

i never said high voltage is less efficient -  the question hereby is: 

Maxing out Voltage VS. Reducing gearing ratio VS. upping kv - the most efficient of those combinations when it comes to: **Speed - Range - Torque**

see, if i would go for 12S, and want 50 kph topspeed: should i lower my kv and get a higher gearing ratio OR should i up my kv and lower my gearing reduction.

this calculations should be done with the maximum providable power of the vesc or the battery..
```

---
## \#134 Posted by: Hummie Posted at: 2018-04-03T15:16:38.864Z Reads: 104

```
what you write sounds good but it's kv and kt are reciprocal.  km shows the relationship of torque to heat which would show what motor is more efficient.  as @Pedrodemio was saying and you have to pair the battery with the kv.  you don't want a no-load speed that's far off in the distance that you don't go to...then you'll be inefficient.    why exactly?...and is it inefficiency in the motor or just the esc in such a situation where youre forced into less than highest duty cycle.
```

---
## \#135 Posted by: Pedrodemio Posted at: 2018-04-03T15:26:41.665Z Reads: 106

```
Km is wrong in the concept, it is torque for a given current divided by the square root of the current for this given torque squared times winding resistance, in other words Km = T/((R*I^2)^1/2)

Comparing motors using Kt or Kv is deceiving. Yes, you increase the the torque for a given current, but not for the absolute torque the motor can produce

That's called the Ni constancy, if you increase the number of turns, you use thinner wires, so the absolute current must go down, the works the other way, if you lower the number of turns you get a higher Kv but the wire must get thicker to maintain the slot fill, so you can pump more current and get the same torque, **you can't change N without changing i**

Back to Km, the formal definition is air gap flux density times rotor inside radius ( for outrunners) times square root of wire volume in a slot all divided by square root of resistivity, all this is independent of number of turns, Kv or Kt

A given motor geometry with the same cooper fill will have the same performance
```

---
## \#136 Posted by: professor_shartsis Posted at: 2018-04-03T15:34:11.204Z Reads: 108

```
km is the same:

100kv - 10 turns - 1 cross section - 0.1ohm
60/(2 * pi * 100kv)=0.09549296585513720146133 newton meters torque per motor amp
(4v battery - 0v bemf) / 0.1ohm = 40a motor & battery current at 0rpm
4v * 40a = 160w electrical
40a * 0.09549296585513720146133nm/a = 3.819718634205488058453nm
3.819718634205488058453nm / sqrt(160w electrical) = **0.3019752726269222102173km**

200kv - 5 turns - 2 cross section - 0.025ohm
60/(2 * pi * 200kv)=0.04774648292756860073067 newton meters torque per motor amp
(4v battery - 0v bemf) / 0.025 ohm = 160a motor & battery current at 0rpm
4v * 160a = 640w electrical 
160a * 0.04774648292756860073067nm/a = 7.639437268410976116907nm
7.639437268410976116907nm / sqrt(640w electrical) = **0.3019752726269222102173km**

^km (torque per square root of watt) is the same

---------

1:1 gearing - 10mph ground speed
100kv - 10 turns - 1 cross section - 0.1ohm
1000rpm = 104.719755 radians per second
(11v battery - 10v bemf) / 0.1ohm = 10a motor/battery current
torque per amp: 60/(2 * pi * KV) = 0.095492nm/a
10a * 0.095492nm/a = 0.95492newton meters torque
11v battery * 10a current = **110w electrical**
0.95492newton meters torque * 104.719755 radians per second = **99.99w mechanical**
copper loss: 10a * 10a * 0.1ohm = **10w**
wheel torque at 10mph @ 110w electrical = 0.95492nm * 1 gear reduction = 0.95 newton meters
summary: **10mph ground speed**, **0.95nm wheel torque, 99.99w mechanical, 110w electrical, 10w copper loss**

2.150:1 gearing - 10mph ground speed
200kv - 5 turns - 2 cross section - 0.025ohm
2150rpm = 225.14747 radians per second
(11v battery - 10.75v bemf) / 0.025ohm = 10a motor/battery current
torque per amp: 60/(2 * pi * KV) = 0.047746nm/a
10a * 0.047746nm/a = 0.47746 newton meters torque
11v battery * 10a current = **110w electrical**
0.47746 newton meters torque * 225.14747 radians per second = **107.49w mechanical**
copper loss: 10a * 10a * 0.025ohm = **2.5w**
wheel torque at 10mph @ 110w electrical = 0.47746nm * 2.15 gear reduction = 1.02 newton meters
summary: **10mph ground speed**, **1.02nm wheel torque, 107.5w mechanical, 110w electrical, 2.5w copper loss**

^same ground speed, same voltage battery, same battery current and motor current, different gearing & the higher kv appears more efficient... it would seem if the 100kv is at constant speed @ 10mph from the load, with the same ground speed & load the 200kv is still accelerating because there is more torque at the wheel...
```

---
## \#137 Posted by: Acidfie Posted at: 2018-04-03T16:34:37.917Z Reads: 104

```
yeah i meant kt, had to translate from german, my bad.

@professor_shartsis yep, that is now the calculation for different amounts of kv, it seems that staying with higher kv would be the better idea.

but what about the difference between:

Therefor given:

10S5P = Cont. Discharge approx. 100 amp
12S4P = Cont. Discharge approx. 80 amps

**staying at low kv** and **adding more voltage** (+2S) 
(higher current delivery without losses to heat)

VS.

**staying at 10S** and **adding more kv**
(higher max. discharge current, but losses to heat e.g.)

since it is clear the continuous discharge current will never be over 60 amps, but what about the maximum current provided when accelerating with:

a) higher kv, lower voltage, greater amp supply from the battery
b) lower kv, higher voltage, lesser amp supply from the battery

when it comes to efficiency?

it seems in my eyes that staying at 190kv, going 12S and 36/15 gearing seems **the best and efficient scenario** or **does anyone recommend another option** ?
```

---
## \#138 Posted by: Hummie Posted at: 2018-04-03T16:52:47.122Z Reads: 103

```
But is it an inefficiency in the motor w a poorly paired kv n voltage and if so why?

I've seenthe same motor w different windings and kv having different stated lower output with the lowest kv stated as least powerful and it seems when u add many many turns, and are trading speed for torque output you lose some of the max potential power. So have the same copper and iron but lesser performance. Just how a hub motor has to be bigger for same power compared to the motor w a pulley.
I think only way to more efficiency as compared to what u last wrote would be to lower the top speed.  Or reduce performance by decreasing amp output to the motor. Probably the motor amps.  Why are motor amps considered more inefficient than battery amps,,,or are they not?
```

---
## \#139 Posted by: Acidfie Posted at: 2018-04-03T17:14:22.813Z Reads: 98

```
the target is to reach 50 kph with the **most efficient setup**, not to be more efficient driving at slower speeds.

it doesnt seem that you lose torque while going to 12S, while you will definitely lose torque with higher kv **if not delivering more amps to your motor** - which can be limited by your battery settings. 

well, why should i power a motor with 60a if my battery only can deliver 40 continuously?

slowly it seems i can't really get a correct answer here in this thread either if i should go with 12S or adding kv.
```

---
## \#140 Posted by: professor_shartsis Posted at: 2018-04-03T18:16:59.594Z Reads: 98

```
[quote="Acidfie, post:139, topic:7246"]
well, why should i power a motor with 60a if my battery only can deliver 40 continuously?
[/quote]

60a “motor amps” continuosly to the motor draws varying amounts of “battery amps” depending on the present angular speed of the motor.... less “battery amps” for 60a motor amps at low rpm and more battery amps at higher rpm for the same constant 60a “motor” amps... 60a motor amps will draw nearly 60a battery amps when you are very close to the peak power output of your motor when considering the motor amp limit you’ve selected.

also, my earlier equations showing higher efficiency with higher kv assumes 2 things... that the “km” is identical with both kvs, and the gearing is modified with the higher kv... if you had higher kv but lower km, the higher kv might be less efficient, even if you change the gearing.
```

---
## \#141 Posted by: Acidfie Posted at: 2018-04-03T18:40:34.883Z Reads: 98

```
so going with 12S?
```

---
## \#142 Posted by: Hummie Posted at: 2018-04-03T19:27:57.480Z Reads: 97

```
More eff if uadjust top speed w gearing to what it was at 10s.   But assuming u dowqnt that top speed, if u gear it more for lower top speed even more eff
```

---
## \#143 Posted by: Acidfie Posted at: 2018-04-03T19:32:58.649Z Reads: 96

```
i just calc'd it, i need about 32 teeth wheel pulley and about 15 -16 teeth motor pulley.. this sounds to me like a big torque loss if i only could add up 2S more for more rpm at higher speeds
```

---
## \#144 Posted by: professor_shartsis Posted at: 2018-04-03T19:36:04.513Z Reads: 99

```
a motor running with 10S instead of 12S has roughly 80% as much peak mechanical power and rpm with the same motor amp (torque) limit... so onto my question...

at 10s how can he reach the same top speed with a motor delivering only ~80% as much peak mechanical power and rpm but the same amount of copper loss and torque?

gearing can increase torque at the proportional expense of rpm, or increase rpm at the proportional expense of torque. mechanical power is torque in newton meters * angular speed in radians per second. changing the gearing doesn’t change the peak mechanical power output of the motor, unlike changing the voltage or motor amp limit.
```

---
## \#145 Posted by: Hummie Posted at: 2018-04-03T19:45:26.898Z Reads: 94

```
Yea. Les power so less speed.
```

---
## \#146 Posted by: lazerusrm Posted at: 2018-04-04T03:38:37.132Z Reads: 84

```
12s bro no bs. don't understand why this is even a discussion!

ride a 10s set up and ride a 12s setup...  

10s is for ladies who cant handle the power :wink:
```

---

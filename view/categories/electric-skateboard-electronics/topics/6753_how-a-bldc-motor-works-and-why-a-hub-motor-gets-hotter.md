# How a BLDC motor works and why a hub motor gets hotter

### Replies: 75 Views: 9147

## \#1 Posted by: PB1 Posted at: 2016-07-28T08:25:11.822Z Reads: 420

```

Triggered by a number of discussions between @hummie, @devin and @brams and because of science I’m digging into this, making a fool out of myself trying to explain why a hub motor gets warmer than a satellite motor cruising at the same speed. Btw, the short answer up front: because of the lack of gearing!

Disclaimer: I’m not a professional writer nor a teacher. And English is not my first language. Just some dude trying to explain things. I will also have to simplify stuff, hopefully not oversimplifying.  So please be patient with me but step in when I’m wrong. 

How does a BLDC motor work?
First we need to understand how a Brushless DC (BLDC) motor works. Regarding the mechanics a BLDC motor is very similar to a step motor and a synchronous motor and a brushed DC motor. I’m not going to discuss mechanics here for now.

The main difference between the mentioned motors is how they are controlled. Synchronous motors are AC motors. They ran at a frequency set by the AC current supply.  Synchronous motors don’t have much with regards to control as the frequency of the input and thus their RPM is normally given. Under load they still run with the same frequency but increase to draw current. Note: most synchronous machines are used as generators. Actually, all of the synchronous motors can be used as generators. 

Brushed DC motors have the “controller” “build it”. Input into the controller is a DC Voltage. The controller is a mechanical thing with brushes and contact areas. This controller converts the DC input into AC output which is then used as input for the actual motor. This is called commutation and the controller is a commutator. The commutator is a mechanical thing and is actually quiet complex. Because of the brushes and the contact areas it has mechanical wear which is a big disadvantage. 
So the brushed DC motor is actually an AC motor very similar to the synchronous motor. Because overall input is DC it’s called a DC motor. :innocent: 
Speed control is done by varying the input voltage into the system, so by varying input voltage into the commutator. Higher voltage results in higher speed. Under load the motor uses more torque and draws more current. Torque and current are proportional. Btw, more current produces more loss due to heat. 

Now we come to our beloved Brushless DC Motor which is similar to a brushed DC motor … without the brushes :grinning:. 
Or better: without the physical commutator. The physical commutator is replaced with an electronic commutator which normally sits outside of the motor! Same as the physical commutator the electronic commutator (EC) is quiet complex. You guessed it, it’s the ESC. The ESC commutates the DC input into AC output which is then AC input for our motors. 
So our BLDC motors are actually AC motors, only the mostly external ESCs make them DC motors … 
And they are very similar to AC generators. 

How is speed control done in the ESC for our motor? Simple answer is it’s the same as for the brushed DC motor, the ESC varies the motor input voltage. But this is oversimplified. Also as we know the voltage into the ESC is normally fixed. In our case it’s the voltage of the battery.  A technique called pulse width modulation (PWM) is used to create an average voltage into the motor. The higher this average voltage the higher the RPM. Higher average voltage is achieved by wider pulses. All this is calculated by electronics and software. In the VESC we have a chip that does all of the calculations plus we have a driver chip that gets input from the calculation chip and that drives the MOSFETS. The MOSFETS open and close the gates for current and voltage. 
So the voltage going out of the VESC and into the motor is the average voltage produce be PWM and it’s always lower than the voltage going into the VESC. It cannot be higher (unless produced by the motor, we come to that later). 
(note: our RC-style remote receiver controls the throttle of the VESC also using PWM, but this has absolutely nothing to do with this, just the same technique)

Now we have to discuss Kv of a motor. Kv is one motor constant, the motor velocity constant. It is fixed and based on the physical characteristics of the specific motor. 
Kv is two things: 
1)	most people will say that Kv is the RMP per Volt of an unloaded motor. As an example the OllinboardCo OM5065 is a 170Kv motor, so at 10s=37V it will have an RPM of 37V*170RPM/V = 6290 RPM (without load) – this is not the definition of Kv, but it’s almost true, it’s very close. The reason is explained below. 
2)	the exact definition of Kv however is the following: Kv is the reciprocal value of the Ke, the back-EMF constant. Kv = 1 / Ke. The back-EMF is the voltage a motor generates when rotated. So when chakas motor is rotated with 5000 RPM it produces 5000 RPM * 1/ 170RPM/V = 29.4V . Remember? Our motors are also AC generators. 

When does a BLDC motor turn / accelerate? Answer: When the average voltage from the ESC is higher than the generated voltage. Then current starts to flow through the motor. But how much current does flow? This depends a) on the mechanical power needs to be produced by the motor and b) the RPM the motor is currently running and thus the back-EMF in V. This mechanical power is produced by electrical power and is calculated voltage times current -  P = U*I where U is the back-EMF generated by the motor. 
If a motor does not need to produce power it will spin up freely and not much current will flow and the RPM reached is very close to the theoretical maximum  Kv * U . 

If the motor needs to produce a lot of power, more current will flow, especially if the motor is at a low RPM (and thus low back-EMF). 



This concludes the first part of my article. I’m working on the second part where I want to show some numbers and calculations and dig into the hub motor story. This needs some time, so please be a little patient.
```

---
## \#2 Posted by: devin Posted at: 2016-07-28T11:23:55.357Z Reads: 309

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: Stevemk14ebr Posted at: 2016-07-28T12:06:48.089Z Reads: 303

```
[quote="PB1, post:1, topic:6753"]
our RC-style remote receiver controls the throttle of the VESC also using PWM, but this has absolutely nothing to do with this, just the same technique
[/quote]
Our remotes actually use PPM, pulse position modulation. This is basically just sending various length bars pulses of on or off. Very different from pwm.
```

---
## \#4 Posted by: PB1 Posted at: 2016-07-28T12:46:23.779Z Reads: 292

```
Hello @Stevemk14ebr
I would like to be exact here and I see some wrong remarks in your post (sorry, I am a smartass): 

I never talked about remotes, only about the receiver. 
My understanding is that the communication between RC __receiver and ESC_ is via PWM (as written above)  

Yes, the communication between transmitter and receiver is via PPM, but I didn't mention that. 

And sending various length bars of pulses is PWM - pulse width (length) modulation

PPM is pulse positioning modulation. A pulses are sent at various timings but have the same length.

Again, sorry for being a smartass, just seems to be such a day ...
```

---
## \#5 Posted by: Stevemk14ebr Posted at: 2016-07-28T12:55:14.164Z Reads: 255

```
you are exactly ppm correct it relies on time not length, my mistake. I read your quote as if you were talking about receiver->controller
```

---
## \#6 Posted by: PB1 Posted at: 2016-07-28T12:56:25.761Z Reads: 242

```
@devin, if there is no load, there will be (almost) no amps. And you cannot "give" (force) more amps, you can only limit amps. 

But you can "give" more voltage. 

The amps are then drawn by the load (if not limited). 

I really tried to explain this using my words, hope it helps. If you don't believe, well you don't need to ... But I honestly think it would help you understanding some things.
```

---
## \#7 Posted by: Stevemk14ebr Posted at: 2016-07-28T13:29:32.304Z Reads: 214

```
Pwm has nothing to do with how the motor is turned. You have ppm from controller -> receiver then pwm (may be ppm aswell, idk) from receiver -> esc and then on a 3 phase dc motor like we use the esc simply energizes the correct coil at the right time. Different methods of determining which coil to energize exist, just 2 being sinusiodal, and foc, there are other methods aswell. 

Again the pwm signal IS NOT fed into the motor.
```

---
## \#8 Posted by: PB1 Posted at: 2016-07-28T14:00:13.577Z Reads: 204

```
Fully agree with you that the PWM signal from the receiver IS NOT fed into the motor. I even mentioned that in my post above. The PWM signal between receiver -> ESC has absolutely nothing to do with the PWM motor control ESC -> motor! So we do not need to discuss that. 
For ease of thinking we can even assume that input into the ESC is not via PWM but via a signal via the USB port or via UART or via Canbus. It doesn't matter. 


Nevertheless: the ESC in BLDC mode produces a PWM voltage that goes into our motor. This is how voltage and speed is controlled. 
FOC is different. In this mode the (V)ESC creates a sinusoidal DC wave. I haven't looked deeply into that yet.
```

---
## \#9 Posted by: Bender Posted at: 2016-07-29T00:46:40.238Z Reads: 196

```
[quote="PB1, post:8, topic:6753"]
FOC is different. In this mode the (V)ESC creates a sinusoidal DC wave. I haven't looked deeply into that yet
[/quote]

I hope you do look into it, I know more than a few of us are really interested in FOC and would like to know more about how it works.

I'm really enjoying your BLDC explanation, Thanks!
```

---
## \#10 Posted by: Stevemk14ebr Posted at: 2016-07-29T13:14:22.898Z Reads: 192

```
There are 3 main algorithms for bldc. In order of increasing efficiency: trapezoidal, sinusiodal, and vector algorithms such as foc.

It is important to note that rotor position is usually measured through "back emf" on the third un-powered phase coil inside the motor (trapezoidal and sinusoidal only power 2 coils at a time). This is a result of the fact that motors act as generators while spinning. 

Trapezoidal is a very basic technique that energizes two of the three coils based on the rotor position. 

Trapezoidal has high torque ripple, torque ripple can be thought of as a jerking push behind the motor, as if someone constantly went full throttle and zero throttle super fast. 

Sinusoidal control improves on trapezoidal by smoothly varying the current as it transitions to energizing a new pair of coils. It has reduced torque ripple but is innacurate for high speed. 

Foc solves all of the above by relying on vectors. As you may or may not know a motor is most effecient when the magnetic field is exactly 90 degrees to the electrical field. Foc mode creates a vector between the 3 phases of the winding in the motor and adjusts the power to line this vector up 90 degrees to the rotor. Foc uses all 3 coils, and always keeps the feld as close to 90 degrees as possible, this is why it is better.

Article: http://www.eetimes.com/document.asp?doc_id=1279321

To answer the thread hub generate more heat because they are at a mechanical disadvantage. This means to go the same speed or have the same torque they have to work harder. This requires them to draw more amperage from the batteries (voltage is a fixed value). Higher amperage systems generate more heat through inneficiencies in the motor and wires. Low amps = less heat = better.

If we doubled the voltage we gave to hubs the heat output would be the same/similar. But we'd also need higher voltage systems.
```

---
## \#11 Posted by: devin Posted at: 2016-07-29T13:23:53.672Z Reads: 169

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#12 Posted by: devin Posted at: 2016-07-29T13:33:58.791Z Reads: 170

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#13 Posted by: PB1 Posted at: 2016-07-29T13:34:18.138Z Reads: 170

```
hello @devin, 
Edit: this answers your "first" question above. 
this statement from @hummie is absolutely true and I've explained it in another thread. 

Reason is the following: it's a misconception that the full battery voltage is applied to the motor at all times. Yes, the full battery voltage is applied, but only in short "spikes", see above under PWM. So we have to think in average voltage. And the voltage on the motor side is actually the induced voltage that depends on the RPM of the motor.

And this voltage at the motor is lower than the battery voltage. So in order to have the same power (power always stays the same), the current in the motor can be higher than the current out of the battery.
```

---
## \#14 Posted by: devin Posted at: 2016-07-29T13:37:31.584Z Reads: 159

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: devin Posted at: 2016-07-29T13:38:35.601Z Reads: 159

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: PB1 Posted at: 2016-07-29T14:01:12.556Z Reads: 169

```
[quote="devin, post:12, topic:6753, full:true"]
@Hummie has made a second claim which, also, strikes me as flying in the face of established science. He says a motor running high amps (100) & low volts (1) will run exactly the same heat as an identical motor running low amps (1) & high volts (100). Both cases equal 100 watts. For ease of comparison let's say both motors are stalled so they can't freely rotate.

From what I understand about electricity, the motor running 100amps would produce exactly 100 times as much heat from resistivity in the wires as the motor running 1amp, even though they are both running at 100 watts.

Will someone knowledgeable explain if it is possible these 2 stalled motors produce the same exact heat, both running 100 watts, when one is at (1) amp, the other at (100) amps?
[/quote]

here I'm not agreeing with @hummie and I'm agreeing with you @devin

The motor with more amps will also produce more loss to heat.



[quote="devin, post:14, topic:6753, full:true"]
where do these extra amps "go" if they are not completing the circuit all the way back to the battery? it seems like they are appearing and disappearing into thin air if the voltage stays the same.
[/quote]

The amps do not disappear at all, they are converted. Think of two linked circuits.
On the left side batter and VESC input ---------- on the right side VESC output and motor
37V ------ 25V
10A ------ 14,8A
370W ------- 370W

Think like an AC transformer. On one side you can have 1000V and 1A on the other side you can have 100V and 10A.

Our ESC does the same: it commutates DC power into something like AC power.

[quote="devin, post:15, topic:6753, full:true"]
also, in the case of a motor which is stalled and unable to rotate, is it still possible for more amps to flow through the motor than come from the battery?
[/quote]

Especially in this case. If a motor is stalled and unable to rotate, current in the motor will go very very high. In theory the current is infinite when a motor does not turn. Reason: voltage at motor (Back-EMF) is 0. 
In real life the motor current is limited by the system. The whole system cannot produce more power than is there.




**One more thing: I would LOVE to discuss all of this over a fine craft beer with you guys. Maybe I fly to SF just to discuss with you two ... honestly!**
```

---
## \#19 Posted by: Hummie Posted at: 2016-07-29T15:37:56.406Z Reads: 162

```
haha.    come on over though and I'll buy you a beer and send you off on my board.

You will have the same heat in a motor to produce the same torque with either a 100 volts system or 1 volts system.(assuming the kv is adjusted)  the inductance producible and resistance of the windings are inversely related.  to get enough inductance to get up a hill with a motor that is 100kv takes ten times less amps than the same motor wound to have 1000kv, true, but the resistance of the windings is 10 times more so it balances.  and then if you also adjust your battery voltage to match and you have ten times more amps in the low voltage battery, of the same size, you go just as far.    Only thing you'd need to think about with the low voltage/high kv/many amp set-up is the rest of the wiring needs to a bit thicker and the vesc doesnt like it as much, but the motor wont notice
the only reason to go to higher voltage is if you want more speed or the vesc overheats or you want to reduce the size of the rest of your wiring.  a low voltage set-up is said to be the future by some as it's safer.  As soon as the escs have better components that can take the amps there's no reason to go to higher voltage...unless you get bored at your current speed.  and then it's more so just a personal thing and will leave you faster but generally a bit less efficient (me)

why a hub motor gets hot though is not that and is simply the lack of gearing...so really a gearing set up enables you to produce a lot less torque from the motor.   If my rare 54mm motor was to be wound to have a kv that was 1/3 of what everyone with a pulley set-up is and they use a 3:1 pulley set-up...so maybe 60kv...I wonder how efficient it would be going the same speed as the pulley set-up at lets say 15mph max speed on a flat.  I think it would fare better than the pulley set-up as long is the load wasnt too much.  So a flat 15mph comparison.  
I've heard that the best way to determine what size motor you need to get to ultimate efficiency is to balance the copper and iron losses.  all of us I imagine are way in the red on the copper losses regardless of hub motors or pulleys.  We're all not doing things for ultimate efficiency and if we were we'd be using bigger motors.  and then the copper will have less resistance, stay cooler.   but MAXIMUM efficiency is not what almost anyone is after on a skateboard.  A bit more loss to copper and we get to have a smaller motor and all is fine and we maybe lose a block or two travel distance and the motor doesnt get too warm to damage anything
```

---
## \#20 Posted by: HTownBomber Posted at: 2016-07-29T15:41:27.315Z Reads: 149

```
[quote="PB1, post:18, topic:6753"]
here I'm not agreeing with @hummie and I'm agreeing with you @devin

The motor with more amps will also produce more loss to heat.
[/quote]

Sure... at stall torque.  There is no applied voltage at stall torque, so of course amps are gonna drive the heat losses.  

A BLDC motor is a circuit, and Ohm's law still applies.  Waste heat (in Watts) can be calculated as some coefficient of the square of current times the electrical resistance ( W = I^2 * R ).  @devin & @PB1, the concept that both you guys are missing is that assuming the same power output, electrical resistance R increases exponentially when you shift the voltage ratio (because R = V / I). So with a high-spinning motor under load, applied voltage quickly becomes a much bigger factor than amps when it comes to waste heat.

At max rpms under full load, the 1 amp 100 volt motor will actually have 10,000 times the electrical resistance of the 100 amp, 1 volt motor, and it'll correspondingly get a lot hotter.
```

---
## \#21 Posted by: Hummie Posted at: 2016-07-29T15:55:40.017Z Reads: 136

```
i think making scenarios with 1 amp and 100 volts or vise versa isn't possible.  the resistance determines what current and voltage it is.  the resistance is the one stable number
```

---
## \#22 Posted by: devin Posted at: 2016-07-29T16:14:55.655Z Reads: 138

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: devin Posted at: 2016-07-29T16:19:09.614Z Reads: 125

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#24 Posted by: Hummie Posted at: 2016-07-29T16:23:33.232Z Reads: 120

```
the winding resistance will stay the same though as far as heat produced.  there's the back emf voltage but it doesnt add resistance to the motor just the amount of current you can put in I believe.
```

---
## \#25 Posted by: devin Posted at: 2016-07-29T16:26:04.929Z Reads: 116

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#26 Posted by: Hummie Posted at: 2016-07-29T16:36:11.891Z Reads: 119

```
i think we're talking about different "resistance".  the true electrical resistance of the windings will never change.   the increase in rpm and subsequent back emf creates a limit of what the max rpm can be but you dont have more heat running at higher rpms.  the only heat produced by the windings is proportional to the resistance of the winding and the amps through it.
```

---
## \#27 Posted by: devin Posted at: 2016-07-29T16:40:19.450Z Reads: 118

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#28 Posted by: Hummie Posted at: 2016-07-29T17:20:46.332Z Reads: 116

```
Keeping the motor the same...let's say 100kv....and adding more batteries in series...yet still keeping to let's say 20mph when now u have the cells to go up to 30...you will run a bit less efficiently as you're now further from the no-load speed 

The volts x amps equals watts just doesn't pan out in the motor.  I don't have an explanation and am hoping pb1 can get to the bottom of that
```

---
## \#29 Posted by: devin Posted at: 2016-07-29T17:25:15.684Z Reads: 108

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#30 Posted by: longhairedboy Posted at: 2016-07-29T17:46:16.851Z Reads: 106

```
as long as you put "in the motor" after it, i'll buy that shirt.
```

---
## \#31 Posted by: quanze Posted at: 2016-07-29T17:54:43.337Z Reads: 108

```
Can someone do a tdlr :joy:
```

---
## \#32 Posted by: PB1 Posted at: 2016-07-29T18:19:16.516Z Reads: 104

```
Gents, I think I have good news and then maybe not so good news for you. 

Good news is that I think I can explain it all.  Part two of my write up covers a lot of your questions. 80% is finished.  But please do not doubt the fundamentals of physics.  

Not so good news (maybe) : I will take a break from esk8 for a week,  go on vacation with the family and do lots of mountain biking (the real MTB).  
Maybe I'll post some pictures,  but I suppose I will not fight with you guys over physics.  

Send me a cask of your favourite craft beer and I might consider coming over to discuss.
```

---
## \#33 Posted by: PB1 Posted at: 2016-07-29T18:21:01.378Z Reads: 102

```
And before I forget : please decouple the voltage of the battery and on the motor side...
```

---
## \#34 Posted by: Hummie Posted at: 2016-07-29T18:35:06.189Z Reads: 102

```

http://www.ebikes.ca/tools/simulator.html

this should shed some light.

I'm really psyched to find this!!

this is why es is the shit

these guys know so much more.
https://endless-sphere.com/forums/viewtopic.php?f=30&t=81074
```

---
## \#35 Posted by: devin Posted at: 2016-07-30T23:36:36.560Z Reads: 100

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#36 Posted by: Hummie Posted at: 2016-07-31T00:10:22.427Z Reads: 92

```
youre right I miss spoke.  I didnt mean to say volts gets converted to amps I meant to say volts GET converted to amps.

the only part misleading as I see it is the rest of the statement.  and really I guess all the ingredients: battery, motor, esc, contribute to converting volts to amps.
```

---
## \#37 Posted by: devin Posted at: 2016-07-31T00:13:21.889Z Reads: 91

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#38 Posted by: Hummie Posted at: 2016-07-31T00:15:28.330Z Reads: 87

```
yes.  and I think the voltage and amp changes are related to all three parts.  battery, esc and motor are variables in what that conversion is
```

---
## \#39 Posted by: devin Posted at: 2016-07-31T00:16:02.787Z Reads: 92

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#40 Posted by: Hummie Posted at: 2016-07-31T00:22:15.945Z Reads: 94

```
The evidence I have from the blog, vedder's site, isn't contradicting it is saying the same.   volts get converted to amps by the vesc.  (and the motor and battery too).  the amps going through the phase wires are more than are going through the motor leads.  This was news to me.  I keep saying it because it changes how most people understand how many amps are moving their motors.  And they throw up an amp limit on motor spec sheets.  Yet the amperage we could be at is almost to the point of infinitely huge at stalling speed.  that's what I read lately.
```

---
## \#41 Posted by: devin Posted at: 2016-07-31T00:43:59.083Z Reads: 95

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#42 Posted by: Stevemk14ebr Posted at: 2016-07-31T01:36:06.970Z Reads: 93

```
Voltage is a constant (theoretically, ignoring voltage droop and such), its simply a measurement of the energy potential. You esc doesnt convert volts to amps. As the load increases on your motor it will want to increase the amount of power it draws. Since voltage is constant the only thing it can increase is current draw (aka amps); this is a result of the equation power = volts × current. Your motor will pull as many amps as it takes to power the load, regardless of your battery spec. If the current your motor draws is greater than your battery can supply the battery will heat up, explode, die, short, etc. The motor WILL DRAW WHAT IT NEEDS and gives zero shits about the battery spec, there is no conversions of anything, the only relevant equation is power = volts × current
```

---
## \#43 Posted by: Hummie Posted at: 2016-07-31T01:47:00.770Z Reads: 87

```
PB1:
No, not in standard bldc mode. This is what I have been saying all along. You have to think two separate circuits, the only link is Watts (not voltage and not amps, only Watts)

One side is battery and esc input. It's DC voltage of the battery and the amps are whatever is needed (if not constraint by anything).

The other side is esc output and motor. It's AC voltage. And the voltage is based on rpm and Kv of the MOTOR (plus something for loss).
IT IS INDEPENDENT OF THE BATTERY VOLTAGE!
Yes!!
So voltage at the motor is only dependent on rpm and Kv! And current is drawn from the esc. How much? As much as needed to have enough Watts to propel the rider.
NOT THE SAME AS BATTERY CURRENT, NORMALLY MORE.
And of course the rider has to open the throttle enough to convert (commutate) enough V and A from the battery side to the motor side.

Wattage is the link! Both sides have the same Watts (neglecting losses). They have different A and V.
```

---
## \#44 Posted by: devin Posted at: 2016-07-31T01:59:37.474Z Reads: 85

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#45 Posted by: devin Posted at: 2016-07-31T02:19:34.401Z Reads: 80

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#46 Posted by: Hummie Posted at: 2016-07-31T03:33:56.046Z Reads: 77

```
Vesc doesn't work that way according to folks at vedder's site.
```

---
## \#47 Posted by: devin Posted at: 2016-07-31T04:25:12.610Z Reads: 77

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#48 Posted by: Hummie Posted at: 2016-07-31T05:58:32.816Z Reads: 80

```
No.  Why such confusion.  I'm saying voltage gets converted to amperage by the vesc.  That's what we're talking about. That's what I keep saying. That's all I'm saying. 
There is a duty cycle program and a current control program.  There are a couple different things going on and FOC being probably the most complicated.  Ask Vedder if u have a question.  But as far as voltage being converted to amps that's as much as I can say
I don't think it works in the typical way.  As has been said the current can be infinately large and there is a transformer-like action occurring.  This is what Ren and Vedder have written and I've linked and quoted.
```

---
## \#49 Posted by: devin Posted at: 2016-07-31T11:17:41.963Z Reads: 82

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#50 Posted by: devin Posted at: 2016-07-31T11:37:38.193Z Reads: 81

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#51 Posted by: devin Posted at: 2016-07-31T12:59:11.689Z Reads: 78

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#52 Posted by: PB1 Posted at: 2016-07-31T19:49:23.137Z Reads: 78

```
@devin,  our esc are not converters in the true sense (yes,  they convert,  but...  ).  Don't look up converter or step up / down.  It's wrong.  

The technique used in bldc controllers is the same as for brushed motors.  A commutator is used.  In our case an electronic commutator.  They create something that looks like AC using pwm.  Your pictures above are correct.  

And there are no large capacitors to store and forward energy.

Calculation for NO LOAD RPM is the same.  Kv * maximum voltage = Kv * battery voltage.  

Remember,  it's a theoretical value that cannot be reached by powering the motor off battery and ESC.
```

---
## \#53 Posted by: KMeyerson Posted at: 2016-08-04T04:10:56.875Z Reads: 68

```
I turn my head for two days.  Man this thing lit up and I am loving the science.

PB1 hit the nail, KV is KV.  A lovely, horribly misunderstood constant.

You can have a similar argument with a Tesla specialist. Their claims used to be that the vehicles were based on variable AC motors which, for the most part, is true.  However the hardware resembled BLDC tech on longboards more than you might realize.  An active Tesla hacker found that the BLDC drivers only resembled AC signaling but did not product true AC signals as expected from Tesla's claims. The modulated signals we use for BLDC are neither true AC nor true DC.  We may need to find the name or come up with one for the particular sinusoidal effect we generate.
```

---
## \#54 Posted by: VladPomogaev Posted at: 2016-08-04T10:28:25.424Z Reads: 73

```
There is a lot of misinformation is this thread. Anybody wanting to learn anything useful should take the information here with a lot of salt :)
```

---
## \#55 Posted by: Bender Posted at: 2016-08-04T12:09:41.774Z Reads: 76

```
@VladPomogaev How about correcting it or posting some links please :grinning:
```

---
## \#56 Posted by: devin Posted at: 2016-08-04T12:23:46.988Z Reads: 84

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#57 Posted by: VladPomogaev Posted at: 2016-08-04T15:54:17.850Z Reads: 81

```
Haha, it will be like the blind following the blind!
```

---
## \#58 Posted by: PB1 Posted at: 2016-08-04T20:24:11.130Z Reads: 84

```
@VladPomogaev " There is a lot of misinformation is this thread. Anybody wanting to learn anything useful should take the information here with a lot of salt ￼" 

Like everything you read somewhere in an Internet forum.  
Would you like to point out which information might be flawed?
```

---
## \#59 Posted by: PB1 Posted at: 2016-08-04T20:38:58.090Z Reads: 82

```
Glad if my article made you look into the right direction.  

Your mentioning of Tesla also triggered something and I did some searching and found this nice post by a tesla engineer:
https://www.tesla.com/de_CH/blog/induction-versus-dc-brushless-motors?redirect=no 

In short,  tesla uses induction motors which are very similar to our bldc motors.  Main difference is that these motors use coils and variable current instead of permanent magnets and control is somewhat different.  They are the synchronous motors I mentioned in my original post but driven by converted AC.  

BTW tesla uses liquid cooling for their power train and still has to deal with excessive heat. You can't push a tesla for very long at full power. It backs off in order to protect the electronics and motors.  

So indeed the whole Tesla set up looks very similar to what we are using.  Gee,  we are leading edge!!!
```

---
## \#60 Posted by: SimosMCmuffin Posted at: 2016-08-04T21:55:16.925Z Reads: 81

```
That's a great article. I remember reading it awhile back.

The reason they use an induction motor is because it's cheaper to manufacture, just iron and copper basically. Magnets for the same power PMSM motor would be more expensive and the motor would be heavier, but the PMSM has better peak efficiency. Tesla probably put quite a nice amount of RD into developing that liquid cooled induction motor.
```

---
## \#61 Posted by: VladPomogaev Posted at: 2016-08-05T00:26:39.813Z Reads: 80

```
Or you guys could just start citing credible sources?
```

---
## \#62 Posted by: Hummie Posted at: 2016-08-05T00:40:42.934Z Reads: 84

```
how bout you add some to our knowledge with a credible source?  I think wer're all looking.  the quick no citation answer for why a hub motor gets hot is it somehow has to do more work for the same output as a geared system so needs to be bigger.  a bigger motor will be more efficient simply until it's so big the iron losses take over the copper losses.  we're all in copper losses with our small motors.


I saw a video on the production of the Tesla and one thing we dont do that he does and seems really worth it especially with the rough conditions our motors are subject to is pot the windings.  I've read about potting windings being a boon for dissipating heat but in my experience doing it it was a detriment.  I had good fancy resin as well.  Wish I knew what he used.  Maybe it's a compromise for the car and ends in more secure windings but a bit hotter and the cooling system can handle it.
```

---
## \#63 Posted by: bbq870 Posted at: 2016-08-05T04:47:15.597Z Reads: 82

```
potting alone will not help, I think. the heat needs to go somewhere. (in our case)
to my understanding not all windings get the same temperature. (hotspots??) correct me if I´m wrong.
so potting would distribute the heat better but as its an enclosed system the heat will stay inside the motor.
so next step is to get out the heat
```

---
## \#64 Posted by: SimosMCmuffin Posted at: 2016-08-07T09:09:45.209Z Reads: 91

```
I would speculate that the reason why hub motor runs hotter, is that it can't dissipate the heat. So if you're running the same power to a identical mass and construction materials belt drive motor and hub motor, both should warm up the same rate, but I think because belt drive motors are usually in the airflow all around the can (lots of surface area) it dissipates the heat more efficiently and therefore runs cooler overall. Hub motors have the insulating polyurethane around the can, so it can't as efficiently cool itself with airflow.
```

---
## \#65 Posted by: Mathias Posted at: 2016-08-08T17:33:02.313Z Reads: 95

```
I like this discussion a lot but there is a lot of misinformation circling around. I am not an expert on VESC or BLDC motors but in physics and maybe I can clear some of the fundamental misconceptions: 

Of course people are right: hub motors are not cooled as efficiently inside the wheel. Even worse: there is rolling friction. Your board doesn't roll forever because the kinetic energy is lost and heats your bearings, the road and your wheels. So the motor is right where you get most of the friction. But what most people completely mix up in this thread is the following

What actually heats the motor the motor in the first place? 

Short answer: Losses! Not the Current, not the total Power.

The Power dissipating into heat is NOT the total power. Let's consider a simple scenario for now: we accelerate, no rolling friction or air friction. Energy E is conserved, so E (P is the change of E over time), is split up into two main channels: kinetic energy K, and the loss L:
E = K + L
All the energy that actually contributes to accelerating you does NOT produce heat at this point. It will eventually since you don't roll forever. But for now it does **not**. Only L. The efficiency is the portion of E that you can get into K instead of L. This is where @HTownBomber is wrong: a motor is not simply a resistor. The power _consumed_ by the motor is P = U*I but that it _not_ the power that dissipates into heat like in a resistor. 

The statement that only P matters, not how you distribute your numbers in U and I, is wrong because the **efficiency** changes! 

One part is electrical loss simply trough the electronics resistance R. The loss due to R is NOT the product of the total battery Voltage Ub, since only a portion of Ub drops over R: Ur. 
Only the rest of the power is USED by the motor. But the **total** battery current I passes through R:
P = Ur * I = R * I²; 
This is the reason why we use high voltage transmission lines. You cannot avoid resistance altogether. So keep the voltage high and you increase the portion of Power that you can USE. But, as @Hummie pointed out, this does not apply to the motor windings: lowering KV reduces I but increases the resistance and the copper losses are the same. It does however apply to the rest of the electrical components and especially the ESC is more efficient at high voltage. 

Apart from the electrical loss there are the typical BLDC motor characteristics. As I said: I am not an expert for BLDC motors but there are some rules of thumb that you can easily apply. The properties of a typical BLDC motor should look somewhat like this:

http://www.mellorelectrics.co.uk/BLDC-performance-graph.jpg

[http://www.mellorelectrics.co.uk/BLDC-MOTOR-EN.html](http://www.mellorelectrics.co.uk/BLDC-MOTOR-EN.html)

N: RPM
EFF: efficiency
P: power
I: current

This an idealized graph for ONE specific motor, and this is imporant: for one KV value (RPM/Voltage). One important fact that people should pay more attention to is that the maximum power is not where you find the maximum efficency! 

To increase efficiency you should run your motor at a high RPM and low torque. This is why you should use a small motor pulley and a large wheel pulley in a timing belt setup. This can bring you to the left side of the graph, where the efficiency is high. 

Also you can lower KV, which should more or less scale the x- and the y-axis. It will give you higher torque at lower current. Therefore you can keep the **torque load further from the maximum that the motor can do**. Reduce the speed, increase the maximum torque, then you can shift the maximum efficiency to lower RPM. 

To estimate what "high RPM" means we can calculate some numbers: 
The largest gear reduction that you can usually get is around 12:36 . Let's assume we want a maximum speed of 35 km/h (21.7 mph). At 83 mm wheels this means the motor will run at ~6630 RPM. The KV that you need for this at 12s is  ~**150 RPM/V** (!!!). This way you can run your motor close to the maximum efficiency.  

What makes hub motors become so hot? The lowest KV of a hub motor that I have seen so far is around 75 RPM/V, which leads us to a **theoretical** top speed of 52.7 km/h (32.8 mph)! So why do you not reach it? If you can't get close to this RPM it means that your load is too high! You run at a regime at too high torque load, too high power (center of the graph), and **low efficiency**. Your motor will get **hot** because it wastes a too much of the precious power from your battery pack!

As you accelerate you climb up the blue curve (RPM) and the efficiency climbs up with it. Your motor has a comfort zone. But you can only get there if you don't use all the torque, that it can offer. Here is a cheesy flowchart to illustrate my point graphically:

<img src="/uploads/db1493/original/2X/e/e08ae5761863413604b30506869d2a07fa34c756.png" width="461" height="291">
```

---
## \#66 Posted by: furryfrog Posted at: 2016-08-09T07:19:01.087Z Reads: 74

```
I like the graph you posted, helpful in understanding the characteristics of brushless motors, and the disadvantage hub motors have not being able to change the gear ratio. Makes sense to me, can't just make a bigger hub motor, because the wheel circumference also increases.
```

---
## \#67 Posted by: PB1 Posted at: 2016-08-09T13:15:10.566Z Reads: 72

```
@Mathias very good post thanks!

As mentioned above I'm working on part 2 of my article that is going to cover the stuff you mentioned, so thanks for contributing. 

I'm also doing a chart that calculates some data based in input. Thinking about it I could use this sheet in order to plot a graph for various motors and extend it and include SPEED. This would then be the theoretical graph that we would have to verify. 

BTW:while the graph in your post is absolutely correct, it is somewhat difficult to read and interpret! 
e.g. the unskilled eye could think that amps is the highest at high RPM while the contrary is true!
```

---
## \#68 Posted by: SimosMCmuffin Posted at: 2016-08-09T13:19:36.057Z Reads: 70

```
http://members.toast.net/joerger/pic2/motorcurve.gif

Would this be easier to interpret?
```

---
## \#69 Posted by: Mathias Posted at: 2016-08-09T13:27:38.899Z Reads: 68

```
[quote="PB1, post:67, topic:6753"]
BTW:while the graph in your post is absolutely correct, it is somewhat difficult to read and interpret! e.g. the unskilled eye could think that amps is the highest at high RPM while the contrary is true!
[/quote]

Yes, didn't actually make it. The link is posted below the graph.
I would also prefer @SimosMCmuffin 's post. It is less confusing.  I was already thinking about making calculations like this on my own, or rather a simulation with proper parameters for an e-skateboard. Unfortunately I'm super busy writing a thesis at the moment. I shouldn't actually be on this board right now... It's just that e-skateboards seem 100 times more interesting at the moment:
```

---
## \#70 Posted by: PB1 Posted at: 2016-08-09T13:32:40.552Z Reads: 75

```
that's the universally agreed graph :-) 

Not sure how many people really know what it means though, hahaha ... 

will try to draw the curves for specific boards or setups and showing speed in km/h as horizontal (x axis), then every eSkater can check at which exact point in power he is. This needs some assumptions of course. 

Thanks guys for your constructive input!

@mathias, fully with you. At day time I should do some work, in the evenings I rather go for a ride on my eSk8 board than this discussion board and then there is family ... :-)
```

---
## \#71 Posted by: SimosMCmuffin Posted at: 2016-08-09T13:33:27.364Z Reads: 74

```
I'm planning on graduating this autumn and I plan to write the thesis about the ESC I designed and I should probably really start writing soon, but man. There really seems to suddenly be a lot of other interesting things I'd rather do :grin:

Also I'm designing the next iteration of the controller at the moment.
<img src="/uploads/db1493/original/2X/5/5350db4efcbdae7c2474c4281987ad84353d3b62.png" width="690" height="364">
```

---
## \#72 Posted by: Catchmeifucan Posted at: 2016-09-09T20:20:34.472Z Reads: 69

```
I like this description, very enlightening and makes you think about the basics that should be obvious. I am not sure about the equation or what the abbreviation Ke stands for?

One thing I just thought of though is if a Vesc controls Voltage output and current then the best place to start is by getting the Vesc that can take the highest voltage input and matching that with a battery that nearly reaches the maximum capacity of the Vesc so regardless of motor choice it can run a bit cooler when modulated to the highest voltage rather than the highest amperage. What do you think?
```

---
## \#73 Posted by: Hummie Posted at: 2016-09-09T20:27:18.923Z Reads: 72

```
voltage gets converted to amps or something to that effect and you'll get the same heat to torque output regardless of the voltage of the battery.  motors run on amps.  higher voltage will be easier on the battery and generally easier on the esc too
```

---
## \#74 Posted by: PB1 Posted at: 2016-09-09T20:32:06.439Z Reads: 73

```
Most important point is a balanced system.  

Motor rating,  Kv,  battery voltage,  gearing, desired speed /torque.  Then apply the proper settings.
```

---
## \#75 Posted by: KMeyerson Posted at: 2016-09-11T00:22:18.111Z Reads: 76

```
I think this discussion has two facets:
1. Physical Motor Design
2. ESC Design

We know we are asking a lot of a fist sized motor. 30Nm and 60kmh are a lot to expect from a stator that shouldn't be much more than 30mm or so long with a diameter of 55mm or less. 

We also know, @devin, that there is some funky stuff happening with the VESC.  In brief, he has tried to understand the discrepancy between expected motor output based on battery/motor output settings in the VESC by examining the power entering and exiting the systems.  If the current draw and voltage entering the VESC from the battery is XXXwatts and that same power leaves (minus some thermal waste) goes into the motor, we should expect XXXwatts worth of performance.  This is significant because the VESC calculates the rms voltage from the available/set current. If this voltage is not significant enough to generate a field, more amps come to compensate (HEAT!). If the amperage is low, then the system doesn't seem to compensate satisfactorily. (If I missed something @devin, let me know).

Since there are a lot of VESCs in the wild now, can we try to understand the VESC settings better before we drop cash on motor building?
```

---
## \#76 Posted by: kieraneboard Posted at: 2017-07-16T00:08:50.994Z Reads: 43

```
This is fantastic.  It helps me a lot.
```

---
## \#77 Posted by: fastesk83r Posted at: 2018-12-09T23:26:37.524Z Reads: 17

```
Hi all XXX! :):stuck_out_tongue_closed_eyes: 

A hub motor gets much hotter because the small motor is required to output high torque, because of this, the motor amps are higher. More current = more heat and the motor is also trapped inside a urethane casing which increases thermal insulation. Enertion uses a great cooling technique for the stator which transfers the heat directly to a heat-sink truck!

Hub motors will get much better soon ;)
```

---

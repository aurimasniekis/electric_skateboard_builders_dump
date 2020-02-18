# What am I missing out on ? BLDC or FOC

### Replies: 24 Views: 1009

## \#1 Posted by: Toughook Posted at: 2018-08-31T23:28:57.934Z Reads: 276

```
Recently changed settings from 40A motor max to 80A and the difference was immense..... but I have a feeling I'm still missing out on something (dual 6374 on a 10s5p)

I have a suspicion I've still improvements to make though (I think). I'm currently running BLDC mode, unsensored.

Should I switch to Sensored FOC, and if so, what am I missing out on - apart from standing starts (currently need a very slight kick push to get going smoothly because of BLDC)

Don't get me wrong, the new settings are incredible, but can they be better?

Cheers
Tony
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2018-08-31T23:32:50.330Z Reads: 267

```
[quote="Toughook, post:1, topic:66705"]
what am I missing out on
[/quote]

A level of refinement because of smoothness and silence. Basically rides the same 😂
```

---
## \#3 Posted by: Deckoz Posted at: 2018-08-31T23:56:47.262Z Reads: 254

```
Sensored FOC, with traction control over canbus, with 100+ motor amps. 😲😲 🚀
```

---
## \#4 Posted by: karma Posted at: 2018-09-01T09:35:35.091Z Reads: 232

```
What VESC are you running? (Focbox and 100A motor current?)
```

---
## \#5 Posted by: Deckoz Posted at: 2018-09-01T13:45:16.832Z Reads: 225

```
@karma  I run FOCBOX on 13s with 120A motor current. You see, the FETS are rated at 75v and upto 250A with proper cooling, if I'm not mistaken (need to check the data sheet again). The Focbox copper pours are rated for 50A @ 60V. 

ESC are basically a buck converter. Varying the duty cycle. You can find lots of my posts on duty cycle. But the answer is simple. 

Motor Max 120
Battery Max 50
Voltage 54.6

54.6V * 50A = 2730Watts
2730Watts / 120A = 22.75v
22.75V / 54.6V = 41% duty cycle.

So above 41% duty cycle the motor amperage will drop the meet the maximum battery amperage/wattage. 

2730W / (54.6V * 42% Duty) = 119A 
2730W / (54.6V * 43% Duty) = 116A 

And below 41% the motor amperage can be upto 120A. Meaning more power to the ground during acceleration giving you your maximum output potential throughout the entire band. For example. Duty cycle comparison of actual output

Motor Max 60A
(54.6V * 10% Duty) * 60A = 327Watts
(54.6V * 20% Duty) * 60A = 655Watts
(54.6V * 30% Duty) * 60A = 982Watts

Motor Max 120A
(54.6V * 10% Duty) * 120A = 655Watts
(54.6V * 20% Duty) * 120A = 1310Watts
(54.6V * 30% Duty) * 120A = 1965Watts

As you can see, all examples are lower than the Battery Max 50A @ 54.6v (2730 watts) and also within the limits of the pours, 50A @ 60v (3000Watts), and the amperage is well under 75% of the rating on the FETs.

So with the right cooling for the ESC, a big battery and the capability of the ESC, why leave all that power on the table if you are within the limitations of the hardware....

Just saying

Edit: my point to this in the original topic of the thread, was sensored FOC helps the controllers accurately calculate motor angle, so no power is wasted from bad timing. The mixture of a clean phase timing,  with lots of power, and traction control enabled so that the controllers can measure slip and not torque out makes the whole combo turn into 🚀sauce.
```

---
## \#6 Posted by: Sender Posted at: 2018-09-01T13:52:30.863Z Reads: 212

```
You know, I have read most of your posts on this.  I think I garner a little more understanding everytime I read them. Gracias.
```

---
## \#7 Posted by: Sender Posted at: 2018-09-01T13:55:01.291Z Reads: 202

```
Of all your/others' explanations, something about this wording in particular makes it clear and easy to undrstand.  Even for us plebs.  Your professorly posts are becoming even more digestible.  Maybe I am also just starting to get it more, but still.
```

---
## \#8 Posted by: wafflejock Posted at: 2018-09-01T13:57:13.084Z Reads: 200

```
Glad you're already more of a proponent of safety gear than anyone I know or you'd have me worried.
```

---
## \#9 Posted by: Deckoz Posted at: 2018-09-01T13:59:41.418Z Reads: 203

```
[quote="Sender, post:7, topic:66705, full:true"]
Of all your/others’ explanations, something about this wording in particular makes it clear and easy to undrstand. Even for us plebs. Your professorly posts are becoming even more digestible. Maybe I am also just starting to get it more, but still.
[/quote]

Haha, thanks, re-read the ending edit I added regarding the OP's question..(traction control) it will make even more sense

[quote="wafflejock, post:8, topic:66705, full:true"]
Glad you’re already more of a proponent of safety gear than anyone I know or you’d have me worried.
[/quote]

Haha yeah, safety first :) it's literally #1 above all else.

Also side note. I think it's hilarious that some production boards are rated for 4000-8000Watts, when really they are just stating the motor specs. Their batteries can hardly even put out above 2000watts. And when they do it's at higher duty cycles, so acceleration is...well boring.

Ie 10s3p 60A constant current max at full charge is 2520Watts total, or 1260W per motor. Really not that much power...double the cell count, like mine 13s5p you've got 5460W, or previous mentioned 2730/ESC. There's good reason people like @chaka @longhairedboy etc use higher P count packs. However I don't believe they utilize the higher P count to their advantage with configuration.
```

---
## \#10 Posted by: longhairedboy Posted at: 2018-09-01T14:40:00.823Z Reads: 189

```
range and regen braking performance are the two main reasons why i prefer packs over 4P.
```

---
## \#11 Posted by: Dmaxx Posted at: 2018-09-01T14:41:32.616Z Reads: 191

```
I recently switched to sensorless FOC on my dual 6374 12s4p dual focbox build and I'm in love!! Dont get me wrong, it was super fun beforehand, but the smoothness and silence are just so nice. One of my motors sensor wires stopped working so I decided to try out foc. In sensorless you do have to give a little push still but it is worth it. Also the brakes are 10x better in the smoothness category! Running motor amps 80/-65 and battery amps 40/-15
```

---
## \#12 Posted by: Toughook Posted at: 2018-09-01T16:32:43.553Z Reads: 187

```
Thanks for all the advice everyone, much appreciated. I can't quite believe that I can make my board even better (but of course I do believe you guys!) but my first trip out on 80A motor max yesterday was incredible. What a machine I've managed to put together ❤

Can't wait to tweak it further 👍
```

---
## \#13 Posted by: professor_shartsis Posted at: 2018-09-01T17:42:31.281Z Reads: 186

```
FOC produces more torque than BLDC for the same amount of battery amps, or consumes less battery amps for the same torque (more efficient). FOC uses a sine wave via all 3 phases simultaneously while BLDC uses constant current through 2 phases at a given time.

FOC Torque:
* RMS Current Limit = Motor Current Limit (peak current per phase) / sqrt(2)
* Newton Meters Torque = 1.5 * (60 / (2 * pi * KV)) * RMS Current Limit
* https://www.motioncontroltips.com/what-is-sinusoidal-commutation-for-dc-motors/

BLDC Torque:
* Newton Meters Torque = (60 / (2 * pi * KV)) * Motor Current Limit



https://upload.wikimedia.org/wikipedia/commons/thumb/8/89/Sine_wave_voltages.svg/530px-Sine_wave_voltages.svg.png

https://image.ibb.co/dBMfBT/3_D4_EC104_25_CA_421_A_8820_56_D249_F4245_F.png

https://image.ibb.co/csUiWT/A82_AAEFC_6_BC4_4708_B6_C6_BFE128_DDB7_F1.png

https://image.ibb.co/cNtxJU/foc_vs_bldc_graph.jpg
http://www.imavs.org/papers/2016/167_IMAV2016_Proceedings.pdf
```

---
## \#14 Posted by: Lionpuncher Posted at: 2018-09-01T19:32:21.906Z Reads: 157

```
That explanation is perfect. I bookmarked that for future use. Thanks @Deckoz. You make nerdiness 😎.
```

---
## \#15 Posted by: professor_shartsis Posted at: 2018-09-01T19:41:09.370Z Reads: 160

```
[quote="Deckoz, post:5, topic:66705"]
The Focbox copper pours are rated for 50A @ 60V.
[/quote]

[quote="Deckoz, post:5, topic:66705"]
As you can see, all examples are lower than the Battery Max 50A @ 54.6v (2730 watts) and also within the limits of the pours, 50A @ 60v (3000Watts), and the amperage is well under 75% of the rating on the FETs.

So with the right cooling for the ESC, a big battery and the capability of the ESC, why leave all that power on the table if you are within the limitations of the hardware...

Just saying
[/quote]

@Deckoz i believe the heating on the fets/copper pour of ESC is proportional to the motor current^2 * esc resistance not battery current^2 * esc resistance... so running constant 120a motor amps, while staying below 50a battery amps won't prevent the ESC from overheating in theory if the copper pour is rated to 50a constant...

[quote="Deckoz, post:5, topic:66705"]
Motor Max 120
Battery Max 50
Voltage 54.6

54.6V * 50A = 2730Watts
2730Watts / 120A = 22.75v
22.75V / 54.6V = 41% duty cycle.
[/quote]

@Deckoz i believe these are correct BLDC values, but not exactly the same w/ FOC, since the 120a motor current limit corresponds to the peak current per phase, not the rms current.
```

---
## \#17 Posted by: Hummie Posted at: 2018-09-01T20:03:22.363Z Reads: 141

```
i understood amps to be the only heat source.
```

---
## \#18 Posted by: professor_shartsis Posted at: 2018-09-01T20:06:41.088Z Reads: 144

```
[quote="Deckoz, post:16, topic:66705"]
Amps aren’t heat. Watts are. 50A @ 60v is 3000watts of heat. Each of those iterations above are less then 3000watts, you shouldn’t be burning the pours. Yes higher current will react and generate more heat with the resistance of the circuit. But you aren’t going to exceed the rating of the pours.
[/quote]


if you want to calculate the heat produced by the motor, it's motor current^2 * winding resistance = copper loss watts

same is true for the vesc fets but substitute esc resistance for winding resistance

& copper loss watts + mechanical watts = electrical watts

[quote="Deckoz, post:16, topic:66705"]
Pretty sure the telemetry output and calculated output is RMS, but I’ll accept otherwise if you can show me in the code of the control loop.
[/quote]

my understanding is the limitation on the vesc as far as motor current is the current sensing abilities, which become inaccurate above ~120a motor current... so if the RMS current was 120a, then the peak current would be 120a * sqrt(2), which would surpass the vesc's current sensing abilities, in theory.
```

---
## \#19 Posted by: Hummie Posted at: 2018-09-01T20:09:25.523Z Reads: 134

```
the flipsky 6.6 is said to be able to do 150 motor amps.  i think the real 6 and also the focobox are also able to do higher than the old vesc4.
```

---
## \#20 Posted by: Okami Posted at: 2018-09-02T08:38:18.005Z Reads: 123

```
While we are still on topic - is it 'safe' to put motor current for 5065 size motor over 60A or will it cook itself?

They are usually rated to 50A..
```

---
## \#22 Posted by: Jake2k17 Posted at: 2018-09-21T03:58:41.000Z Reads: 89

```
sorry to bring this thread back but @Deckoz I'm using Torqueboards 4.12 vescs, would this be a good idea to run FOC on these or no?
```

---
## \#23 Posted by: robthebuilder Posted at: 2019-01-21T06:45:20.187Z Reads: 59

```
I turned FOC on, on my first 12S setup and it burned the DRV-chip. I got a new one running 12S on bldc and haven’t had a problem since
```

---
## \#24 Posted by: Friskies Posted at: 2019-01-21T06:48:05.930Z Reads: 60

```
I saw your icon and thought that @ChrisChaput was back!!!

Also FOC  mode is fine on quality hardware Ollin/Unity/Focbox
```

---
## \#25 Posted by: Bjork3n Posted at: 2019-01-21T09:11:53.083Z Reads: 50

```
I went foc after running bldc for a year. 
Foc makes everything feels so refined, it's smooth, powerful and braking is alot better. 
I lost around 5km/h going Foc but I still feels it's worth it. 
Using focboxes v1.7
```

---
## \#26 Posted by: robthebuilder Posted at: 2019-01-21T11:42:23.672Z Reads: 44

```
I'm sure it is! I'm using a standard VESC v. 4.12
```

---

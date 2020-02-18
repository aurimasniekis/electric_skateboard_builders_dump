# Changing FOC Switching frequency

### Replies: 231 Views: 7512

## \#1 Posted by: RiGo Posted at: 2017-08-17T22:38:18.798Z Reads: 529

```
I asked this question in a separate thread but it got lost in all the other talk.

What are the risks of setting the wrong switching frequency in FOC? I changed mine from the default 40000Hz to 20000Hz to make the motors quieter but @Ackmaniac  suggested I set it to 30000Hz for my motors (Enertion 6355 190kv R-Spec). The change also made startup smoother with hardly any cogging (sensorless).

<img src="/uploads/db1493/original/3X/c/2/c2fc845562b29276a4e3b944bcaa7f62d3347e25.png" width="598" height="165">


What does F_SW do?
Why would he have made that suggestion?
What's the risk of getting that number wrong?
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-08-18T01:14:32.059Z Reads: 487

```
Bump...Im interested in this as well.
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-08-18T02:11:02.688Z Reads: 475

```
I'm definitely interested.
```

---
## \#4 Posted by: evoheyax Posted at: 2017-08-18T02:36:30.174Z Reads: 471

```
interested as well. @Hummie might know. Was talking to devin about these settings a few days ago
```

---
## \#5 Posted by: Hummie Posted at: 2017-08-18T04:11:38.909Z Reads: 464

```
I've never heard of it.  you should ask on the vedder forum and tell us!  sounds pretty fantastic.
```

---
## \#6 Posted by: RiGo Posted at: 2017-08-18T05:35:18.535Z Reads: 454

```
Well @Ackmaniac is the one who originally made a comment about this setting, so I'm hoping he will chime in.
```

---
## \#7 Posted by: smurf Posted at: 2017-08-18T06:08:14.074Z Reads: 445

```
Maybe @chaka knows the answer
```

---
## \#8 Posted by: chaka Posted at: 2017-08-18T14:22:37.128Z Reads: 434

```
The way I  understand it is you want to have your switching speeds as low as possible, too low and you will begin to lose control of the torque ripple and the gains from having a low switching speed will be lost. 

Much of what we see in the new VESC-tool and the BLDC-tool was borrowed from TI InstaSpin. Should find more info if you include that in your search queries.
```

---
## \#9 Posted by: Deckoz Posted at: 2017-08-18T21:13:38.272Z Reads: 428

```
I run mine in FOC at 20khz.

Basically its the same across all brushless type drive trains. Changing the motor update rate changes the degrees per update and also efficiency and top RPMs. For example if I'm remembering right 32khz is once every 6 degrees of rotation and 48khz is every 2 degrees of rotation. There is a physical limit of how fast you can update a motor as there reaches a point where the updates per degree of rotation have little to no effect on the angle of the motor. The faster the update rate the more efficient and smoother the motor transitions will be. The slower the update the more current can be pushed with each burst which in turn lowers efficiency and increases top RPMs

Side note. Most RC escs have an input range from receiver/controller -> ESC of 400hz - 32khz+. While the ESC -> motor runs at 16khz as that is the limitations of the FETs(Slew Rate) in use.
```

---
## \#10 Posted by: evoheyax Posted at: 2017-08-19T05:51:28.104Z Reads: 413

```
haha, the mystery of vesc settings. Few understand them, yet 1000's use the vesc :P
```

---
## \#11 Posted by: Hummie Posted at: 2017-08-19T22:25:21.400Z Reads: 399

```
@Deckoz  is there a difference between what you're talking about and erpm?  can you define the terminology in numbnut terms please and walk us through what you know at snail pace with stops to reinforce and possibly visuals or references!  the goal of getting the best efficiency and smoothness without sensors is alluring.  And how much  more efficient are sensors and are they only relevant till like 3mph and then the hybrid mode will switch to foc?  especially on a slower erpm hub motor what are the options here?
```

---
## \#12 Posted by: Deckoz Posted at: 2017-08-20T01:02:38.609Z Reads: 391

```
One is cycles per second one is cycles per minute.
```

---
## \#13 Posted by: Hummie Posted at: 2017-08-20T04:21:21.569Z Reads: 379

```
haha.  you did answer the first question thank you.   I'll try the vedder forum and maybe find a guy who cant stop talking.
```

---
## \#14 Posted by: Nowind Posted at: 2017-08-20T05:01:24.784Z Reads: 382

```

Can tell this from own expierence:
with 20khz i got some jigglers by high rpm ... it sound wired and feels like the motors start to go up and down with rpm
@ackmaniac set the SF to 30khz and the jigglers where history... 
be carefull you have to do new detection with a "correctur factor of 0.75" or anything... 

[quote="evoheyax, post:10, topic:30928"]
haha, the mystery of vesc settings. Few understand them, yet 1000's use the vesc :stuck_out_tongue:
[/quote]

haha i´m one of the 1000´s

Cheers
```

---
## \#15 Posted by: Deckoz Posted at: 2017-08-20T15:49:02.021Z Reads: 353

```
Sorry I didn't answer all of your questions

BLDC / Hybrid never switches to FOC with sensors. The point of Hybrid with sensors is to allow the BLDC timing (6 sequence timing) to be timed at a rate that will make the motor move forward without de-synchronization. Once the motor is moving fast enough it creates enough back EMF for the driver to take over and keep sync without assistance - whether sensored or emulated sensorless. No matter what way you look at it, it is BLDC Timing, with assistance of sensors for that timing. It will never be as smooth as FOC. BLDC timing applies current in bursts so a singular phase at a time to move the motor forward.

FOC is sinusoidal/trapezoidal wave forms. FOC can be done without sensors but it is very crude. With sensors, as the bell housing turns past each sensor, the readout if graphed makes a 3 phase sinusoidal wave form - this is used to calculate position, as well as creating the driving current from the fets as the sensor data can be transformed into a value to control the gates on the FET - making it more natural sinusoidal vs trapezoidal. FOC also applies current to all three phases all the time when under load. There is no timing. It is the values of sensor data transformed into a value to control the gates at various voltages to provide X percentage of current over X phase at X time. there are 3 phases the load must be divided/driven between.

asking what is best? I think is mostly user preference. or application needs. as there's positives and cons to both. 

Its not just about motor size, magnet size/types(different magnets can deform or demagnetize at different heat and emf index's). phase resistance etc etc. which is probably to complicated for something like a skateboard....so best to just leave these things to user preference of "feel". 

my opinion for skateboards is I like FOC, and the driving hz depends on your gear ratio, voltage and RPM to create smooth transitions. Other applications I'd say I like BLDC.

is the hardware we're using safe and designed for both? I'm not really to sure yet, I've been looking at the github and sources to try to determine that. Hope it answers some of your questions, lol...I don't like talking soo....
```

---
## \#16 Posted by: Hummie Posted at: 2017-08-20T16:42:25.934Z Reads: 325

```
so the sensors are used continuously, at all speeds, when in foc and they enable the esc to produce a true sine wave which would be more efficient at all these speeds?
is it safe enough to mess with all those 4 settings to a certain degree and see what the results are?
```

---
## \#17 Posted by: Deckoz Posted at: 2017-08-20T17:47:16.291Z Reads: 335

```
Which 4 settings? 
If I'm not mistaken
F_SW is the frequency sensor write (the kHz at which the sensor is read and written to the KI loop

DTC is the control cycle time. This is not something I would change unless you are familiar with calculating magnetic flux and torque deviation over time for permanent magnet motors.

the speed tracker and duty down ramp loops are essentially PID loops with no derivative function. Its used to compare deltas rate of change and control how reactive the loop is to the difference in change. KP ie proportional in most PID controllers, is the same as "present time". KI ie integral is "past time", and Kd ie derivative is "future time".  Again not values I would mess with unless you are familiar with how PID controllers work, your familiar with Vedders implementation of a PI controller, and you have reason to believe for your setup it would do better with change. 

I'm not sure if the bldc tool in its current state is capable of logging (like a blackbox) the multiple PID loops while riding to see if there is improvement that could be made to the Kp and Ki values to enhance performance. 

So in its current state I would probably only change the frequency of the sensor writes(F_SW) - be it as it may the PI loops may be optimized for a specific sensor cycle, but I have not looked deep enough in the code to find  out due to lack of onboard logging, as changing the PI loops would be blindly done currently.
```

---
## \#18 Posted by: Pedrodemio Posted at: 2018-04-08T03:19:25.431Z Reads: 292

```
Just increased from 20KHz to 30KHz, anyone tried higher? Now it’s barely audible, but for me it’s a little still, from the pitch I guess it’s a 15 KHz harmonic from the bell or something
```

---
## \#19 Posted by: Hummie Posted at: 2018-04-08T07:46:33.416Z Reads: 293

```
@Deckoz you and chaka seem to be saying opposite things here.  is the motor more efficient at a faster update rate or slower? 

I don't know what 4 parameters I was talking about before but can you please tell us more about any settings which might be worthwhile for us to learn about if we're trying to get:

best startup smoothness at lowest speeds
quiet
efficiency


the op says he got a smoother startup and quieter with reducing his switching frequency down to 20000 while @Pedrodemio moved his higher and got quieter.   are we talking about the "speed tracker" and "Ki"?
```

---
## \#20 Posted by: Pedrodemio Posted at: 2018-04-08T12:55:40.918Z Reads: 285

```
The switching frequency is simply the frequency the MOSFET’s are operating, the higher the less audible, until a point it doesn’t make difference to increase

But as you go higher you increase the loses on the transistors since they have to switch more time per second
```

---
## \#21 Posted by: Cobber Posted at: 2018-04-08T13:56:48.868Z Reads: 276

```
quoted from another page....

in response to a question where the op had 1-16KHz choices with his ESC software.

>PWM frequency has no effect on maximum torque and rpm, because at full power the PWM ratio is 100% (full on) so there is no frequency. At lower PWM ratios the frequency has an effect on motor efficiency and throttle linearity - the lower the frequency the worse it gets.

>PWM controls motor speed by switching the power on and off rapidly with a varying ratio, so the motor is getting getting a series of full power pulses. At low PWM frequency this causes extra loss due to vibration and current surges, but the increased rms current and voltage at mid throttle causes the motor to produce more torque and rpm than it would with the equivalent DC voltage. So you might think that it's more powerful, but that's only because the throttle response is non-linear. In reality more power is lost due to the higher rms current heating up the windings more, and the vibration wasting energy in the gears etc.

>As PWM frequency is increased the motor's winding inductance begins to smooth out current flow, so the motor runs more efficiently due to lower rms current and torque ripple. On the down side, higher PWM frequency causes higher loss in the controller. So you should choose a frequency high enough to make the motor run smoothly without making the controller get too hot. Inductance is proportional to number of turns, so the 13.5T motor could get away with a lower PWM frequency than the 4.5T. However if the controller can handle it I would just choose 16KHz for both.

https://electronics.stackexchange.com/questions/212665/what-pwm-frequency-would-give-higher-torque-or-rpm-for-a-brushless-dc-motor
```

---
## \#22 Posted by: Hummie Posted at: 2018-04-13T05:47:33.326Z Reads: 264

```
@Deckoz thanks for bearing with me on these side questions, but back to the op's question and adjusting the F_SW, if we could.   Why do you run it down at 20,000?  The OP @RiGo also went down and it seems ironic as its quieter and smoother, isn't that supposed to be happening at the higher frequency?    I haven't had a chance to mess with the F_SW yet but would like to know the possible dangers or limits.  Do you think a hub motor would more so benefit from a higher frequency than a motor with a 3:1 pulley?

[quote="Deckoz, post:9, topic:30928"]
Side note. Most RC escs have an input range from receiver/controller -&gt; ESC of 400hz - 32khz+. While the ESC -&gt; motor runs at 16khz as that is the limitations of the FETs(Slew Rate) in use.
[/quote]
are you saying this is the lower limit of the F_SW?  is there an upper limit or a danger in going too low or high, maybe within reason?

[quote="Nowind, post:14, topic:30928"]
be carefull you have to do new detection with a “correctur factor of 0.75” or anything…
[/quote]
whats this?
```

---
## \#23 Posted by: bevilacqua Posted at: 2018-04-14T18:34:08.308Z Reads: 253

```
today I tested FOC-30khz on both my Maytech 4.12 (C18-Modded) vescs. The noise difference is incredible :)  

(( Default 20khz -> 30khz ))
```

---
## \#24 Posted by: Nordle Posted at: 2018-04-15T07:01:01.898Z Reads: 249

```
Mosfet temperatures are the same?
```

---
## \#25 Posted by: bevilacqua Posted at: 2018-04-15T07:46:56.308Z Reads: 255

```
Yeah I was concerned about that, but didn‘t observe any difference. I run the Mosfets/drvs (for now) without heatsink in a ABS enclosure. T_max 40 degC rinding pretty hard (just 7km thoug)
```

---
## \#26 Posted by: Petertaylor Posted at: 2018-11-07T23:13:09.985Z Reads: 238

```
Built myself a VESC based Dyno system to investigate motor efficiency. This plot is pretty interesting. All runs except red on were at same settings, but default 20khz switching frequency. Red one is at 25khz. I didn't redetect the motor, as someone mentioned above, but i kinda don't see that changing anything. 
![switching%20frequency%20investigation|690x336](upload://dCx9PH7C5GEmxJ0kDnXNAAYAdRd.jpeg) 

Other than the red line, the color is a ballpark motor temperature guide. Warmer colors are warmer temperatures. 

Thought y'all might be interested in some data in the conversation about switching frequency. Not that it matters to everyone, but it's interesting and important to some.
```

---
## \#27 Posted by: Petertaylor Posted at: 2018-11-07T23:46:42.236Z Reads: 237

```
Did a few more tests. Redetected for with the 16khz selected (didn't improve matters). Reset to 20khz and ran another test (run 15, purple). It aligns nicely with prior results, so nothing much changed. 
However, even 1 khz above or below 20khz, and efficiency is dramatically reduced. Interesting. Seems like perhaps there is a setting that's hardcoded in the firmware that assumes 20khz. Perhaps something optimized about the MOSFETs? Any ideas?

![switching%20frequency%20investigation_2|690x335](upload://hIRktfyWX35smyPzs7EVUYM5L1v.jpeg)
```

---
## \#28 Posted by: Deodand Posted at: 2018-11-08T00:53:44.047Z Reads: 223

```
are you running the latest firmware?
```

---
## \#29 Posted by: Petertaylor Posted at: 2018-11-08T00:57:20.866Z Reads: 221

```
Yep, 3.40.
```

---
## \#30 Posted by: Pedrodemio Posted at: 2018-11-08T01:00:38.036Z Reads: 218

```
Really interesting results, I can try to do the same route with both settings to see if in the daily use there is this big difference
```

---
## \#31 Posted by: Petertaylor Posted at: 2018-11-08T01:18:28.545Z Reads: 220

```
Watch out a bit if you do Pedrodemio, if the lower switching frequencies really are this much less efficient, you'll get much more heating (or noise?) from your motor/controller. Energy has to go somewhere, right?
```

---
## \#32 Posted by: Pedrodemio Posted at: 2018-11-08T01:27:57.848Z Reads: 221

```
I will log both rides and post here, but I will have to wait the weather to calm down, it's pretty windy these last days which would interfere with the test, unfortunately I don't have thermistors on the motors, but will put in a few weeks and we can see if the diference show up

But, and a big but, I remember the first time I rode this new board and was getting around 8 Wh/km, but the noise was really bad and after a few weeks changed to 30 kHz, now after lots of kilometers my global consumption is 9,7 Wh/km. I always attributed that to being accustomed with the board, but maybe there is more to it
```

---
## \#33 Posted by: Deodand Posted at: 2018-11-08T01:54:07.877Z Reads: 223

```
Do you have any documentation of your test setup anywhere? Would love to see it!
```

---
## \#34 Posted by: Hummie Posted at: 2018-11-08T02:20:24.319Z Reads: 218

```
To confirm the temp sensor is in the motor not the esc right?  Maybe it would depend on the amount of inductance and kv
```

---
## \#35 Posted by: Petertaylor Posted at: 2018-11-08T02:41:33.112Z Reads: 229

```
Not great documentation, yet. I'll document it a bit more completely soon (days?). For now here are the main points.

1. Custom python script, commanding test motor, brake motor, and an arduino reading a load cell via usb/serial.
2. Cheap Load cell, 5kg.
3. Custom frame. The motor that is cantilevered out has a "tailstock" type support to limit vibrations i was getting at certain rpms. Two motor shafts rigidly connected together.
4. Two identical batteries, 8s lipo, 6000mah. One draining, one regeneratively charging.

Basic script flow-
Test motor commanded to run at a duty cycle or rpm (doesn't seem to matter). Basically run as fast as it can. It has a VESC power limit of 450w (constraint simulating my application).
The brake motor is spun up by the test motor. When at top speed, it's commanded to gradually increase braking current until it's loaded the test motor to its power limit. From here, take a set of x samples, average them, check their standard deviation. Assuming they're pretty close, record stuff and increase the brake current a bit and do it again. If there is insufficient stability in test motor rpm, take a little longer to sample, but move on if it can't stabilize in 100 samples. When it hits the lower test range limit, or one of the other limit parameters are reached (too much current, battery too full/empty etc), quit. 
It dumps a bunch of data to a csv, and i load that into excel to graph and compare. 

![IMG_20181107_181611|666x500](upload://6eVFii01eDiX6rMN0WsOWXUZTTq.jpeg) 

![IMG_20181107_181604|666x500](upload://b777k8bUaSdiC5TKHz8rHRsJJ40.jpeg) 


![IMG_20181107_181629|666x500](upload://2ibq80VmEVzVxcHG3ZeYRwnr52h.jpeg)
```

---
## \#36 Posted by: Pedrodemio Posted at: 2018-11-08T02:47:37.786Z Reads: 210

```
Really nice setup

These motors you are using have a nigher pole count right? Maybe the higher inductance of them has something to do, but it still doesn't make sense that inly 20 kHz is the most efficient, have you tried something like 20001 Hz or other small variation?
```

---
## \#37 Posted by: Petertaylor Posted at: 2018-11-08T02:50:27.932Z Reads: 209

```
Testing the other motor in this current setup. Stock length wires (hella long). This one seems to like higher switching frequencies better, leading me away from the conclusion that the VESC had some build in bias towards 20khz. Just a coincidence on the last motor. Only a few runs, but the trend is pretty clear, i think. Not really anywhere enough data to draw really confident conclusions, but it's better than nothing. 

![turnigy%20multistar%20100kv|690x334](upload://7CYLMGjCWB2kaETPZ8M5vffHPgC.jpeg)
```

---
## \#38 Posted by: Petertaylor Posted at: 2018-11-08T02:54:34.819Z Reads: 214

```
Pedrodemio, yeah my application is a solar powered boat, so ideally i'm looking for low rpm, high efficiency motors. I've also tested (before the setup was as dialed as it is now; no "tailstock" before)  a popular eskate motor, the Turnigy sk3 260kv. I'll return to that one to do some more testing. I didn't try different switching frequencies on that, didn't think it'd have much effect, but i'm proving myself wrong on that :slight_smile: 

![combined_new_routine|690x335](upload://oTfYZSPSYlT29ObH3c3msrOlyep.jpeg)
```

---
## \#39 Posted by: chuttney1 Posted at: 2018-11-08T02:55:07.146Z Reads: 205

```
Regarding the data. What does it mean in terms of torque produced?
```

---
## \#40 Posted by: Pedrodemio Posted at: 2018-11-08T03:03:05.208Z Reads: 204

```
Nice, to you have more info about it somewhere?

Also it may be worth testing in BLDC, even if it will be probably less efficient
```

---
## \#41 Posted by: Petertaylor Posted at: 2018-11-08T03:03:59.145Z Reads: 206

```
[chuttney1](https://www.electric-skateboard.builders/u/chuttney1)
Power, torque, rpm are all linked via simple formulae. 
https://www.engineeringtoolbox.com/angular-velocity-acceleration-power-torque-d_1397.html

Basically, at a given input power and rpm, there is a maximum torque that's produced. Multiply that torque by the efficiency (0.85 is 85%) to get the actual torque output. There are calculators out there that'll let you avoid the math and unit conversions. 
https://www.engineeringtoolbox.com/angular-velocity-acceleration-power-torque-d_1397.html

To me, i prefer to think about power in, efficiency and rpm as input variables, and torque being a result of the efficiency.
```

---
## \#42 Posted by: Petertaylor Posted at: 2018-11-08T03:05:09.110Z Reads: 206

```
[Pedrodemio](https://www.electric-skateboard.builders/u/Pedrodemio), i did start with BLDC, and in my first couple tests, it seemed a couple percent lower efficiency, so i kinda stopped testing. I'll go back and see what else shows up. Easy to change and test.
```

---
## \#43 Posted by: Petertaylor Posted at: 2018-11-08T03:51:46.480Z Reads: 203

```
Think i managed to include a dodgey run in the last set, which offset the conclusions. 
![turnigy%20multistar%20100kv_2|690x333](upload://hJrzp6ZzM1Wcs4sgjWYE8UVgbQe.jpeg) 
Omitting the first run, which didn't have a strong curve, and seemingly lots of noise (like run5?), it seems that the same trend of 20khz being the preferred frequency has re-emerged. 

Not sure why that first run was so bad. Will think on that one.

Runs are numbered chronologically but the legend lists them in order of frequency. Switched battery half way through, but i don't think that had a strong effect. Ideally i'd have a fatty lab power supply, but then i'd have to have a scheme for dumping the generated energy too.
```

---
## \#44 Posted by: Deodand Posted at: 2018-11-08T09:52:25.376Z Reads: 201

```
You need your own thread for this setup man! It is good stuff.
```

---
## \#45 Posted by: taz Posted at: 2018-11-08T10:12:49.977Z Reads: 201

```
This is very interesting.
I have not done any extensive testing like you, however I changed the FOC frequency from 20 to 30kHz in an attempt to reduce noise even further and for the first time my FocBoxes exceeded 80C and started to cutout.
This is the first time this has happened as it is usually my motors that overheat first.
I think I will go back to 20kHz.
```

---
## \#46 Posted by: Hummie Posted at: 2018-11-08T17:27:10.907Z Reads: 200

```
Why would the switching frequency effect the motor?  I can imagine inefficient torque pulses at a really low frequency But at the high frequency wouldn’t it smooth the current flow and hit a point of ideal efficiency based on the inductance and capacitance at that point when the current in the primary waveform is smooth as can be?
Looking around the web I don’t see an explanation for motor heating due to increased frequency but much to the contrary 
https://kebblog.com/vfd-switching-frequency/
```

---
## \#47 Posted by: taz Posted at: 2018-11-08T18:17:35.756Z Reads: 199

```
If you are replying to me, what I wrote is that it is the vescs that overheat when increasing the switching temperature.
Motors overheating is irrelevant to switching frequency in my case.
```

---
## \#48 Posted by: Petertaylor Posted at: 2018-11-08T18:58:15.408Z Reads: 194

```
Hummie, i think you're right in that i don't think there is a reason a higher switching frequency would negatively affect a motor. In my tests the motor and controller are considered together, so it could be that while the motor is marginally _more_ efficient, the controller get _less_ efficient by a greater amount. I guess there could be some negative capacitive and/or inductive effects, but i'm not sure i'm smart enough to figure that out :-/

Also, in my offhand remark about the motor temperature (if that's what you're referring to), the "measurement" was an approximate and subjective one. "I've run it a few times back to back, and the same test twice in a row gives slightly different but consistent results, i wonder why, oh, the temperature is definitely higher, let's let it cool off a bit and do another" type deal. No real science/measurement there (as if there was rigor elsewhere).

I'm absolutely no EE, but the interwebs says this about MOSFET switching losses _"The other source of power loss is through switching losses. As the MOSFET switches on and off, its intrinsic parasitic capacitance stores and then dissipates energy during each switching transition. The losses are proportional to the switching frequency and the values of the parasitic capacitances. As the physical size of the MOSFET increases, its capacitance also increases; so, increasing MOSFET size also increases switching loss."_

https://www.eetimes.com/document.asp?doc_id=1278970
```

---
## \#49 Posted by: Hummie Posted at: 2018-11-08T19:01:00.262Z Reads: 184

```
Thanks.  I’m believing the heat is only increasing with increased frequency in the esc at the fets

Especially with the low kv we use maybe we could go down to a lower frequency for ultimate eff. I’m more and more wanting an oscilloscope to see the different harmonics.
```

---
## \#50 Posted by: Petertaylor Posted at: 2018-11-08T19:25:47.131Z Reads: 183

```
Yeah, i've got a USB scope that i'm thinking i might hook up to this and see what the waveforms look like. 

In my testing, i was surprised that i got a _lower_ efficiency with a lower switching frequency. I'd heard that higher frequencies would be less efficient, so that wasn't surprising, so i'm a little confused about the lower frequencies. My guess is it has to do with the PID constants. I haven't changed those from their defaults, and they are likely set up to work well with the 20khz default. The curves i'm getting are much more erratic under 20khz, so perhaps it's hunting a bit more? I haven't investigated PID changes yet, but that might be another interesting thing to chase after (along with the scope reading)
```

---
## \#51 Posted by: Deodand Posted at: 2018-11-08T19:30:37.960Z Reads: 186

```
the control loop of the FOC algorithm runs at 0.5*pwm frequency. The current controllers is designed to have a 1000 us (1kHz) time constant by default . As a rule of thumb, it's wise to run your controller at about 10x the controller frequency to avoid aliasing effects so its possible tuning down the current controller time constant at lower pwm frequency could help.

Lower pwm frequency results in lower switching losses on the vesc but can generate more losses in the windings due to higher ripple current in the motor (more losses during current spikes with i^2)
```

---
## \#52 Posted by: Petertaylor Posted at: 2018-11-08T20:28:43.684Z Reads: 184

```
Fascinating! I haven't poked around too much in the VESC firmware, other than the confirm serial communication format, and research on an issue with braking duty cycle below 5%. 

In my config, i've got a vesc 6, and sample V0 and V7 is enabled, which according to the tooltip means it's actually sampling at full 1* pwm freq. 

Any thoughts or can anyone point me towards a vesc pid tuning guide?

As to the current spike losses in the motor, that's an interesting point, but i'd imagine that there is still an optimal balance between motor losses and vesc losses, and it's unlikely to be 20khz. There will be a superposition of the two efficiencies that is lowest, what frequency is that at? Surely it'll change per motor, and perhaps with different models of vesc. 
Why do both the motors i've investigated frequency on (on the same controller, but i've got two, and perhaps that's the next test, run a known motor on the 4.12 controller and see what the differences are) have max efficiency at 20khz?
```

---
## \#53 Posted by: chuttney1 Posted at: 2018-11-08T20:36:20.282Z Reads: 182

```
[quote="Petertaylor, post:50, topic:30928"]
see what the waveforms look like.
[/quote]

Generally, the waveform for a bldc motor is a step-like pattern in the shape of a sine wave unless you are talking about the one where you can see the switching of the mosfet on and off.
```

---
## \#54 Posted by: Petertaylor Posted at: 2018-11-08T20:43:47.484Z Reads: 178

```
You're right about the simulated sine wave, i think, but that's the ideal waveform, what does it _really_ look like? How mangled are the leading and trailing edges of the steps from capacitance? What about voltage spikes from changing/collapsing magnetic fields? What about frequencies too high for wires that are too big (lots of skin effect?). We could theorize about all that, but just putting a scope on it and seeing for real (understanding that the scope will also load and change the circuit very slightly) would be illuminating.
```

---
## \#55 Posted by: Hummie Posted at: 2018-11-08T20:53:01.620Z Reads: 177

```
This shows wire diameter and frequency and skin effect
https://chemandy.com/calculators/skin-effect-calculator.htm
```

---
## \#56 Posted by: professor_shartsis Posted at: 2018-11-08T20:56:31.303Z Reads: 184

```
[quote="Petertaylor, post:54, topic:30928"]
You’re right about the simulated sine wave, i think, but that’s the ideal waveform, what does it *really* look like?
[/quote]

[quote="chuttney1, post:53, topic:30928"]
Generally, the waveform for a bldc motor is a step-like pattern in the shape of a sine wave unless you are talking about the one where you can see the switching of the mosfet on and off
[/quote]

BLDC:
https://image.ibb.co/gwsyy8/32802_F14_5_EA2_4_A35_AFE0_123_A2_E429_AD4.png

^in bldc/block commutation, the switching frequency affects the spacing of the tiny current spikes, which averaged gives the motor current value (2 phases are always powered while one has avg ~0a current), but the switching frequency does not affect the overall commutation timing or avg current value...

as the switching frequency gets lower, this plot will look more "toothy" & "jagged..." & as the frequency gets higher, the plot will look smoother and less jagged.

FOC will look more like this with a sinusoidal waveform, with all 3 phases energized simultaneously (except for the 0a crossings):
https://image.ibb.co/dBMfBT/3_D4_EC104_25_CA_421_A_8820_56_D249_F4245_F.png
```

---
## \#57 Posted by: Petertaylor Posted at: 2018-11-08T20:58:26.028Z Reads: 175

```
For skin effect, 
https://chemandy.com/calculators/skin-effect-calculator.htm

I get ~500uM which is 0.5mm at 0.02Mhz = 20khz. 

Appreciable number, but i'm not sure if there will be a real effect.
```

---
## \#58 Posted by: professor_shartsis Posted at: 2018-11-08T21:39:07.153Z Reads: 174

```
@Petertaylor i wonder whether each separate motor's differing inductance value influences the "most efficient" switching frequency?
```

---
## \#59 Posted by: Petertaylor Posted at: 2018-11-08T21:43:57.988Z Reads: 171

```
I absolutely would have thought so, but the tests seem to prove otherwise. That's the bit i'm wondering if the community can speak to. The two motors here are very similar however, so perhaps it's just blind luck that they are at the 20khz mark.
```

---
## \#60 Posted by: professor_shartsis Posted at: 2018-11-08T21:48:02.348Z Reads: 176

```
@Petertaylor I suspect, for example, a motor with very low inductance would require a much higher switching frequency to prevent the current plot from becoming too "jagged..."
```

---
## \#61 Posted by: Petertaylor Posted at: 2018-11-08T22:03:35.124Z Reads: 168

```
I just measured (with the vesc) each of the motors in the setup, and the two i posted plots for yesterday.
The more efficient of the two (HobbyWing x-rotor 8120-100kv) is at 6.27uH
The less efficient, (Turnigy 9235-100KV Multistar ) is at 11.14uH. 

I'm going to set up the scope in a second and see what i can see.
```

---
## \#62 Posted by: professor_shartsis Posted at: 2018-11-08T22:31:27.193Z Reads: 169

```
[quote="Petertaylor, post:61, topic:30928"]
The more efficient of the two (HobbyWing x-rotor 8120-100kv) is at 6.27uH
The less efficient, (Turnigy 9235-100KV Multistar ) is at 11.14uH.
[/quote]


@Petertaylor do you think the "more efficient" motor has lower inductance from having less iron/stator volume and therefore more room for copper... lower resistance & lower inductance... more efficiency?
```

---
## \#63 Posted by: Petertaylor Posted at: 2018-11-08T23:09:20.592Z Reads: 164

```
good question. 
I'm absolutely no expert on this stuff (read on), so i really couldn't tell. I'd like to know, but i'm not there yet :-/

Also, guess who just fried their usb o-scope? Yep, forgot that while i could drill-scope motors at low rpms and get low induced voltages, the Digilent AD2 only has a max voltage of 26v. The difference between phases on the motor was at ~50v at its peak. Looks like just one SMD component next to the usb port, but you never know. I'll use this as an excuse to get a real scope...

So, the scope trace will have to wait until i get a real scope (few days? a week?)
```

---
## \#64 Posted by: Petertaylor Posted at: 2018-11-21T21:48:26.800Z Reads: 152

```
Well, new scope here. Proper scope that can handle higher voltages. I was a dummy before, and it wasn't the scopes fault. Anyhow. Currently can see each pulse, with a changing width to average to a sine wave, but need to figure out how the have the scope do the math/averaging to translate those small pulses into the sine wave it's approximating. Any ideas?

edit: What i want is to graph the average voltage over a known and constant switching frequency. That'll give an idea of what the sine-wave should be looking like. I'm a rookie with scopes.
```

---
## \#65 Posted by: Pedrodemio Posted at: 2018-11-22T00:24:25.200Z Reads: 153

```
What if you did an analog low pass filter before the scope? Just a resistor and a capacitor
```

---
## \#66 Posted by: Petertaylor Posted at: 2018-11-22T02:02:23.458Z Reads: 154

```
Yeah, that's kinda were i think this is headed. 
Been futzing around with Low Pass filters on the scope directly, but the resolution of the result is either  ok and noisy, or lousy resolution and smooth, but the oddities from the imperfect sine wave back emf and switching frequency changes will be lost.
Grrr. It's always something.

The worry is that by adding a filter, i'll smooth out the stuff i'm looking to detect. Trying to simulate a filter now. since the FOC sine wave period is variable (with rpm), the filter needs to be adjustable too, unless i'm happy running tests only at one eprm. Wondering if i can't capture a wave and do the moving average in excel ort whatever. Definitely slower, but the variables are easily controlled.
```

---
## \#67 Posted by: Pedrodemio Posted at: 2018-11-22T02:13:49.506Z Reads: 149

```
MATLAB has some pretty powerful filtering tools in Simulink, might be worth a look

About the real life efficiency test is in my todo list, the weather is not cooperating, it hasn’t stopped raining for enough time for the pavement to dry and to make all test in one go
```

---
## \#68 Posted by: Petertaylor Posted at: 2018-11-22T02:35:47.587Z Reads: 151

```
Yeah, i don't have matlab, and it's not free. I'm a student, so i think i can discounted SW, but free is better :slight_smile:
I've used octave quite a bit, but haven't seen anything there that looks like it'd help too much. I'm pursuing the excel path as we speak, will see how far i can get with that.  
Not really a big fan of matlab or octave tbh. I don't really see what it does that python with numpy and the various other libraries can't do, but that's probably my inexperience with the software/applications it's useful for.
```

---
## \#69 Posted by: Petertaylor Posted at: 2018-11-22T05:02:47.400Z Reads: 153

```
Well, i'm getting the same thing when doing the analysis on the computer. Excel croaks past 1M lines, but the interface for the usb scope i blew up accepts the output from my new scope. It's reasonably fast at processing it all too. 6M samples was enough data without taking 20 minutes to write to thumb drive, but after applying a low pass filter, the results are still total mush. 

![vesc%20waveform2|690x378](upload://nybAjK4NclCi9JUxNFR9hxor4cX.png) 

Low pass filtering just isn't the way. All the detail is gone (stands to reason peter, duh).
The switching is clearly visible, and the underlying sine is there too. It's the right frequency (i was running at 12000erpm so 200 electric revs/sec = 5ms period. There has to be a smarter filter to apply, or some other method. Perhaps not trying to see the sine wave but more looking for the noise or deviation from a perfect sine of the same frequency?

I'm measuring one phase relative to ground. Don't think there is any other way to do it differently. 

Not sure what the right way is. Also, i've gotten sidetracked. Seeing the waveform is interesting, and i don't like to back down from a challenge/failure, but having the knowledge that for whatever reason efficiency is highest at 20khz (vesc 6) is the thing i came for. I've got a few more motors to test on the dyno. I'll give the waveform question some thought. If someone has some good ideas, i'd like to know. I can do some more testing as suggestions pop up. if anyone wants the raw capture data (120mb csv file), lemme know. I'll ask the grey-beards i know too. 

One day i'll figure it all out.
```

---
## \#70 Posted by: Pedrodemio Posted at: 2018-11-22T12:21:38.391Z Reads: 141

```
I got lost a bit, what are you trying to visualize? The sine wave smoothed out? Like the motor would see?
```

---
## \#71 Posted by: Petertaylor Posted at: 2018-11-22T18:52:50.957Z Reads: 147

```
So i'm trying to figure out what's changing, or why there is a drop in efficiency when the PWM switching frequency is changed from the default of 20khz. 

I hoped to be able to run a motor at a constant load on the dyno, scope the waveform, change the switching frequency, run the same motor, same load, same everything (except  pwm freq.) and scope that new waveform. 
I expected to see something that illuminated why 20khz was preferred. Is the sine fatter? Skinnier? Is there a lump in it? I guess i'm hung up on seeing a sine wave. That likely isn't necessary. Perhaps a FFT plot will show some harmonic? Maybe looking at each pulse away from 20khz will show a weird shape, slow rise or fall time? Not sure what would cause this decrease in efficiency, but it's gotta be in there somewhere...

In general, lower pwm frequencies should deliver high efficiencies, and yet that's not what my tests have shown, on two seperate motors with multiple runs out of sequence with each other.
```

---
## \#72 Posted by: Pedrodemio Posted at: 2018-11-22T20:04:35.369Z Reads: 144

```
Yeah, FFT is your best bet, if something is different it will definitely show there

Another thing, where are you getting the current sensing? Using vesc itself to log? Maybe there is something going on just on the measurements of the power and energy
```

---
## \#73 Posted by: b264 Posted at: 2018-11-23T01:19:32.980Z Reads: 143

```
[quote="Petertaylor, post:69, topic:30928"]
There has to be a smarter filter to apply, or some other method
[/quote]

Measure with the motor attached or another inductor -- and run motor detection with the scope attached first.  Maybe?
```

---
## \#74 Posted by: Deodand Posted at: 2018-11-23T23:25:13.476Z Reads: 139

```
[quote="Pedrodemio, post:72, topic:30928"]
Another thing, where are you getting the current sensing? Using vesc itself to log?
[/quote]

Definitely agree to use external power measurement from the vesc. Depending on duty cycle/sampling window/load I've seen very strange outputs from the current sensing of the vesc at times.
```

---
## \#75 Posted by: Pedrodemio Posted at: 2018-11-24T01:46:37.501Z Reads: 138

```
I think that only real life test without having an external meter would be run the board to empty ridding at the same conditions

I may do that but only charging to 36v or something like that, doing the same circuit at constant speed for 40km does not sound fun, did it once to test my range under ideal conditions
```

---
## \#76 Posted by: Petertaylor Posted at: 2018-11-24T03:50:49.007Z Reads: 137

```
Deodand, Pedrodemio
I've been doing the current and voltage measurement from the vesc via python. Seems accurate enough for what i'm doing, particularly since i'm averaging 10 samples to come up with my measurements. Likely the vesc is already doing some averaging internally to get the result it presents. I've got an inline current sensor i can use, it'd just take changing the code, and having the arduino read that input and send it to the computer. Don't think it'll matter though. Look at the curves posted [earlier](https://www.electric-skateboard.builders/t/changing-foc-switching-frequency/30928/43?u=petertaylor). Pretty obvious trends for the most part. 

I'm not measuring current at all on the scope however, just voltage. I guess the inductive qualities of the motor might(/should if the controller is doing its job?) be enough to smooth/average the wave and let me see what i want to see on the scope. Not sure how to best measure current on a scope without expensive probes :-/ 

I did try a super low tech idea, which was to probe a wire wrapped around one of the insulated phases coming out of the vesc. Saw a steppy looking wave that approximated a sine, but it was at 10khz (this was with the other vecc, 4.12 hardware, so half of 20khz programmed frequency). That frequency means it's just a modified version of the pwm pulses, and not indicative of current sine wave. I should have got 200hz for the current sine wave. The steps were the EM waves from the nearby two other phases, i think. 
Thoughts?
```

---
## \#77 Posted by: Petertaylor Posted at: 2018-11-24T03:52:39.038Z Reads: 127

```
b624, not sure what that would get me. Do you think the scope is interfering with the motor and should be in the system during detection? It should be basically invisible to theses voltages and currents.
```

---
## \#78 Posted by: Pedrodemio Posted at: 2018-11-24T16:53:26.549Z Reads: 131

```
I think it’s worth a try using your external current measurement, as @Deodand said the vesc measurements can be really off it for example the energy sampling is hardcoded somewhere and it gets out of sync by changing the switching frequency

Did you post anything or vedders forum? He take a long time to reply but this discussion is extremely important in my point o view, we try a lot of thing to make our boards more efficient, but if we throwing energy out just to make out boards silent it needs to be reviewed 

@trampa could you please talk to Benjamim about it? Just see what he has to say, thanks
```

---
## \#79 Posted by: trampa Posted at: 2018-11-24T20:23:28.840Z Reads: 138

```
I will, but please open a thread on vesc-project.com. For the motors we use, standard settings work just fine. There is probably little reason to change that, and little gain. We tested a 30kW 0.7uH inrunner last weekend and such a motor definitely needs a lot higher switching frequency. Most of the motors used in skateboarding are pretty similar outrunners. 

Probably it's possible to auto tune the switching frequency. Benjamin is currently working on auto everything that can possibly be automated. Many things are not trivial though. 

[quote="Pedrodemio, post:78, topic:30928"]
we try a lot of thing to make our boards more efficient, but if we throwing energy out just to make out boards silent it needs to be reviewed
[/quote]
Or if you throw energy out using no gearing....The correct transmission and matched motor has magnitudes more impact on efficiency. Also choice of wheels, surface of the track, ride style etc. impacts the efficiency a lot. Battery pack size, battery voltage, voltage sag, twin or single drive...
If your motor and ESC stays cool, you are not experiencing drastic losses. Losses always go into heat. You could just monitor temperatures while playing around.  Things will also depend on the design of the ESC. The three phase shunts design of the VESC 6 improved FOC big time. Data readings are more precise and in consequence FOC computation is a lot more precise.
```

---
## \#80 Posted by: Deodand Posted at: 2018-11-24T21:53:35.491Z Reads: 139

```
[quote="trampa, post:79, topic:30928"]
You could just monitor temperatures
[/quote]

Interesting point, if you had identical vesc's the delta T of each one could be looked at as a possible measure of efficiency for the motor controller itself at the end of the test... of course the motor itself may have more or less losses depending on switching frequency also. I'd guess it depends on the impedance of the L-R circuit within the windings, such a circuit will have a frequency response plot and will be most efficient near the peak of said plot.

Also @trampa I think this project can be seen as a good way to look at individual factors and how they play into the vesc performance alone. One need not take a global view of the entire skateboard all the time. Even if the efficiency gain for the entire system isn't significant it could improve the relative efficiency of the vesc itself which would enable larger current throughput at that stage provided you have ample sized motors to handle it.
```

---
## \#81 Posted by: Pedrodemio Posted at: 2018-11-24T22:05:20.948Z Reads: 135

```
The main reason for decreasing noise, at least for my motors the default 20 kHz make almost the same noise as BLDC, at 30 kHz is dead silent
```

---
## \#82 Posted by: trampa Posted at: 2018-11-24T22:29:34.235Z Reads: 136

```
The ESC is like 99% efficient already. Not much to gain here. If the entire system is not totally perfect optimized, there is no need to talk about slightly optimizing the switching frequency. 

Question is: how far to the edge of the theoretical output performance do you want to go.  If you hardly ever push the ESC to its limits it will stay very cool all the time. If you push to the limits, better cooling will have the biggest impact on efficiency and losses.  
Strap a VESC 6 to to 5Kg of alluminum and you can push 120A continuous all day long. 
If you are not completely off the ideal frequency, we are talking point x gains or losses. Benjamin is the expert, he will be able to give good advice and further explanations. 
Standard settings work a treat for nearly all bldc outrunner motors used in skateboards.
```

---
## \#83 Posted by: trampa Posted at: 2018-11-24T22:31:37.109Z Reads: 131

```
Then run it like that and see if it impacts temp and range. If not, you have a silent efficient board.
Benjamin also plays around with it a bit.
```

---
## \#84 Posted by: Deodand Posted at: 2018-11-24T22:41:50.590Z Reads: 130

```
Currently the major driving cost of the VESC is the FETs, they have to be high performance. I agree it is 99% efficient in most cases, that isn't the point. The point is that during high power draw 1% is a lot of heat. If you decrease that 1% to 0.5% it saves you basically no energy at a system level, however it does mean that half the heat will be generated within the VESC. Suddenly you don't need to strap it to a giant aluminum block for high power, or use more expensive/larger quantity of fets to push the same amps. The relative efficiency gains within the vesc can go a long way toward reducing its own cost/mass/physical footprint/ longevity due to high operating temperatures. I would never discourage people from analyzing what parameters can impact the efficiency of this system.
```

---
## \#85 Posted by: trampa Posted at: 2018-11-24T23:14:18.213Z Reads: 129

```
Sure, that's exactly why you want to overrated your ESC. It stays cooler and is more happy on the long run. 
The more you design it to the edge, the more it will suffer from heat if cooling is limited. 
If your average Amp draw is low, the .x % doesn't matter so much. If you drain a lot all the time it becomes more relevant. I'm not saying it's not worth to experiment! 
There is definitely less efficiency if you go for higher switching. I personally enjoy the silence. If it matters in reality, for your setup, can be seen after doing some rides and comparing temp and Wh usage per km.  Pull out your phone and read the data. As long as Mosfet temp stays reasonable low you are good. The range will probably not be affected a lot.
```

---
## \#86 Posted by: Deodand Posted at: 2018-11-24T23:21:06.508Z Reads: 138

```
I agree range will not be impacted significantly. Higher switching frequency can in theory result in higher efficiency for certain systems, but switching losses will increase. Switching losses are generally not dominant for the regime we are operating in, my tests have shown Rds on is a much more relevant player in the losses for the vesc scale systems. 

If there is something funny going on with bad sample timing etc. at switching frequencies which are not the default 20 kHz it would be very useful to identify and fix any small oversight here. Many people would prefer to run 25-30kHz for quieter operation, and simply writing it off saying what we have is good enough isn't the spirit of this forum. 

Something like an assumed timestep not being updated in one of the estimators could be culprit. I will be keeping an eye out to see if I can spot any funny business next time I go through the code.
```

---
## \#87 Posted by: trampa Posted at: 2018-11-24T23:59:07.025Z Reads: 135

```
It's simple: you trade noise with heat. If your ESC is very beefy (relative to the system), it doesn't matter so much, if it's designed to the edge it starts to matter. Simple to find out with a reality check monitoring the temps. Some people ride with PU wheels on tarmac in flat areas, other do hard-core offroad riding in the mountains. 
Average Amp draw is totally different.
Benjamin has implemented all the RT data, so it's easy to see what happens if you change values. 
Just change the value and have a look what happens. Share your experience - nothing is written off.
```

---
## \#88 Posted by: Deodand Posted at: 2018-11-25T01:31:36.045Z Reads: 129

```
If only life were so simple.... the way you describe it is wildly over-simplifying the problem.  As I've said many times some motors will operate more efficiently at higher switching frequencies. Especially larger motors with lower resistance or ironless stators with less inductance. If making ESCs efficient was so simple it wouldn't have taken somewhat as smart as Vedder to tackle it in the first place. There are **MANY** factors contributing to what switching frequency is most efficient, we shouldn't see 20 kHz always being  the best like his data is showing. Also if your statement was correct than why isn't 10kHz more efficient? Think a little. 

I can guarantee you also that things are sometimes written off. There is no shunt resistor on the input of the vesc so measurements of input current are back calculated from applied motor voltage and measured motor amps. These measurements aren't always accurate for various reasons. Stop acting like the business man with a blindfold on pretending your product is perfect and think like a researcher asking, what possible variables could be contaminating the results?
```

---
## \#89 Posted by: Petertaylor Posted at: 2018-11-25T01:59:34.118Z Reads: 131

```
So i did start a [post](https://vesc-project.com/node/658) about my data over on the official vesc forum, and no one seems to have noticed or commented. Please point vedder at this thread or that one. I'd be interesting to hear his take. I do think there is likely something in the firmware that's assuming 20khz switching, and when you change the value, things don't line up like they should. Lots of code, and i don't really wanna rake through it all if i can avoid it. 

Trampa, my application is not skateboards at all, so the talk of whole system efficiency doesn't translate. I have other efficiency losses in my project (solar panel I-V curve, and propeller design/optimization). I'm racing a solar powered boat, and every last percent matters with limited power (i'm lowering the oil viscosity in a planetary gearbox tonight to increase efficiency at a loss of lifespan, for instance). The reason i stumbled into this data showing 20khz is preferred is by attempting to squeeze a couple more percent from my system. If race day was tomorrow, i'd run it at 20khz. If we can figure out the issue, i'll run the ideal switching frequency for my chosen motor and perhaps pick up a percent or two.

Also, it's just interesting to investigate and understand systems. If there are bugs, we need to identify and squash them. If this is an issue with my methodology (it could be), then i wanna know where and how, so i can get better data. For most of folks, none of this matters. It doesn't really matter to me either, in the end; who cares about a stupid boat race? But the knowledge and process is valuable.
```

---
## \#90 Posted by: Petertaylor Posted at: 2018-11-25T02:07:59.468Z Reads: 126

```
> The ESC is like 99% efficient already. Not much to gain here. If the entire system is not totally perfect optimized, there is no need to talk about slightly optimizing the switching frequency.

The thing is, from my data, it seems like up to a 6% difference in peak vesc+motor efficiency changing from 20khz to 18khz. That's pretty significant. Not sure if that is going into the motor, or the vesc. If the motor can handle it, it should be more efficient at 18khz, not less efficient, so i presume the extra loss is in the motor.
```

---
## \#91 Posted by: Gamer43 Posted at: 2018-11-25T04:42:34.116Z Reads: 133

```
I would just like to add, if you use VERY large motors, such as hoverboard hub motors, there is a significant difference in upping the switching frequency from the default 20khz to around 28-33khz, both in noise and no-load current draw. If I tried switching frequencies above 35khz, there was a faint high pitched whine coming from the motors.

If you are using default hardware, increasing the switching frequency will actually generate significantly more heat since International Rectifier MOSFETS have literally the worst gate charge characteristics in the industry, resulting in excessive switching losses. Above 30khz, the drv830x's charge pump actually can't keep up with the current draw at those switching frequencies. Gate drive voltage starts to sag and you get excessive conduction loss added to the already terrible switching losses.

Since most hobby motors (5065, 6374, etc.) run fine on trapezoidal control since they are high speed bldc motors (with concentrated windings), changing the switching frequency in field oriented control for those motors often has little effect unless you go below 15khz or above 40khz (in which case the effect is negative). 

If you are using larger motors such as hub motors, or a proper PMSM with distributed windings, higher switching frequency is usually better, up to a point. At excessively high frequencies, switching losses will generate excessive heat, resonance and other phenomena start screwing with your motor, and gate drive voltage will sag too much and trigger UVLO.
```

---
## \#92 Posted by: Petertaylor Posted at: 2018-11-25T05:44:57.008Z Reads: 132

```
>If I tried switching frequencies above 35khz, there was a faint high pitched whine coming from the motors.

35khz is above human hearing, what whine would you be hearing? Where would it be coming from? What frequency sound?
_Edit: Perhaps harmonics at the resonant frequencies of various mechanical stuff in the motor would be within the audible range. RPM would shift this into/out of the resonant range though, so it'd only be audible at certain frequencies._

> changing the switching frequency in field oriented control for those motors often has little effect unless you go below 15khz or above 40khz (in which case the effect is negative).

i've got a 6% system loss at peak efficiency from two different motors (same controller) going from 20khz to 18khz and 19khz. That's not a "little effect". The motors are similar form factor, same kv rating, different pole counts however.
```

---
## \#93 Posted by: Gamer43 Posted at: 2018-11-25T07:21:58.487Z Reads: 132

```
[quote="Petertaylor, post:92, topic:30928"]
> If I tried switching frequencies above 35khz, there was a faint high pitched whine coming from the motors.

35khz is above human hearing, what whine would you be hearing? Where would it be coming from? What frequency sound?
*Edit: Perhaps harmonics at the resonant frequencies of various mechanical stuff in the motor would be within the audible range. RPM would shift this into/out of the resonant range though, so it’d only be audible at certain frequencies.*
[/quote]

It was a sub-harmonic in range of 15-20khz, very faint and high pitched, very similar to the whine you would hear from a grid-tie inverter.

[quote="Petertaylor, post:92, topic:30928"]
> changing the switching frequency in field oriented control for those motors often has little effect unless you go below 15khz or above 40khz (in which case the effect is negative).

i’ve got a 6% system loss at peak efficiency from two different motors (same controller) going from 20khz to 18khz and 19khz. That’s not a “little effect”. The motors are similar form factor, same kv rating, different pole counts however.
[/quote]
Your motor was 100KV, which is reasonably low-speed for switching frequency to have an effect. I was talking about motors that have KVs in range of 200 or even higher. Also, I have a sneaking suspicion that the measured lower efficiency is firmware related, either in inaccuracies in the values reported or something else.
The reason why I believe the cause is firmware bugs is because if you run fast decay in BLDC mode, the VESC says that motor draws significantly more no-load current compared to slow decay; HOWEVER, I built my own motor controller from scratch, tested both slow decay and fast decay, I got exactly the same current draw at the same speed (measured current draw using a bench supply).
```

---
## \#94 Posted by: 12meterkuk Posted at: 2018-11-25T09:11:14.895Z Reads: 124

```
What would you consider as a bigger motor?

I’m trying to eliminate all unnecessary heat from my build as much as I can so I am able to shred as hard as I can without getting throttled or damaging any components. 

Does the switching frequency actually make a big difference in motor sizes such as 6374 and at around 200kv? 

Also my focboxes would not have any airflow so keeping it cool is a priority too.
```

---
## \#95 Posted by: Pedrodemio Posted at: 2018-11-25T11:47:14.292Z Reads: 122

```
It’s definitely a 2nd order sub harmonic at 15 kHz when running at 30 kHz

@12meterkuk should be, try it and see, maybe some motors dampen the harmonics better, on small 5055 motors

The efficiency part is exactly what we are trying to find, for now we don’t know if the measurements taken by the vesc taken at anything other than 20 kHz are valid
```

---
## \#96 Posted by: 12meterkuk Posted at: 2018-11-25T11:51:51.172Z Reads: 126

```
Less efficiency means more heat right? I’d say run the motor on a dyno at a constant currant for a bit and see how hot it gets both motor and vesc after a set amount of time using different frequency 

Problem is I already disassembled my makeshift dyno ☹️
```

---
## \#97 Posted by: 12meterkuk Posted at: 2018-11-25T11:54:14.188Z Reads: 128

```
Would be better if someone knows how switching frequency actually affects different motors (kv, resistance, size, inductance, etc) so Don’t have to spend so much time diagnosing each frequency
```

---
## \#98 Posted by: Petertaylor Posted at: 2018-11-26T04:22:31.819Z Reads: 119

```
Ok, ok, ok!
I'm almost done integrating real voltage and current sensing into the system. I'm keeping the vesc data too, so two plots can be done one top of each other, comparing the measurements. Got a little more code to go, but gotta take a break, get groceries, and that kinda real-world interference :-) Initial results show my current sensor swinging around a bit more, but i have a filter cap getting it down to 1khz bandwidth now. Only really taking measurements at 10hz though, so a little more filtering is likely in order. Maybe i'll plot what i get after the 10 sample averaging and see what's up before changing the cap.
```

---
## \#99 Posted by: Deodand Posted at: 2018-11-26T04:29:53.587Z Reads: 119

```
Nice work man, excited to see the comparison. Will be awesome to have a better idea how accurate the vesc measurements are.
```

---
## \#100 Posted by: Petertaylor Posted at: 2018-11-26T05:58:25.762Z Reads: 120

```
Yep, thought it's likely a toss up as to which is more accurate/true. They'll both be off to some extent. It may just confuse matters. I really hope not though. I kinda expect to see the measured numbers stay roughly where they are for 20khz across other switching frequencies, indicating something assumed in the firmware that shouldn't be assumed. 
Time will tell. 

Also, another upshot of making the driven motor esc agnostic (which it will be after this if i write power limit control code for PPM control) is that other controllers can be tested with the same motors. Comparing hobby escs will be interesting. Maybe i'll grab an o-drive as well and see how that stacks up? It's designed for a different application, but i'd be interesting to know.
```

---
## \#101 Posted by: Petertaylor Posted at: 2018-12-02T07:54:01.503Z Reads: 124

```
Well, dyno now has external current, voltage and rpm measurement. Current measurement is calculated using the formula on Pololu's website, but reads ~10% higher than vesc's current measurement. I could fudge the measured reading to line up with the vesc readings. Not sure which is correct, however. Each run is capturing data from both sources simultaneously. I did add a filter cap to bring the current sensor's bandwidth down to smooth spikes.

Ignoring the offset for now, the dotted lines are the externally measured voltage and current, and the solid the ones calculated from vesc's internal voltage and current. There is also an external RPM sensor, but that tracks very cleanly to the vesc rpm. Both use the same load cell reading for torque, of course. 

Somewhat amazingly, the 20khz setting was unstable for the tested motor. It hunted quite a bit. Redetection helped that out, but made it an apples to oranges comparison to the other plots, perhaps. 

Not really conclusive yet. Thoughts?
I'll do more testing soon (gonna annoy the neighbours if i continue tonight). 
Just wanted to share what i'd got today. More data should make it more clear what's going on. Will try other motors too, of course. 

![inconclusive|690x338](upload://wbA5vdYca0CfbsBoTpJlOnR4SpE.jpeg)
```

---
## \#102 Posted by: Deodand Posted at: 2018-12-02T19:29:46.046Z Reads: 118

```
Very interesting, the VESC back calculates current pull from battery based off of motor amps so I suppose it doesn't account for the draw of all the passive stuff (something like 0.1 amp) what current ranges are you operating in? Regarding your filter cap, did you add a RC passive filter? In theory this would only lower the analog value which wouldn't make sense why the current pull was actually higher.  The data seems pretty noisy to make any real conclusions off of.
```

---
## \#103 Posted by: Hummie Posted at: 2018-12-02T19:42:03.068Z Reads: 115

```
With the Vesc tool doing no-load testing I’ll get slight increases in current drawn going faster until I hit 95% duty cycle and then it will drop and maybe even half an amp lower.  Why? Are esc losses included?
```

---
## \#104 Posted by: Petertaylor Posted at: 2018-12-02T20:24:42.839Z Reads: 122

```
There is a dedicated filter pad for the pololu current meter. https://www.pololu.com/product/2199
I'm using the chart from the datasheet to get 0.1khz (1000nF cap) bandwidth. I'm sure they didn't create a pin on the IC for this if it'd modify the reading accuracy. 

The 0.1khz is still 10x higher than i'm actually sampling at, which means some artifacts from fast changing current could get through. I guess i'll add some buffering and averaging in the arduino code to get 10x samples per sample from the pc to arduino, which itself is already doing 10 samples per point on the graph. This may or may solve it, but i don't think it could hurt. Wanted to keep all the smarts in the computer and have the arduino just be a dumb data collector (no math, constants or conversions).

I just added a watt meter i had laying around to the setup, so there is an LCD display giving voltage and current. I'm seeing 40mA to 60mA for the vesc and the current sensor with voltage divider. Not accurate at this low level i'd imagine, but it's something. There current difference i'm seeing is upto a couple amps, so it's not the quiescent current. Current range is 15a (at 30v = 450 watts). 
With this _third_ measurement device i'm hoping to get a  consensus. Which is wrong? Vesc or pololu current sensor? Likely i'll get a third opinion, because of course i will.

Stay tuned.
```

---
## \#105 Posted by: Petertaylor Posted at: 2018-12-02T20:48:35.346Z Reads: 124

```
Initial reading from the external LCD current measurement show it and the pololu agreeing, leaving the vesc pretty far off :-/ All readings were pretty stable, bouncing a couple hundred mA or so. For this sample measurement 50% duty chosen on the test motor, 15a of braking on the brake motor. 

I'm manually doing the same math the script does (since it's kinda buried in there). Depending on what i choose as the current reading from the arduino (559 or 558) the value is pretty close. Serial monitor in background to show readings from the arduino, "c=xxx" is the current part. 
![pololu_current|625x500](upload://6O3Wh6eNhSlir1K4O62PfFSsKCK.png) 

Photo of the watt meter.
![IMG_20181202_123441|666x500](upload://iPM4vyBCOKI5lnAt9za6Bc3ZqC3.jpeg)

Photo of VESC-tool's current meter. 
![IMG_20181202_123434|666x500](upload://e2GpCogZpYWK8cRCxDowCp5NEVV.jpeg)
```

---
## \#106 Posted by: Petertaylor Posted at: 2018-12-02T20:58:11.613Z Reads: 118

```
Which also means the efficiencies i was seeing are way too high. The motors are in the 85% range, not the 92% range.
Another frowny face due here. Better to know than not though, of course. Means heat dissipation calculations/simulations i've done are also way off.
(Just for fun, since it's off topic, here's a CFD airflow simulation of airflow in a submerged pod in water. Motor assumed to create 50watts of waste heat (450watts input * 90% efficiency)
 ![heat_flow__submerged_pod|689x378](upload://9FsrFBP9NFBKuO1pHWEiMYLDkGZ.png)
```

---
## \#107 Posted by: Petertaylor Posted at: 2018-12-03T00:00:39.521Z Reads: 120

```
Ps, thanks everyone for the support on my progress on this project. I'm hoping the data helps the VESC community, but it's also a selfish desire to improve my own knowledge. Apologies for anyone angry that i seem to have highjacked this thread. I only wanted to share those initial findings, but the conversation lead me/us toward more questions that mattered, and lead to improvements in the techniques and data collected. 

Anyhow,
Ran outta battery juice, recharging. So far the new data looks like this. This is only the externally measured data, which seems to be smoother now than the vesc reported data. The arduino is doing 10 point moving average of the measured voltage and current. Python script averaging over 10 samples too. I'm also using a median average, rather than a mean, so it's much more spike/error tolerant, which are visible in the mean averaged data.

![beginning_foc_switching|690x349](upload://4MFM4WF4yXhFUyKVRhvjwuYvEbi.jpeg) 

Interestingly, on this motor, with only a few runs done, it seems like 15khz isn't any worse than 20khz. 25khz is pretty bad though. Not only is it less efficient, the curve shape is different, and peak efficiency for that curve is at a much lower rpm. 22khz might be slightly better, but it's not clear with so few runs. Getting interesting...

As always, more data required, and i've got shit to do in the real world, so it'll be at least a couple days until i can work on this some more.
```

---
## \#108 Posted by: Hummie Posted at: 2018-12-03T00:07:40.073Z Reads: 115

```
Are u solely getting data on motor eff or also the esc included?
```

---
## \#109 Posted by: Petertaylor Posted at: 2018-12-03T00:11:16.466Z Reads: 114

```
It's system wide. It's the motor and controller together. There are a couple bearings in the system too, so each of those is robbing a little power in heat. Three bearings in the dyno plus the two in the brake motor (though the motor ones do contribute a little in the torque reading). 

Mechanical power out / Electrical power into esc
```

---
## \#110 Posted by: Hummie Posted at: 2018-12-03T00:32:18.980Z Reads: 117

```
Is the Vesc data logging including the esc losses?  I’ll get a drop in no load current when I get to 95% duty
```

---
## \#111 Posted by: Petertaylor Posted at: 2018-12-03T00:37:43.630Z Reads: 118

```
In theory, the only thing the VESC isn't measuring is it's own power draw, i think, which is minimal. I'm seeing that the VESC's current measurement from the battery leave a lot to be desired, so take any measurements you do via the ESC with a pinch of scepticism. Maybe put a meter in the circuit for no-load current, it'll only be an amp or two. Can compare results that way.
```

---
## \#112 Posted by: Pedrodemio Posted at: 2018-12-03T00:40:14.579Z Reads: 117

```
Interesting, if your data is good, it’s seens to be motor dependent to a really high degree, really want to finish my board to try this in real life
```

---
## \#113 Posted by: Hummie Posted at: 2018-12-03T00:41:28.058Z Reads: 117

```
I thought 100% duty would be more eff w no switching (if 100% duty even possible) but 95%?
```

---
## \#114 Posted by: Pedrodemio Posted at: 2018-12-03T11:09:21.113Z Reads: 124

```
VESC tops out a 95% duty
```

---
## \#115 Posted by: Hummie Posted at: 2018-12-03T12:54:10.374Z Reads: 122

```
I know on the Vesc 95% is max duty cycle but why the current draw is about half an amp less at that.  Is it because at 95 it’s ON consistently throughout the commutation and no pwm?  I’m guessing that’s why
```

---
## \#116 Posted by: Jc06505n Posted at: 2018-12-03T15:54:29.186Z Reads: 124

```
Me trying to understand everything that’s being said in this thread : 

![image|220x124](upload://bnClmS7lYhOKsqcTz8BDCIlJHqG.gif)
```

---
## \#117 Posted by: Petertaylor Posted at: 2018-12-09T23:12:52.393Z Reads: 124

```
https://youtu.be/fbK2dcoYS7g

Looks like vedder is doing similar testing on his new VESC.
```

---
## \#118 Posted by: nickw1881 Posted at: 2018-12-12T19:14:25.858Z Reads: 119

```
The VESC adc sampling is tied to the switching frequency, so as you drop switching frequency (increases efficiency) you also drop sensor resolution, which can introduce control errors.
```

---
## \#119 Posted by: mmaner Posted at: 2018-12-12T19:24:38.769Z Reads: 121

```
[quote="nickw1881, post:118, topic:30928, full:true"]
The VESC adc sampling is tied to the switching frequency, so as you drop switching frequency (increases efficiency) you also drop sensor resolution, which can introduce control errors.
[/quote]

We are talking about dropping the freq on sensorless motors.
```

---
## \#120 Posted by: trampa Posted at: 2018-12-13T20:04:37.785Z Reads: 122

```
This is a very special motor, putting max strain onto the ESC. 70kHz switching!  We use 20kHz for our motors. 
This turbine is the worst case scenario. The 75/300 is probably the only controller in the world being able to run it in FOC at full power. Good news: A lot of the 75/300 tech will be part of the next generation VESC SIX design. Be surprised!
```

---
## \#121 Posted by: Petertaylor Posted at: 2018-12-15T18:10:41.366Z Reads: 117

```
Yeah, this is the kind of thing that makes sense for what i'm seeing. 
I'm going to do some more testing today/tomorrow and see what i can see. I got another current sensor, so i'll hook that up to one phase wire of the motor and see if there is anything interesting going on. Think i'll build a variable capacitor filter board too, to try to smooth the current spikes into something more easily visualized.
```

---
## \#122 Posted by: Petertaylor Posted at: 2018-12-15T18:18:33.999Z Reads: 119

```
"sensor resolution" he's referring to is current sensing per phase as it relates to controlling the sensorless electrical commutation and control. He's correct in that if the ADC measuring current is tied to switching frequency, we might get some odd results, particularly if it isn't measuring at a consistent/representative time in the current pulse.
```

---
## \#123 Posted by: Petertaylor Posted at: 2018-12-15T18:28:46.901Z Reads: 120

```
Right, we did actually watch the video i posted. Vedder said, measured and demonstrated that this is an unusually low inductance motor. Just because you use 20khz for your motors doesn't mean it's ideal for each one of your motors (or any of mine), and/or doesn't mean there isn't a firmware bug that's forcing 20khz to be "best" by hobbling the other frequencies. Testing will continue on my end until it's clear if there is a bug, an error in my setup/procedure, or that the seeming 20khz preference is refuted by new data. Nothing absolutely conclusive on my end yet, just stuff that seems to indicate something strange. 

It is good news that a new vesc 6(vesc 7?) will have some trickle down tech from the 75/300.
```

---
## \#124 Posted by: Petertaylor Posted at: 2018-12-15T21:33:24.052Z Reads: 122

```
These tests are with a pololu current sensor rated to 120khz, so they should be capturing good data. The sensor centers on 2.5v for 0amps, so consider that the baseline. The graphs are a 3khz low pass filter to smooth the current pulses into an average of the "sine-wave" that the FOC controller is hypothetically delivering to the motor. 

It sure looks like the 25khz test results in each commutation phase being more similar to the others (though this could be to do with the increase inductive impedance from faster switching, right?). Remembering that this is only one phase of three, i see much greater similarity one every third cycle. I also see a slight lowering of amplitude as the switching frequency increases. Inductive impedance in the motor preventing these shorter pulses from reaching full voltage/current? 

The change in jaggedness clearly shows the effect of the increased switching frequency. 

This is with 4.12 hardware, on a flipsky 6374 190kv motor. It's running sensorless at 30% duty cycle with 30w of total energy consumption.

15khz
![15khz-30duty-190kv|660x500](upload://obVInGG9bCRdbCC2A1oG5v6W9jf.png)  

20khz
![20khz-30duty-190kv|660x500](upload://jzgZqLc990MyFIExHIaZS3yIEyj.png) 

25khz
![25khz-30duty-190kv|661x500](upload://yyuNDmRPTOqoIhTRWQWGi0MoeJ0.png)

Thoughts, anyone?
```

---
## \#125 Posted by: Petertaylor Posted at: 2018-12-15T22:08:00.826Z Reads: 111

```
30khz
![30khz-30duty-190kv|661x500](upload://7uwL65yXydKM00is0DvMoQG79a4.png) 

zoomed out in the time domain a bit to make sure we see two of each cycle, otherwise same settings as above. (Gearbox that was acting as a load was cooler, so the amplitude won't be comparable to the others, since the grease is high viscosity at lower temps.)
```

---
## \#126 Posted by: Hummie Posted at: 2018-12-16T16:28:57.433Z Reads: 107

```
The higher frequency seems to produce a cleaner wave with the one primary frequency, so do I guess right in that it will be more efficient in the motor and maybe less efficient in the esc at 30k?  But even within the samples there’s a lot of variation of then waveform which I’d have thought they’d stay the same.   I have a weird motor I’d like to see how it shows if you’re open to others.
```

---
## \#127 Posted by: nickw1881 Posted at: 2018-12-18T07:31:29.641Z Reads: 103

```
You shouldn't need a low pass to filter the current pulses, the motor inductance does that automatically. The 3khz is adding distortion by taking the energy from any fast spikes and smearing it all over the real signal, and also delaying the signal. If the signal is noisy, power the polulu from a battery and make sure scope ground and polulu ground are right at the vesc -input, like right on the board. Shorter scope grouns are better.

Does your scope have multiple channels? Could you capture phase voltage and phase current at the same time? What does the vesc +input look like with ac coupling and 500mV/div?
```

---
## \#128 Posted by: Petertaylor Posted at: 2018-12-18T22:01:25.837Z Reads: 112

```
Without the lowpass, the individual current spikes were visible, and the trend was hard to see. Perhaps not enough motor inductance to smooth the spikes into a sine? If so, this might be an indicator that all else being equal (it isn't), a switching frequency just high enough to smooth the wave via motor inductance is optimal? 
3khz seemed about right to smooth the pulses into a sine wave. It's not what the motor sees, but it is a lot easier to see and think about. I can post without filter to show you. 

I've got two scopes now, a 4 channel rigol, and the 2 channel AD2. After i posted these, i did hook voltage up to the second channel of the AD2. I also applied (just by hand) more load, and the spikes in this filtered waveform did get much cleaner sine shaped. 

My flipsky 6.6 is acting up (no USB detect anymore), so i can't run a motor-vs-motor dyno test to look at waveforms under higher torque loads right now. I'll probably modify my program to send PPM test motor signals rather than VESC UART to make the dyno more universal. I do have other controllers i'd like to test. After finals week though, which is this week.
```

---
## \#129 Posted by: Petertaylor Posted at: 2018-12-25T03:40:28.618Z Reads: 111

```
Ok, finally gotten around to making the latest batch of changes. This graph is sorta tangentially related to the VESC.

Testing procedure changed just a little. Now the power limiting (that i need to simulate my power limited situation) is external to the VESC. The code is now lowering commanded duty cycle when the power exceeds the setpoint. The dyno is now agnostic to the tested esc and motor, but still uses a vesc as the adjustable regenerative brake.

![vdyno_esc_agnostic|690x346](upload://knVOf39n6hlhueOx4PIxOzeIkOM.jpeg) 

Anyhow, the results from three green runs (where i don't have any options to play with, so they're all the same) show them ahead of the vesc by ~4%. Also this other esc runs at a switching frequency of 30khz (apparently, maybe i'll put a scope on it to see if it's real). This seems to further demonstrate there there is something problematic with the VESC's switching frequency algorithm, if this esc really is running at 30khz. 

All data was collected externally to the VESC, so the inaccurate current sensing in the vesc isn't a cause of the discrepancy.
```

---
## \#130 Posted by: Pedrodemio Posted at: 2018-12-25T04:33:39.023Z Reads: 107

```
All energy measurements are using external sensing?

Now that my board is working I will see if I can do the real life tests before the new year

What frequency’s should I test? Was thinking is just 20 and 30 KHz, and if I have patience do a full discharge test for both and see how far can I go, this way we eliminate errors in the vesc energy measurements
```

---
## \#131 Posted by: Petertaylor Posted at: 2018-12-25T05:37:00.584Z Reads: 109

```
Yep, all energy sensing external. I'm measuring voltage and current into the esc, rpm, and force. All external sensors, and the conversion constants don't change between runs. 

![IMG_20181224_185818|666x500](upload://7Xuk2YfGxJGi48IjVkuwRxYPRLk.jpeg) 
It's a nutty rig, honestly.
```

---
## \#132 Posted by: Hummie Posted at: 2018-12-25T06:05:21.642Z Reads: 107

```
what esc is the green?  And the brown, blue and red are the Vesc I guess.  But such low efficiency shown on the side of the graph it seems unbelievable.  Peak efficiency for the Vesc at 80%.   Maybe there’s some other Vesc variable that u could adjust for better results like boost or timing or something. Maybe ur particular Vesc is the issue. What version and model is it.  I’ve heard ones with three shunts are more efficient 

Agnostic?
```

---
## \#133 Posted by: Petertaylor Posted at: 2018-12-25T07:07:07.148Z Reads: 112

```
Agnostic?

meaning before it needed a vesc to control the duty cycle, report rpm, current and voltage. That meant i couldn't compare escs to each other. 

Green dots are the Hobbywing hv foc esc. 
All others are vesc at different frequencies. Same rig, same mounting, same sensors, same calibration. These were all with a flipsky vesc 6.6 with three shunts.

It's a little surprising to me too. The hobbywing esc is actually "designed" to go with that motor, so that's one thing. I'm sure i could have fiddled with every button in VESCTOOL and run the tests again. Not sure if i'd have found anything different in the data. What options other than switching frequency would affect performance? I expected the VESC to be significantly better, just because of how many people are using it, and how the source is open so bugs might get caught. 

My flipsky 6.6 is fucked, and i've finally convinced them to take it back to look at. USB on the fritz from day one, and now it just won't detect at all. Wish me luck with that. That means that until i can get another vesc, it'll be hard to test any other motors on the vesc. I've got another one coming (one of the crazy cheap 50a 4.12 hardware based ones). 
The one going back is the only one i own with three shunts. 

Any rich folks wanna ship me a nice vesc six to test with? Or even better some vesc spinoff custom hardware? ESCape?
:slight_smile:
```

---
## \#134 Posted by: Petertaylor Posted at: 2018-12-25T07:12:08.986Z Reads: 107

```
Pedro, i'm worried your data won't be very conclusive, unless the road conditions and your application of throttle is just identical. However, if you wanted to try something, i'd go for 10khz, 20khz, 30khz. You might not even get any motor stability at the 10khz frequency, but if you can, run it and see!

Another thought is that you might be able to reduce battery factors somewhat by logging the power used over time "Wh Draw" in vesc tool. That way you know how much power total got used, and how far you went on that much power. It'll also factor in voltage sag, though the motor won't necessarily behave the same when voltage sags.
```

---
## \#135 Posted by: Pedrodemio Posted at: 2018-12-25T13:07:40.142Z Reads: 105

```
Yeah, I will keep the road the same and only do it with no wind, the route I use to test I can keep full throttle all the time apart from turning back, should be consistent enough
```

---
## \#136 Posted by: Hummie Posted at: 2018-12-25T15:49:14.056Z Reads: 104

```
I have a couple different escs u could try.   4.12 w updated hardware and you could use a flipsky six I have.  Have some focboxes that one might work and two coming in the mail 

I don’t know the variable you can adjust but have heard the timing is one.  I don’t know where that is though.  Have you posted this in the old or new vedder forum?  Bet you’d get a lot of info there
```

---
## \#137 Posted by: Hummie Posted at: 2018-12-25T15:53:17.481Z Reads: 100

```
If ur going full throttle and at top speed wouldn’t that amount to the full battery voltage directly being put to the motor as there’d be no pwm needed to reduce voltage and the back voltage would need to be overcome? If you set an erpm limit then went full throttle it would be reducing the speed and therefore need Pwm, no?
```

---
## \#138 Posted by: Pedrodemio Posted at: 2018-12-25T16:45:10.971Z Reads: 102

```
Sorry, forgot to say that, full throttle but erpm limited so the speed is constant across all battery voltage
```

---
## \#139 Posted by: Petertaylor Posted at: 2018-12-25T19:40:30.749Z Reads: 110

```
Hummie,
I'm not sure where the old/new forums are. I added some detail to the thread over here https://vesc-project.com/comment/2821#comment-2821

I also realised that there are a couple gaps to think about.

1. The above graph isn't quite apples to apples, since the vesc tests were with internal vesc power limiting, and the hobbywing tests were with external limiting. Since the internal limits are based on shoddy current measurements, they could be off and change the power range i'm examining, and thus the results could be offset. Need another vesc to see how true that is.

2. Max efficiency on my curves are power limited to 450w. If the motor/esc max efficiency peaks at 800w, then i'll never see that in my graphs. It's unimportant for my testing, since my application will never see 800w, and only ever 200-450w. However, the numbers might be hampered slightly by this, and absolute max efficiency is likely higher that ~80%. 

3. I haven't been keeping track of whether motors are tested CW or CCW (_edit: though the tests in the graph above were definitely the same direction, previously in this thread i'm not sure about_). I don't understand _why_ but i know that many motor manufacturers that do provide power/efficiency curves will have curves for both directions, and i've seen differences upto around 5% with only the spin direction changed. I'll need to move back to a push/pull load cell to make that happen. I'll also need a good way to make sure the push and pull are calibrated the same, which i can't think of yet.

Lastly, i'd love to borrow an ESC to keep the testing going. Whatever vesc you wanna lend me, i'd be happy to test with. What is the custom hardware 4.12 you mentioned? What's different about it? I'd be interested to try a focbox too. Those are modified 4.12 hardware, right? Hit me up via email and we'll sort out something.
```

---
## \#140 Posted by: Gamer43 Posted at: 2018-12-27T06:13:12.574Z Reads: 109

```
EDIT: Nevermind, the motor sees an effective frequency of twice the pwm frequency, so the main point of this post is irrelevant.

@Petertaylor 
Hey guys, not sure how helpful this is, but I just took a quick look at the VESC firmware and saw this
![CenterAligned|690x251](upload://lSpUAZo14L6yypH193vXYRRMCiF.png) 

Now, if I understand STM32's advanced control timers correctly, in center aligned mode, the actual PWM frequency is Input Clock / (Period x 2).
I discovered this when I read debug information from the VESC terminal, it said TIM1 and TIM8 TOP was ~6000, which did not sound right at all for center-aligned PWM. 
Looks like the actual switching frequency is HALF of what it is when set in VESC tool. 
(This would explain the high pitched ringing on my Hoverboard Motors at "35khz and up", because it was actually 17.5khz). 
This also explains why "30khz" doesn't give you DRV GVDD undervoltage faults galore. 

Theoretically, on 4.12 hardware, using typical gate charge values, any real switching frequency above 22khz would overload the GVDD charge pump. 

This is how sampling is determined:
Timer 8 is synchronized to Timer 1, and set in up-counting mode.
Capture compare channel 1 triggers ADC conversion sequence. 
Compare value is set to some small value (looks like 2 from what I can see), so that the start of conversion occurs close to (but not exactly, very shortly after) Timer 1 underflow and overflow (center of low and high pulse).
One sample will occur when all phases are low, the other when all phases are high. If you don't have phase shunts, the second sample (when all phases are high) is thrown out. 

The way PWM is updated, the applied PWM lags behind by half a PWM period, not sure what kind of effect this has on the FOC algorithm as a whole.
One way to get around this is to estimate the current at the next timer update event by extrapolation and use those values for your SMO and current control loops. 

TL:DR  There might be (or very likely? if I am looking at this code correctly) a firmware bug making the real switching frequency be half of the switching frequency specified in VESC tool. 

Current control loop lags behind by one PWM cycle and does not compensate accordingly.
```

---
## \#141 Posted by: Hummie Posted at: 2018-12-27T06:32:29.812Z Reads: 100

```
The large majority of us don’t have the background in this stuff but if u were to go way back to the basics and walk us through i for one would appreciate, especially with what it seems you’re saying. Is there better programming possible for the Vesc?
```

---
## \#142 Posted by: Gamer43 Posted at: 2018-12-27T06:40:11.078Z Reads: 108

```
EDIT: first part of this post is irrelevant.
@Hummie
Basically, I know this is hard to believe, but I think Vedder left out a "divide by 2" in the code that is making the switching frequency half of what it should be. (This is just a guess, I could be very wrong).

Microcontrollers use this hardware unit called a "timer" that basically takes in a clock and counts up, or counts down. "Center-Aligned Mode" means the the timer counts up then counts down and repeats. 
PWM is generated by changing the output state when the timer hits a certain value. 
The "Period" value is what the timer counts up to and counts down from. Let us use 500 as an example. So, in "Center-Aligned Mode", the timer will start at 0, count up until it reaches 500, then count down until it reaches 0 again, generating one PWM cycle along the way. 
This means the timer needs 500 counts to reach the top, and 500 counts to reach the bottom, resulting in a total of 1000 counts for one cycle. 
Let's say we give the timer a clock of 100khz. This means the timer will count 100,000 times in one second. Since it takes our timer 1,000 counts to complete one cycle, this means the timer (and resulting PWM) frequency is 100,000 divided by 1,000, which in this case is 100. 
What this means is it takes the timer two times the period value to complete one cycle. 
In the code, the period value was determined assuming the timer only requires one times the period value to complete one cycle.
The result is your PWM frequency is half of what you expect it to be.

EDIT: everything below here might still be irrelevant?

The part where I was rambling about sample timing, that isn't an issue, just a resource inefficiency that I am anal-retentive about. That can be optimized by using Timer 8 instead of Timer 1 to generate the PWMs (but this change is not possible on most hardware), or use a different microcontroller and modify the code accordingly; STM32F446RE and STM32L452RE are two possible candidates.
Using a different microcontroller would reduce the cost of the VESC, in fact, using the latter wouldn't even need a crystal oscillator, further reducing cost.
Vedder used the STM32F405RG because there was a discovery board for it, making prototyping and developing easy, and the two microcontrollers I mentioned were not available when he developed the first iteration of the VESC. Porting the code will be an arduous task as Vedder wrote the code to be highly efficient, making it difficult to port (this is a tradeoff common to all embedded software). One possibility is to try to wrap his FOC algorithm and USB communication scheme into a library and develop a new application.

The second part is a little hard to explain. Imagine you are trying to get your house to a certain temperature by using your air conditioner and heater. But what is happening here is it takes 30 minutes to either turn on or turn off the air conditioner or heater. You can get around this issue by trying to guess what temperature your house will be in 30 minutes.

@Petertaylor
Oh, what did you set the dead-time compensation to be? In firmware, the actual dead-time is 60 timer counts, at 168Mhz, this comes out to be ~360nS (or 0.36uS), and incorrect values for dead-time compensation will only become exacerbated by higher switching frequencies.  The default in VESC tool is 0.06uS.
```

---
## \#143 Posted by: Deodand Posted at: 2018-12-27T16:58:10.691Z Reads: 97

```
Your analysis is somewhat correct but flawed. The whole point of using center aligned pwm mode is it effectively doubles the pwm switching frequency for a given pwm period. Honestly a bit too lazy too draw up all the diagrams etc but if you look at how center-aligned three phase switching works for a 10kHz switching period you get an effective 20 kHz resonance. Trust me if your motor was switching at a lower frequency it would be intolerably loud. The whining you hear is lower harmonics, since the system has some nonlinearities smaller amplitude lower harmonics present themselves as 1/2 and 1/4 the switching frequency, and the amplitude of these just depends on system Dynamics.
```

---
## \#144 Posted by: Gamer43 Posted at: 2018-12-27T17:44:12.126Z Reads: 97

```
I thought the purpose of center-aligned pwm is to generate a symmetric pwm signal to reduce higher order harmonics. Every reference manual I have read tells me Center-aligned mode generates a pwm signal of half the frequency of the equivalent edge-aligned signal with the same period value. So you're saying the LR filter that makes up the phase windings actually sees a signal twice that of the actual pwm signal frequency?
```

---
## \#145 Posted by: Deodand Posted at: 2018-12-27T17:47:14.087Z Reads: 102

```
Yeah the frequency gets set to 10 kHz for instance and the windings LR sees 20 kHz. I've also seen this topic brought up with vedder before and he had the same response.
```

---
## \#146 Posted by: taz Posted at: 2018-12-27T17:50:27.705Z Reads: 106

```
![08|690x388](upload://u4xwMYKZdNyi40X7h0OTnzrkAHG.png) ![30|690x388](upload://6N2zTTFFLOrYrqEZeV41dVrpzpA.png)
```

---
## \#147 Posted by: Gamer43 Posted at: 2018-12-27T17:56:52.732Z Reads: 103

```
Oh hmm, no wonder why transistor switching losses aren't as bad as I thought they would be. I wonder if the whining would persist if I tried a switching frequency of 40khz or higher (20khz pwm).
What could be causing the discrepancy petertaylor is seeing?
Some things I noticed is that the VESC sometimes has issues transitioning from sensored to sensorless, and the observer has some problems locking on at low speeds.

EDIT: I took another look at the firmware, I think that the code does not compensate the fact that the updated duty cycles do not take effect until the next update event (update events occur at twice the PWM frequency). I am not exactly sure what effect this has on the current control loop and observer, but I do know that if this is indeed the case, the current control loop will run half a PWM cycle behind the actual measured current, and the applied Valpha and Vbeta vectors used in the observer are slightly off. 

The fix for this is current extrapolation, but the trade-off is that the observer will run at one quarter the switching frequency (or one half the switching frequency if phase shunts are used). 
You can get around this by doubling the PWM frequency and using MOSFETs that aren't from International Rectifier, i.e have decent gate charge characteristics. International Rectifier MOSFETs are reliable and rugged (because the transistor die is HUGE), but aside from Rdson and avalanche energy, have relatively poor electrical characteristics compared to similar MOSFETs on the market (again, because the die is absolutely huge).
```

---
## \#148 Posted by: Petertaylor Posted at: 2018-12-30T05:23:32.287Z Reads: 97

```
Hi Gamer43! 
Thanks for the info, and looking seriously at the code. It's perhaps a little over my head, or at least desire :slight_smile:

Looks like you're retracted some of the prior statements. Anyhow, i really appreciate the look at the code, and thoughts. Can you keep checking back on this thread as more info shows up?

I had defaults settings as far as i could, so i presume the graphs above were done with the default (which i see as 0.080 µS, not 0.06uS). For optimum efficiency, do you recommend 0.36uS?

In other news, i realised that the sensor voltage i was using has drifted slightly, and i' should really be using a dedicated reference voltage, or ADC with one incorporated. That change will happen soon/tomorrow. It's only a percent or two, but still annoying. 

I've got a couple other motors on the dyno now, so can do some testing in a different range of motor kvs, pole counts, resistance, etc. I also got another vesc (4.12 hardware) to play with. New motors are Flipsky 6374 190kv and turnigy 6364 213kv.
```

---
## \#149 Posted by: Gamer43 Posted at: 2018-12-30T08:40:50.988Z Reads: 99

```
In the firmware, in file "mc_interface.h" , there is a #define called "HW_DEAD_TIME_VALUE" and it is defined with a value of 60.

If my math is right, at 168mhz the frequency of Timer 1, 60 counts comes out to be ~357.14 nS, which I rounded to 0.36uS. 
To get the most accurate value, use 0.357uS. The STM32F405RG only supports single precision floating points so more precise values will simply be truncated when dead-time compensation is applied.

I don't think it'll have too much of an effect, though. Improper (or the lack thereof) dead-time compensation causes minor hiccups with the observer, especially when phase current crosses zero. Detailed description can be found in this application note: https://www.nxp.com/docs/en/application-note/AN4863.pdf

Basically the rotor angle calculated by the observer would be slightly off, and may jump around when phase current crosses zero, this can introduce inefficiencies, but really is only problematic at low speeds in sensorless operation and high switching frequencies. (Or when you are using 8-in delta wound hub motors that have really high magnetizing currents, the observer utterly could not lock on until 3500 ERPM). 

Although I really would like to verify whether the VESC compensates for the fact that the applied phase voltages do not take effect until the next timer update event. On low side shunt hardware, the real applied voltage will be the average of the previous and currently calculated values; on phase shunt hardware, the real applied voltage will actually be the previously calculated value. From what I could tell in the firmware (namely the observer_update and current_control functions), it did not appear to do this. Maybe there was something I missed and it does indeed perform this compensation. 
I feel that if the VESC firmware did not compensate, this would negatively affect dynamic performance of the FOC algorithm. 

I will check back on this thread regularly, I really appreciate all the work you've done to perform these experiments.
```

---
## \#150 Posted by: Gamer43 Posted at: 2018-12-31T21:57:24.677Z Reads: 97

```
Sorry for the double post, but I discovered something interesting/funny.

So I was messing around with really high switching frequencies on my FSESC 4.20.
running with a damaged TB 6374 motor,
It did 60khz just fine (this is 30khz pwm).

80khz bricked the MCU.

How did it brick it? The FOC algorithm does not run fast enough, LMAO. The adc ISR is not fast enough.
Since the 4.20 uses low-side shunts, this means the controllers and estimators cannot run at 40khz, and probably cannot run much faster above 30khz. 

This means phase shunt hardware can't run above 30-some khz switching. 
EDIT: It will work at 70khz switching, which is 35khz for the observer, thus 35khz is most likely the maximum switching frequency for phase shunt hardware.

Interestingly enough, a very high switching frequency makes faults happen less often on the FSESC 4.20

I also ran into this when I was messing with STM32F4 ADC throughput.
```

---
## \#151 Posted by: Deodand Posted at: 2018-12-31T23:46:35.279Z Reads: 96

```
Yeah, I've run into this before. Note that for phase shunt hardware if you disable "sample in v0 and v7" then you can run the same frequency as low side shunt hardware. Sorry if this is obvious to you but you can re-flash with an st-link to fix.

Can you elaborate on the adc throughput? I'm pretty sure theres a few options you can tune to increase sampling speed at the cost of a small amount ofaccuracy.
```

---
## \#152 Posted by: Gamer43 Posted at: 2019-01-01T00:10:09.275Z Reads: 99

```
That's what I did, had to dig out an old connector and hooked it up to my Nucleo-H743ZI board, at first I thought I busted the DRV8302, but then realized when USB would enumerate but then block.

Basically, what I was doing was on an STM32F446RE was I set a single adc to its max sample rate on one channel, and experimented with how many samples I needed the DMA to transfer before the adc_conv_complted callback.would overload and stall the CPU.

The answer is 7 xD.

At 1.5 msps, this means the amount of overhead on the adc_conv_complted ISR only allows for it to be called at ~214khz (lower for the STM32F405RG since it runs at 168mhz instead of 180mhz).

I was using the HAL library from STMicroelectronics, and oh boy is there a ton of overhead in the ISR callbacks. (lots of branches to select the correct callback and clearing the status registers).

This was right in-line with what I observed with my own BLDC controller algorithm (only trapezoidal control). 200khz was just about the highest I could push the sampling frequency without the entire algorithm becoming unstable (it could do up to 400khz, since I would blank the sample timer 50% of the time in delay commutation mode, but because I didn't handle my state variables properly, if the sample timer were to be enabled with the motor not spinning, the algorithm would brick itself).
```

---
## \#153 Posted by: Deodand Posted at: 2019-01-01T00:14:48.238Z Reads: 94

```
Very interesting, thanks for sharing. Yeah I was doing some testing on the unity to see how long between triggering the adc sampling and all 15 samples were put into memory. I remember it being a small percentage of the total time window of pwm period. I could definitely see running into problems around 200 kHz but such a switching frequency probably only would be needed for super low inductance motors.
```

---
## \#154 Posted by: Gamer43 Posted at: 2019-01-01T00:15:29.678Z Reads: 99

```
or extremely high speed motors, I was running one motor at 140k ERPM xD.
```

---
## \#155 Posted by: Deodand Posted at: 2019-01-01T00:21:43.535Z Reads: 101

```
We've tested the unity up to 135k erpm, works but definitely gets loud. It's like 2200 rev/s so at 15kHz update (30 kHz pwm low side shunts) you only get about 7 updates per revolution so its basically back to a trapezoid at those speeds.

Vedder's video shows 80 kHz pwm on his new 75/300 vesc, I've been wondering if he cut some of the bloat in the loop to achieve that. Any idea of the compiler gets rid if multiplies in #defines for instance? Haven't had a chance to test but if it doesn't theres a ton of waste clock cycles in conversion defines etc.
```

---
## \#156 Posted by: Gamer43 Posted at: 2019-01-01T01:01:02.085Z Reads: 100

```
Wow, that's really impressive.

Maybe he's using the STM32H743ZI instead? That beast runs at 400mhz, has a superscalar pipeline, and supports double precision floats; it is several times more powerful than the STM32F405RG for only about double the cost xD.

Preprocessor substitutes all #defines with the literal expression prior to compile time (THIS IS WHY PARENTHESIZING YOUR EXPRESSIONS IS SO IMPORTANT), so as long as compiler optimizations are enabled, shouldn't be losing clock cycles to #defines as any expressions that evaluate to a constant should be compiled as a single constant in the code.

For example, this:
#define MACRO 10 * 5 + 3

int val = MACRO * 6;

will appear as this to the compiler:

int val = 10 * 5 + 3 * 6;

Although when I was looking through the code, there were a few things I thought could be optimized, can't recall all of them off the top of my head. Some of those optimizations would be at the cost of portability (and maybe code safety?). 
One of them was when updating duty cycles, timer update event is disabled and then re-enabled afterwards.
That's at least two store instructions (so three clock cycles?), but cutting this out would mean that the algorithm operates under the assumption that observer and current updates can be calculated before the next update event. If only sampling on the low side, setting the repetition counter to 1 instead of 0 might be necessary.


The observer also calculates phase angle iteratively, a different observer algorithm that solves for BEMF and phase angle in one go could potentially cut down on clock cycles.
```

---
## \#157 Posted by: Deodand Posted at: 2019-01-01T02:31:56.094Z Reads: 93

```
I did some googling of my own on the whole #define thing, a lot of interesting reading out there on code optimization. I guess anywhere there is a float divide it wouldn't optimize unless you raised the optimization level (by default the makefile is at -O2, if you set it to -Ofast I guess it would do this) but I'm not sure if it would have adverse effects anywhere else. I'll give it a try tomorrow.

Yeah I'd need to do some profiling to determine where best to focus attention. The iterative observer looks reasonably cheap and runs at a fixed 6 iterations but obviously it all adds up. Going to do some testing on this sometime soon. 

That MCU looks pretty amazing, but I think a more expensive MCU is definitely the wrong direction for eskate motor controller, I guess maybe if you need insane ERPM for other applications.
```

---
## \#158 Posted by: Gamer43 Posted at: 2019-01-01T03:13:35.370Z Reads: 93

```
I heard Vedder was testing the 75/300 on a wind turbine, that would definitely warrant an overpowered MCU xD.
Or EV applications.
Or four independent FOC motors from one controller xD.

Honestly, I would've loved to see something like the H743ZI go into the Unity xD, but that's just my ridiculous opinion. 

Moving from O2 to Ofast optimization does a few things. First, the compiler will start sacrificing significant amounts of code size, doing things like unrolling entire loops, inlining functions, and using lookup tables. The F405RG has plenty of additional flash memory so no problem there. 
Second, debugging becomes extremely difficult as the compiler tries to generate an order of instructions the most independent from each other so as to mitigate stalls from pipeline hazards and pipeline refills from branch mispredicts. 
Third, it may introduce some bugs if variables were not declared as volatile or if certain caveats are not followed, since the compiler may end up optimizing something away that is critical, but because of the context it appears in, the compiler did not think so. 
Fourth, as you mentioned, things like floating point division optimization. Divide is REALLY expensive, taking up to 17(if i remember correctly) clocks on the ARM-Cortex M4, and causing data dependencies down the line to stall. One well known optimization for floating point division is to approximate the reciprocal (it might do this using a lookup table, actually, some architectures have an instruction for this) and multiply (takes one clock) by that instead. The approximation is slightly less accurate, but much faster.
Although I don't remember if the compiler will start sacrificing accuracy for speed at Ofast automatically and you may need to explicitly tell it to do so using a flag in the makefile or project settings.
```

---
## \#159 Posted by: Deodand Posted at: 2019-01-01T03:21:36.054Z Reads: 91

```
Thanks, really useful information. My background is all over the place so I kind of have to pick up things as I go. I think I will test out timing impacts of increasing optimization that way vs just using the fast math flag with GCC which is probably less risky. I'll report back soon, I'm expecting very little :slight_smile:
```

---
## \#160 Posted by: Gamer43 Posted at: 2019-01-01T03:49:59.835Z Reads: 104

```
Glad I could helpful. 
I appreciate the tests you are doing. :)

Also, I just remembered another caveat with floating point #defines and constants (at least with the toolchain I was using, Atollic Truestudio)

All floating point constants need to be suffixed with an -f I believe (or something else to indicate "TREAT AS SINGLE PRECISION", can't remember exactly, I do know explicitly casting to float will work as well) otherwise the compiler will treat them as doubles. Software implementation of doubles is costly in terms of code and in terms of speed. 

I remember from my own tests, the difference from O2 to Ofast on my BLDC algorithm was something like 23% CPU utilization to 21% CPU utilization. (This was at 200khz sampling with sample timer blanking and BEMF integration). About 10%, significant, but not too much, I think it got most of it from function inlining and lookup tables. 

Interesting design point, if you add filter capacitors to the phase voltage resistor dividers (RC time constant of ~183uS), you can get BLDC Integration mode to work out of the box with no tuning whatsoever (on a different algorithm, VESC algorithm does not support this).
Ramp up the motor in openloop or sensored mode until the BEMF signal exceeds a certain hysteresis or until a certain ERPM, let the motor freewheel and watch one phase. Integrate between two zero crossings and divide that total value by 16 (or 14.98 for sinusoidal BEMF) to get the integration limit. Lock onto rotor position at the next zero crossing using a lookup table. The motor should freewheel at most two electrical revolutions, so there shouldn't be too much of a problem with dynamic performance there. 
Added bonus, works the same regardless of whether you use slow decay or fast decay. 
You can also sample whenever you want and at whatever speed you want. E.g. pwm can be 25khz, sample at 157khz.
I got the idea for this on-the-fly detection scheme from Allegro Microsystems' A4960 and A4964 datasheets.
The one downside is the BEMF signal after the filter will lag behind by 6 degrees at higher speeds (according to LTSpice), but this can be compensated for using phase advance, also I couldn't see much lag when I probed with my oscilloscope (at no phase advance).
```

---
## \#161 Posted by: Gamer43 Posted at: 2019-02-02T07:56:19.498Z Reads: 100

```
@Deodand

Are you still working on improving MCU performance on the Unity? 
This may seem a little random, but are any engineers working on the Unity familiar with digital design/FPGAs?

I started reading into this stuff, and more and more sources are pointing towards using an FPGA instead of a MCU for FOC motor control applications, especially ones with more than one motor.

Many tool chains for FPGA development advertise that they already have SVM and FOC libraries for use.
I'm thinking, would it be possible to use an FPGA to run the FOC algorithm, and then just double it up (a.k.a. copy-paste) to control two motors? Since many FPGAs have built in CPU cores, it might be possible to port Vedder's USB/UART interface code and FOC detection code, and rewrite the emulated flash library so that it writes to the relevant memory addresses/registers used in the hardware FOC algorithm.

With an FPGA, a motor controller can probably get up to some really crazy switching frequencies without issue.
```

---
## \#162 Posted by: TowerCrisis Posted at: 2019-02-02T09:14:57.533Z Reads: 92

```
My limited experience with fpga's tell me this is possible, and the crazy high polling rates they have would definitely be a step in the right direction.

But I'm completely unsure of how much processing power these things have and how they scale. Pricing could be a significant hurdle.
```

---
## \#163 Posted by: Indiangummy Posted at: 2019-02-02T15:25:35.734Z Reads: 93

```
It's been done before and as far as I'm aware and it's under patent. I'm taking a class in vhdl desgin with fpga's this semester and my professor has done research realted to this field. I'l talk to him and see what he says. But like @TowerCrisis said I think cost is the biggest hurdle

 https://www.eenewseurope.com/news/field-oriented-motor-control-fpga-takes-resolver-inputs-0#
```

---
## \#164 Posted by: Petertaylor Posted at: 2019-02-02T19:27:16.121Z Reads: 93

```
I think you're onto something with the VESC FOC implementation being somewhat constrained by the MCU. 

FPGAs would be one way to dramatically increase switching frequency, but there is also specific hardware on teh market that's way cheaper than an FPGA. I've been looking into the Trinamic TMC4671. 

https://www.trinamic.com/fileadmin/assets/Products/ICs_Documents/TMC4671_datasheet_v1.05.pdf

I've got the BOB, but haven't sourced/built a power stage for it yet. I'm no EE, so it's all learning and i'm not sure exactly what i should do in that regard yet. I've got a couple local experts though, so it'll happen, just slowly. 

Anyhow, the Trinamic IC does FOC in hardware, upto 100khz switching. 
It seems from my limited knowledge that there is going to be a switching frequency for each set of FETs combined with a particular motor. Too fast and switching losses take over, too slow and the motor losses dominate. I expect you could (relatively) easily calculate each function and combine them to find the ideal switching frequency for a controller/motor combination. 

If anyone wants to build a power stage for the TMC4671, i'd be glad to test on my dyno (which just got some upgrades last night). I've got a small stack of motors, and some other controllers to compare the Trinamic to.

Peter
```

---
## \#165 Posted by: AlexBE Posted at: 2019-02-02T23:01:40.604Z Reads: 90

```
What part of the performance are you trying to improve by moving to an FPGA? You mention "crazy switching frequencies", if you mean the PWM frequency, that is constrained by switching losses. The only thing to be gained in our application by an FPGA is efficiency at high speed, but its a few percent at most. The things lost are cost, complexity, availability of parts etc....
```

---
## \#166 Posted by: Petertaylor Posted at: 2019-02-02T23:03:54.368Z Reads: 92

```
Ok, finally got around to making some new mods to the dyno. Cleaned everything up, improved rpm sensor, added a better ADC for current and voltage measurements (importantly with a much more stable voltage reference). 
Basically numbers are getting closer and closer to reality and more and more consistent. 

Somewhat gladly, the latest numbers seem to show no big change in total system efficiency on the VESC+motor when changing switching frequencies. 

![efficiency%20with%20varying%20switching%20frequencies|690x343](upload://xbaXcvRYnz0B7L4QZGzJysamKAF.png) 

Thoughts?
(edit: this is with a different motor to some previous motor tests, so perhaps there is a motor inefficiency at higher switching frequencies i discovered before (rather than a controller inefficiency), that this SK3 6364 213kv doesn't see. as always more testing needed to get concrete results, as though such a thing is even possible :-) )
```

---
## \#167 Posted by: Petertaylor Posted at: 2019-02-02T23:08:40.582Z Reads: 87

```
Some of us are really concerned about efficiency, and to us a few percent matter. Most folks don't care in the slightest. 
In certain cases faster switching makes more sense, and the vesc is pretty limited in max switching rate it seems, so the thought might be to open up different types of motors with an FPGA or faster hardware. Again though, you're right in that for most cases it likely doesn't matter, and the added cost isn't worth the marginal benefit.
```

---
## \#168 Posted by: Pedrodemio Posted at: 2019-02-02T23:36:14.805Z Reads: 82

```
That’s good, now that my board is back working I will do the tests if I have some time this week
```

---
## \#169 Posted by: Gamer43 Posted at: 2019-02-03T00:00:44.966Z Reads: 84

```
Which MOSFETs are you using that are making switching losses a problem? 
Also, one of the things an FPGA provides is deterministic behavior across a range of conditions, assuming it is still performing the same algorithm, which is unlike a MCU, which may behave differently depending on what you load it with. This provides consistent performance across said range of conditions. Additionally, a surprisingly small FPGA can accomplish complex algorithms, and, this is what one of my professors told me, a relatively cheap FPGA can implement an algorithm that would otherwise require beefy and expensive MCU. However, you have a great point that FPGA development is much more difficult and costly than MCU software development, and since they aren't produced in as much volume, unit availability could also be a problem (BUT since it is an FPGA, the design can be easily ported over to other, potentially available,  parts). The potentially lower production cost may not in many cases justify the additional develoment cost and time to market. It was just a thought I had, if it is not suitable for this application, then that is my mistake.
```

---
## \#170 Posted by: AlexBE Posted at: 2019-02-03T00:45:59.237Z Reads: 80

```
Mosfet switching losses are a problem no matter which mosfets you use. I would guess that at 30kHz switching losses would equal conduction losses.

MCUs are also deterministic as long as the program is written correctly.

Oh your professor told you? Take what people who work in universities with a grain of salt unless they have extensive industry experience. Working in commercial design vs a university is a completely different world.

The production cost will always be more because you need a host MCU AND an FPGA.
```

---
## \#171 Posted by: Petertaylor Posted at: 2019-02-03T01:09:41.771Z Reads: 77

```
Alex, if you can disPROVE a statement, do that. Don't simply tell him that his professor is wrong without anything other than some snark. I've seen folks with doctorates be wrong, i've seen people with 40 years of industry experience be wrong, i've _definitely_ seen folks on internet forums be wrong. 

Can we be civil, and discuss things without the "Oh your professor told you?" snark, can we?
```

---
## \#172 Posted by: AlexBE Posted at: 2019-02-03T01:27:11.659Z Reads: 77

```
Never said his professor was wrong
```

---
## \#173 Posted by: Gamer43 Posted at: 2019-02-03T01:31:55.835Z Reads: 83

```
[quote="AlexBE, post:170, topic:30928"]
Mosfet switching losses are a problem no matter which mosfets you use. I would guess that at 30kHz switching losses would equal conduction losses.
[/quote]

Check out the NTMFS5H600NL, at 1A source, 2A sink (gate drive currents), 40V system voltage, 25khz PWM (50khz switching) switching losses don't equal conduction losses until 160A, assuming three phase sine is generated. Even higher if running trapezoidal control. It has 15nC of gate switching charge, and 1.3miliohms rdson.

[quote="AlexBE, post:170, topic:30928"]
MCUs are also deterministic as long as the program is written correctly.
[/quote]
Yes, but proving that a program implementing an algorithm is deterministic is much more rigorous than proving a digital circuit is deterministic, assuming you can write such a program in the first place (and if so, such programs that can be formally proven to be deterministic often prove very difficult and/or time consuming to write). See halting problem. Although it's not hard to write and prove that a program that can be reliably said to behave a certain way, though not necessarily formally and rigorously proven.

There are many FPGAs (that are under $10 in single quantity) nowadays that have embedded CPU cores and non-volatile memory, meaning you don't need an external chip to store and load the configuration file. 

One problem I've noticed with industry is the inertia they have behind what's already done, now there's really good reasons for going with what has been done and proven itself in the field, but sometimes trying out some of the new-fangled toys might yield promising results.
```

---
## \#174 Posted by: AlexBE Posted at: 2019-02-03T01:42:15.111Z Reads: 81

```
[quote="Gamer43, post:173, topic:30928"]
Check out the NTMFS5H600NL, at 1A source, 2A sink (gate drive currents), 40V system voltage, 25khz PWM (50khz switching) switching losses don’t equal conduction losses until 160A, assuming three phase sine is generated. Even higher if running trapezoidal control
[/quote]
 So we agree that the switching losses are significant.

[quote="Gamer43, post:173, topic:30928"]
proving that a program implementing an algorithm is deterministic
[/quote]

Given that FOC is not written for the banking industry, the program doesn't have to be proven. To the extent that it matters for motor drive applications the VESC code is deterministic. It doesn't run differently depending on what else it has to manage (like CAN, USB, displays etc). The switching parameters are calculated at a fixed time interval by design and the peripherals are run at a lower priority.

[quote="Gamer43, post:173, topic:30928"]
One problem I’ve noticed with industry is the inertia they have behind what’s already done, now there’s really good reasons for going with what has been done and proven itself in the field, but sometimes trying out some of the new-fangled toys might yield promising results.
[/quote]

Absolutely right. The reason 99% of eskate piggybacks off the open source VESC is that no other system existed with that level of configuration ability. All motor drive systems that I have developed were for a specific motor and so didn't need to be user configured. For those applications maybe an FPGA would be a good option. Even then it would have to be extremely high speed or some other difficulty.
```

---
## \#175 Posted by: Gamer43 Posted at: 2019-02-03T02:15:27.737Z Reads: 82

```
[quote="AlexBE, post:174, topic:30928"]
> Check out the NTMFS5H600NL, at 1A source, 2A sink (gate drive currents), 40V system voltage, 25khz PWM (50khz switching) switching losses don’t equal conduction losses until 160A, assuming three phase sine is generated. Even higher if running trapezoidal control

So we agree that the switching losses are significant.
[/quote]

Wait, I made a mistake with the current benchmark, what I should say is, switching losses dominate at under 
16A, in which case it is about 1W of power at 16A across the entire power stage (no problem at all, even without a passive heatsink most power stages can dissipate 5W of power without a problem), after which, conduction losses are the main issue. 

Even at 50khz PWM, (100khz switching) switching losses dominate under 32A, in which case its losses are 4W at 32A, yeah this may require additional heat dissipation hardware, but considering that the VESC default pwm frequency is 10khz (20khz switching), I think it has quite a bit of headroom before it runs into power dissipation issues. (from my own tests, the VESC can only go up to 35khz PWM, 70khz switching, before stalling and bricking itself).

This means if a VESC were to use the NTMFS5H600NL at the default switching frequency in FOC, switching losses would be utterly negligible, as it would amount to less than 1W of power across a large part of its usable range, and even then, conduction losses are your problem. I.e. 80A is a reasonable upper limit, switching losses in default configuration are 2.2W, conduction losses 23W, more than 10 times as much.

You are correct that switching losses must be considered when specifying and qualifying a power stage, what I'm trying to say is conduction losses are a more significant contribution (among other considerations) when designing the motor controller if you spec out the proper MOSFETs, (i.e. if your application requires switching, I would advise against MOSFETs from International Rectifier, they are rugged, but their switching characteristics don't compete very well against similarly price MOSFETs on the market. Infineon is trying to fix that, but there is still some work to be done).

Although, one problem with "specing the proper MOSFETs" is that the "proper MOSFETs" may cost twice as much, and that can prove problematic. However, in this case, the NTMFS5H600NL is actually cheaper than the IRFS7530.

[quote="AlexBE, post:174, topic:30928"]
> proving that a program implementing an algorithm is deterministic

Given that FOC is not written for the banking industry, the program doesn’t have to be proven. To the extent that it matters for motor drive applications the VESC code is deterministic. It doesn’t run differently depending on what else it has to manage (like CAN, USB, displays etc). The switching parameters are calculated at a fixed time interval by design and the peripherals are run at a lower priority.
[/quote]

For our application, (eskating) yes, for all intents and purposes it can be reliably said to run an FOC algorithm up to a certain switching frequency. Occasionally, there's a glitch, but most of the time it works.
However, other applications require a much higher standard of reliability, such as Electric Cars and precision servo controllers, and I have seen others consider the use of the VESC firmware to scale up to significant EV applications. In those cases, deterministic behavior would need to be ensured.  


Since most of the configuration in the FOC algorithm is in tweaking the values of certain (or many) parameters, the main FOC algorithm is essentially the same (in terms of the instructions it executes and how it handles data) in most configurations.
What I'm trying to say is, maybe if we can hardwire the base algorithm in something like an FPGA, and offload the tuning/detection, configuration functionally, and communication off on the embedded CPU core, which then loads the relevant parameters in shared memory, then there is a possibility to lower the cost of the controller as well as push the limits on how hard and how fast the controller can run. Additionally, since the algorithm itself becomes a digital circuit, scaling it up to two or even four simultaneous motors becomes much easier, all the while preserving deterministic behavior.

(this is what I meant by programs are harder to be proven as deterministic, if a program meant for one motor is scaled for two motors, but run on the same processor, at any given point in time, the motors might require more computation than they do normally, and this can potentially cause problems with hitting certain real-time deadlines, what I mean is, let's say the average computation of one motor is less than half that of the CPU's maximum processing power, this does not necessarily mean the CPU can handle the computation for two motors 100% of the time, since there may be times the motors require more computation than other times, and if this happens with both motors simultaneously, there will be a problem).

This was just an idea I wanted to share, if it is impractical, then by all means ignore it :).
```

---
## \#176 Posted by: AlexBE Posted at: 2019-02-03T02:27:51.514Z Reads: 70

```
[quote="Gamer43, post:175, topic:30928"]
This was just an idea I wanted to share, if it is impractical, then by all means ignore it :).
[/quote]
It definitely is a very interesting idea and if you ever make one, please open source it and I will contribute (or buy some of your hardware). However, to my knowledge, nobody uses FPGA in BLDC applications. All the major players make motor controllers (TI, stmicro, microchip, LT, Trinamic etc...), AFAIK none of them use FPGA or anything similar.

Similarly I have never seen a teardown of an EV, train, Formula E where the custom controller uses an FPGA. I believe the reason is that they are not required and are inferior to the other options.

I think in general you underestimate the ability of a normal microcontroller to be reliable in time-critical control applications. The VESC uses an update rate that will never glitch if you run it at the recommended speeds. Of course what would be nice is being able to run a much faster update rate so that high ERPM contains smoother control signals.
```

---
## \#177 Posted by: Gamer43 Posted at: 2019-02-03T02:40:57.360Z Reads: 80

```
[quote="AlexBE, post:176, topic:30928"]
> This was just an idea I wanted to share, if it is impractical, then by all means ignore it :).

It definitely is a very interesting idea and if you ever make one, please open source it and I will contribute (or buy some of your hardware). However, to my knowledge, nobody uses FPGA in BLDC applications. All the major players make motor controllers (TI, stmicro, microchip, LT, Trinamic etc…), AFAIK none of them use FPGA or anything similar.

Similarly I have never seen a teardown of an EV, train, Formula E where the custom controller uses an FPGA. I believe the reason is that they are not required and are inferior to the other options.
[/quote]
I am hoping to develop some sort of BLDC motor controller with an FPGA as a research project next semester in one of the embedded labs at my university, I will do my best to have it come to fruition.

What I know some of these companies and applications do, is they design a prototype in an FPGA, but then move forward to creating an ASIC, (I think that is what Trinamic has done, their products are ASICs, I also know Allegro Microsystems has some sine wave controller ASICs as well.)

And also back to the point of the development cost and time to market, it is much cheaper and faster to develop an algorithm on an MCU rather than an FPGA, so that is likely why in those teardowns an FPGA was nowhere to be found, either an ASIC was put in, or the developer didn't want to spend the extra time and resources on what they deemed unnecessary and put in a MCU or application processor.

I don't doubt that microcontrollers can be reliable in time-critical real-time applications, what I was trying to say was, some applications require a much more expensive and powerful MCU in order to ensure that reliability and that there was a possibility that a potentially cheaper FPGA could accomplish the same task. 
For example, lets say an algorithm doesn't need to do much with data, but has to handle a lot of data at a time and do it quickly. Going the MCU route means needing something with SIMD instructions, but with an FPGA, just copy-paste the circuit a bunch of times. Potentially cheaper to produce, potentially much more headache.

Basically what I mean is, with MCUs, a lot of feature may end up unused, that's unused silicon that you paid for. With an FPGA, you can use all of the silicon for your application if you wish.

I also forgot to mention, I used to intern for a company that produces rockets, their engineers heavily preferred the use of FPGAs because ASICs were not cost effective, but they needed 100% reliability and short latency from resets or other events. Some of them told me that certain events couldn't wait for the processor to do a reset cycle.
```

---
## \#178 Posted by: Petertaylor Posted at: 2019-02-03T03:26:13.311Z Reads: 79

```
Ok, what do y'all think is going on here?
![long%20wires2|690x354](upload://oGIiyeer5cvRz2XW3NxWQBgYC85.png) 

I'm testing the same setup with and without about 60in of 10awg phase wire. Various FOC switching frequencies. at first i didn't redetect the motor with new phase wire lengths, but then redetected. No real change there. Certainly there is some run to run variation (partly because i don't have a burly enough power supply, and keep swapping batteries back and forth, so voltage from one run to another might vary from 32v to 29v. or so. 

I colored these points and fit lines so that 
BLUE is long wires
ORANGE is short wires

My instinct is to suspect the longer wires are acting as antennae, and inducing currents in the other measurement wires. I've tried waving the loop of extra phase wire around the apparatus, without any effect. 

The other thought it that maybe the added inductance is beneficially holding energy then releasing it over time to the motor coil. This could decrease the current spikes, and thus decrease the resistive heating on te coils.

Am i crazy? what the hell is going on? 

Next up i'll be putting a current probe in one phase wire attached to a scope to see if there is a visible difference. 
Thoughts?
```

---
## \#179 Posted by: Gamer43 Posted at: 2019-02-03T03:42:01.214Z Reads: 80

```
Few things are going on, firstly, at what point are current and voltage measurements being taken? How far away is it from the controller, and what path do the measuring wires take? Electroboom did a series of videos illustrating how critical probe points and the path that the wires take to those probe points for dealing with picking up EMI in your measurements.

Adding the additional wire increases BOTH resistance and inductance, according to an online calculator adding 60in of 10AWG increases phase resistance by 5miliohms, and inductance by 1uH, (assuming it is uncoiled).

This has a significant impact on the phase angle of the current with respect to the applied voltage. Basically, the greater the phase angle, the less DC current needed from the DC bus to generate the three phase AC.
It also impacts the reactance, meaning a higher applied voltage is needed to achieve the same current (but this is reactive power and should be returned to the DC bus). More inductance = bigger phase angle, more resistance = smaller phase angle, but it's based off the arctan of reactance (which is also dependent on frequency) so the relationship is very non-linear.
DC current consumption is scaled by the cosine of the phase angle.

It's a little counterintuitive that this would result in less power consumption from the DC bus, but I guess not outside the realm of possibilities if the motor has a very high phase resistance but very low phase inductance (and as a result would also lower the max speed and power output of your motor).
(I guess the wire acts as a ballast???)
What were the original detected phase inductance and resistances?
```

---
## \#180 Posted by: AlexBE Posted at: 2019-02-03T03:52:27.955Z Reads: 75

```
What kind of lowpass filtering are you doing to your input/output power measurements? (to avoid induced errors like you suggest)
```

---
## \#181 Posted by: Petertaylor Posted at: 2019-02-03T04:01:12.975Z Reads: 82

```
I saw that electroboom series. 

originally, tests done with same detection settings: 14mOhms, 6.19uH, 3.508mWb, 0.0062KP, 14.02KI, 81.26 Observer Gain

I changed that after the first few long wire measurements to 19.6mOhms, 8.38uH, 3.451mWb, 0.0084KP, 19.61KI, 83.97 Observer Gain. 

The change occured when the legend says "redetected" though the colors are all now the same so you can't see what effect that had. I can share the excel file with more data, and an additional graph with separate colors for each run. That one was just a bit busy to show the trend of long vs short. 

That's all i took note of, though i think in a motor detection, that's all the changes.

Setup is VERY far from well isolated from EMI. 

![IMG_20190202_194916|666x500](upload://kK5BYOJnh1XD1CFXT3rBPJCFoTz.jpeg) 

This is with a less organized set of phase wires, but needed the additional current sensor to be closer to the MCU to steal it's 5v for the sensor. 

Scope showed this on one phase for current. No vertical scale units, but it's linear. Shape was what i was attempting to see. The individual pulses are visible, but the sine wave is reasonably clean.
![DS1Z_QuickPrint1|690x414](upload://5X4d19PnmLbEvxHsrPa3oyoebLX.png)
```

---
## \#182 Posted by: Petertaylor Posted at: 2019-02-03T04:29:27.362Z Reads: 83

```
...and a comparison with short wires again

![long%20wires3|690x355](upload://je1WYyqk1hcg6kYCXN7sGXea8CB.png) 

PURPLE is the long wires from above,
RED is the short wires

here is the scope trace from the short wire test. no real visual difference. Could be less spikey. I only took one shot the last time, and this time took a few. Some had more noise, this is about average. 

![DS1Z_QuickPrint7|690x414](upload://hoeFbePXZu14E3arD8MWTQcPfCR.png) 

Current sensor supposed to have a max frequency around 100khz iirc. Not ideal for catching these spikes, but that's what i've got.
```

---
## \#183 Posted by: Petertaylor Posted at: 2019-02-03T04:42:28.598Z Reads: 85

```
hmmm, no big difference.
did another, more zoomed in test, and this time with identical settings, at the same speeds and loads.
long wires, 
![longwires1|690x414](upload://uY7BMyz7bn5XLHl2pj1nHbw4P6m.png) 

short wires,
![shortwires2|690x414](upload://aI4uizJ13Me2HpTkhO1q15bnbxQ.png) 

very subtle differences, but (i think?) spikier on the short wires. Think i'm at the limit of the sensor though :-/ I expect the difference would be bigger if i could see it.
```

---
## \#184 Posted by: AlexBE Posted at: 2019-02-03T04:49:24.268Z Reads: 78

```
I apologize if you have explained this further up in the thread... How are you calculating power -> efficiency? You aren't using the scope are you?
```

---
## \#185 Posted by: Petertaylor Posted at: 2019-02-03T04:57:30.745Z Reads: 80

```
No, i've got a current and voltage sensor for electrical power input. 
I've got rpm and a load cell with torque arm attached to the motor for mechanical power out. 

I'm averaging basically everything a few times over. 
I'm using median where i can to eliminate outliers. An arduino collects data, 100x a second for current, voltage, 10x second for load cell, and whatever is needed for rpm (1/rev). I'm then requesting those averages 10x a second with a python script. That data gets averaged in python, and the median is taken again for 10 data points.

So each point on the graph draws from 100 samples for voltage and current, and 10 for torque.  I've average for longer in python, but didn't see better data. I've got a capacitor on the current sensor in the dyno for slower, smoother results. Forget what frequency it brings it down to, but i expect i shot for 100hz. 
Nothing super fancy. 
http://www.taylorpeter.com/#/duelling-motors-dyno/
```

---
## \#186 Posted by: AlexBE Posted at: 2019-02-03T05:56:35.437Z Reads: 76

```
Makes sense. Are you using an off the shelf current/voltage sensor? Does it give power?

My suggestion is to do much more aggressive low pass of the current (voltage) signal. I have a strong suspicion that you are seeing aliasing of a higher frequency signal messing with your data.

Do you agree that adding the long phase wire does not give the result you would expect? If it does truly increase the efficiency of the system, maybe the vesc timing is off and it can be improved which would be nice.
```

---
## \#187 Posted by: Gamer43 Posted at: 2019-02-03T08:23:47.822Z Reads: 79

```
Adding the long phase wires reduced the efficiency at lower speeds, but it climbed to higher efficiencies at higher speeds.

Could it be possible that the added resistance and inductance (maybe even the parasitic capacitance?) is having a weird effect on the reactance and power factor of the system (as well as how much reactive current is dissipated as heat)?
Could it be possible that the longer phase wires generate less reactive current (than without) that is being dissipated as heat? (since power loss is proportional to the square of current, while linearly proportional to resistance).
Or am I just wrong and the current control loops are supposed to ensure reactive current is zero?
```

---
## \#188 Posted by: Petertaylor Posted at: 2019-02-03T10:18:35.797Z Reads: 84

```
Voltage is a simple voltage divider circuit 11:1 on a channel of the ADC.
Current is a pololu breakout, based on the allegro ac709, hall effect current sensor. https://www.pololu.com/product/2199

No power, but since i'm measuring voltage and current into the ESC, which is buffered by some fat caps, the power into the ESC is calculated by simple V*I. voltage is super steady. 

Come to think of it, I didn't do any math, but i assume the caps aren't holding enough power to affect the test. They couldn't be, could they? 

If the caps start charged, and the voltage gradually drops during the test, then some amount of energy stored in the caps is entering the system. That energy might explain a false high at the beginning each test (at high rpm), before the voltage sags. If the voltage sagged more and/or faster in the long wires setup, then perhaps the general trend line would be steeper. Can't say i'm noting how long each run is taking in clock time, thought it could easily be measured. Don't think there is a difference, and it wouldn't explain the higher start.

The caps are 680uF *3. That's about a joule at 32v. A watt is 1 joule/second. The power input is about 400w, so it's 1/400 second worth of power. Blows that theory.

I too think there is something else afoot. If an aliased signal from somewhere else, why such repeatability? What would be the source? How can we test this theory most easily?

More aggressive lowpass of the current where? on the sensor before the ESC? That sensor is already buffered with a capacitor, effectively a lowpass (though using pads built into their breakout board).
```

---
## \#189 Posted by: AlexBE Posted at: 2019-02-03T13:35:28.281Z Reads: 79

```
You're right about repeatability making it unlikely that there is a high frequency aliasing problem. Ill have a think about this in the morning and see if I can think of something.

Yeah the caps only hold a few ms of power, but as long as its more than one PWM cycle they do their job!
```

---
## \#190 Posted by: Petertaylor Posted at: 2019-02-04T00:11:02.080Z Reads: 81

```
Yeah, the numbers feel wrong, so it's smart to investigate the various errors in the methodology i might be making. However, it's also possible the data is right, and it's a matter of understanding why longer wires might be better at higher rpms with this motor, power level and esc. 

The main difference between low and high rpm on the same motor is the period of the FOC sine wave, and the number of pwm pulses in that wave. What about a more quickly changing PWM width favors higher inductance?
```

---
## \#191 Posted by: AlexBE Posted at: 2019-02-04T01:13:14.463Z Reads: 80

```
I think that with a perfect controller, the longer wires that don't make up any part of the windings will always make the performance worse. If the measurements are correct, I guess the effect you are seeing is due to timing differences being caused by the long wires. eg the ESC is firing too early, and adding the long wires brings it back into the correct alignment. Maybe there is a setting that allows you to modify the timing?
```

---
## \#192 Posted by: Petertaylor Posted at: 2019-02-04T03:46:00.948Z Reads: 77

```
Interesting idea.
Not sure about a way to change the timing directly, but altering the detected inductance may be hack-y way to achieve that. I'm certainly no expert :-/
```

---
## \#193 Posted by: AlexBE Posted at: 2019-02-04T04:54:49.506Z Reads: 76

```
If only we knew someone who could try manually adjusting the detected inductance and seeing what effect it had on efficiency......
```

---
## \#194 Posted by: Gamer43 Posted at: 2019-02-04T05:35:34.230Z Reads: 77

```
Just something I'd like to add,

I took another look at the firmware, the VESC measures inductance at a switching frequency of 3khz.
This may have an effect, since the inductance of an inductor is not necessarily constant with respect to frequency, especially since a motor's inductance will have several resonant frequencies due to the parasitic capacitance between windings. 

![image|690x30](upload://8rQlBRRyg7H3aNixtq8gSuZ1QDc.png) 

I also REALLY don't like the way the VESC firmware does the math here, there might be some floating point round off errors happening as well in the calculation.
I would write it as float t = (float)((uint_16)(TIM1->ARR * m_samples.measure_inductance_duty) - (MCPWM_FOC_INDUCTANCE_SAMPLE_CNT_OFFSET + MCPWM_FOC_INDUCTANCE_SAMPLE_RISE_COMP)) / (float) SYSTEM_CORE_CLOCK

Honestly, I would just rewrite the measure inductance function to avoid floating points as much as possible. Calculate everything using fixed point arithmetic, then convert to float in one final calculation to avoid loss of precision and round-off errors.

Like, the avg_current and avg_voltage running totals, accumulate those as 32 bit integers, then add the relevant floating point scalars in one final calculation.

Additionally, there isn't any dead-time compensation in the calculation, the sample rise time constant partially, but not completely compensates for it.
```

---
## \#195 Posted by: AlexBE Posted at: 2019-02-04T05:36:46.266Z Reads: 74

```
If you guys have discovered something that increases efficiency this much, it's very interesting. Im just annoyed my dyno is no longer assembled (all the bits are in my board).
```

---
## \#196 Posted by: Petertaylor Posted at: 2019-02-04T05:37:42.018Z Reads: 81

```
Lol. Yeah, i'll do that someday soon. 

I think i need to make the dyno frame a little more rigid. Worrying that some of the vibrations i'm seeing are robbing energy, or worse, resonating only at certain rpms, which cause irregularities in the data. Checked every bolt on the thing a found a few that were less snug than i'd like. Running the thing makes some noise, so it'll have to wait until tomorrow. 

Did a few tests on another motor (this time on the other side of the rig, because it has no way to support the spinning end. Adds 1 bearing's worth or resistance). The curves are super weird looking. Humps and troughs! Could be a property of the motor (Flipsky 6374 190kv), or could be evidence the dyno is acting strangely. Also on a different VESC.
Inconclusive.
```

---
## \#197 Posted by: Petertaylor Posted at: 2019-02-04T05:42:48.207Z Reads: 79

```
It's almost greek to me. I'll believe you that it's not awesome. 

I was considering using an external LCR meter to test inductance and resistance on motor coils. Might be interesting to use measured values. 

Don't have one at home, but i hope we've got something at work.
```

---
## \#198 Posted by: AlexBE Posted at: 2019-02-04T08:30:43.393Z Reads: 78

```
consider adding a flywheel too if you need smoother rpm.
```

---
## \#199 Posted by: Petertaylor Posted at: 2019-02-04T19:15:40.113Z Reads: 79

```
First dyno was entirely a flywheel. (http://www.taylorpeter.com/#/flywheel-dyno/) It was a pain in the ass. 

I'm waiting long enough that the rpm is stable, and i don't average the 10 sample bracket unless the standard deviation of those 10 samples is less than a pretty low setpoint. Also, the median of the sample set is used, so a few outliers could be present without affecting the selected sample. In theory, no dirty rpm samples are getting through. 

If there is something odd going on, it's most likely in the hall effect current sensor. Datasheet for this model doesn't mention anything, but from a different model from the same manufacturer says it'll move 10mV per Gauss of external field. Who knows what gauss the phase wires are putting off, or how sensitive this sensor is to outside noise. 

Anyhow, i'll figure it out. As per  @Gamer43, I'm thinking that the VESC's inductance measurement isn't great, and that it's just a lucky accident that the increased inductance of the phase wires is beneficial for a more correct phase angle. Better tuning of the inductance settings would reveal this. Not too hard to do. Sometime soon. 

Peter
```

---
## \#200 Posted by: Gamer43 Posted at: 2019-02-04T19:24:21.715Z Reads: 74

```
Any chance you would be able to use a chassis mount shunt resistor instead? Hall effect current sensors provide galvanic isolation and lower power dissipation at the cost of precision and non-linearity accuracy problems.
```

---
## \#201 Posted by: Petertaylor Posted at: 2019-02-04T22:49:34.181Z Reads: 75

```
Send me a recommendation and i'll make it happen. Anyone make a breakout board for the current range we're talking about (~15 battery amps, so 20a minimum)?

Or send a design and i'll put something together, but less stoked on that. I'm mostly into another phase of my project.
```

---
## \#202 Posted by: Gamer43 Posted at: 2019-02-04T23:13:37.865Z Reads: 79

```
I can't seem to find any fully assembled breakouts fit for this application (I'm just bad at sourcing these kinds of things), but I did find something that could work

EDIT: Alex speced out some drone current sensors, forgot those existed, whoops.

https://www.digikey.com/product-detail/en/riedon/MSR5-0R005F1/696-1649-ND/1641092

Current shunt resistor, kelvin points are at the flat spots on the terminals.
5miliohm, 5W, 20ppm temperature coefficient.

https://www.digikey.com/products/en/development-boards-kits-programmers/evaluation-boards-op-amps/788?k=ina180

INA180 eval board, connect in+ and in- to the kelvin points on the current shunt, give it 5V and have the arduino read the output voltage. 
If you decide to try this, the eval kit gives 8 different op amps, use the ina180A1, unidirectional, 20x gain.

The ina240 is even more accurate, but costs $25 for the eval board.

Just curious, have you considered using something other than an arduino to collect data? I do know the arduino's processor and peripheral sets are bit on the low end and slow side. This could possibly be introducing error into the data due to inaccuracies in the peripheral set.

Something like the Nucleo F446RE could be easily programmed to collect data and send over UART, and has a much better peripheral set. (e.g. 12bit adc that runs way faster) It costs about $15. 
Or even the CY8CKIT-059, also $15, less peripherals and processor but it has a 20bit Delta-Sigma ADC (I think like 17 or 18 ENOB in practice) that inherently averages the signals, so it is much more accurate, and it has a digital filter block to do lowpass filtering as well. Figuring out the filter block might take too much time than it's worth, but it shouldn't take long to set up a program to collect data from the delta-sigma adc and send it over native USB or through the debugger's UART.

Quick question, is there a filter capacitor on the voltage divider?
```

---
## \#203 Posted by: AlexBE Posted at: 2019-02-04T23:33:21.153Z Reads: 78

```
https://www.getfpv.com/team-blacksheep-core-current-sensor-25-amps.html

https://www.getfpv.com/core-current-sensor-100-amps.html

Not sure which country you are in, but quadcopter current shunts are cheap and available and do what you need. However a digital one would be far better as you don't want to run analog signals to your arduino.
```

---
## \#204 Posted by: Petertaylor Posted at: 2019-02-05T02:26:34.956Z Reads: 79

```
Good suggestions. I'll look into those other microcontrollers. Amazed by that cypress controller. They're selling for 10$ + 4 shipping. That's pretty dang good in my book. 

I used an Uno because i had one laying around, and a screw terminal shield with proto space. The form factor is going away, and i'd like to use up my supply for these older boards on projects that don't need much. It's doing more than i expected it to when i started this build, but it's still not a lot. 

The arduino itself only processing digital signals, so noise is less of a problem.
An i2c connection from the ads1115 (three channels: voltage, current, current midpoint/reference). 
A data and clock signal from from the hx711 load cell sensor. 
A digital interrupt pin used for a photointerrupter for rpm. 
It's also outputting a PWM signal as a command to the tested motor controller. 

I'm pretty sure i'm not seeing anything nasty from the arduino side of things. 
I'm not using the onboard ADC, i'm using a breakout for the ads1115, a 16bit adc with onboard reference source. It's not super fast, but it's fine for the very low polling rates i'm doing (100sps max).
I think if i replaced the microcontroller, i'd replace it with something that can run python, so i could have all the code running in one place. Easier to port the smaller arduino code to python than the other way around. I'm using numpy though, so perhaps it'd have to be a Raspberry pi with external ADC or something instead.

I am running relatively long unshielded wires with analog signals from current and voltage sample locations, and that's susceptible to noise. The load cell analog output is through an already shielded cable. Perhaps replacing those two analog signal cables with shielded is an easy and smart move. 

The voltage measuring voltage divider does not have any filtering cap, but the voltage is also not changing very much at all. Ideally, it wouldn't change at all. I'm pretty sure it doesn't need filtering. It's easy to add, and perhaps i'll look at the signal on the scope while running to see if there is anything interesting going on. unlikely though. 

While all of these changes could be made, i'm somewhat dubious that it'll make much difference. I think the first step is to carefully probe the various signals with and without the long wires and see how much noise there is in either case. I'm open to making changes if i see something genuinely problematic, but can't afford the time to rebuild it over and over chasing very diminished returns if the results are at least repeatable. My goal isn't absolute numbers, more identifying the best motor, rpm, esc, and esc settings from the bunch. If there is consistent error across the board, that wouldn't actually hurt, just make the numbers detached from some real units.

Ps, i'm in San Francisco, USA. Where are you guys?
```

---
## \#205 Posted by: Petertaylor Posted at: 2019-02-05T02:28:00.427Z Reads: 72

```
Those look great Alex. I'll look into them a little more closely. I don't think accuracy is a big issue, but will be more pro-active and testing that assumption.
```

---
## \#206 Posted by: AlexBE Posted at: 2019-02-05T02:45:27.192Z Reads: 76

```
More information : I chatted to my friend who designs control systems for very very large motors, think hundreds of kW for metal extruders. He confirmed that it is possible that an increase in inductance could increase efficiency due to low pass filtering some of the high frequency components that would otherwise be going into the motor.
```

---
## \#207 Posted by: Petertaylor Posted at: 2019-02-05T21:05:04.433Z Reads: 77

```
Yeah, that's kinda what i was thinking as one explanation. Energy stored in a magnetic field reducing the amplitude of the current spike, and releasing it during the pwm off part of the duty cycle. Lower max current, means less heating of the copper. P proportial to I^2 * R. The key is that the current is squared. 

The problem remains, why lower efficiency at lower RPMs? Switching frequency is the same, so the current pulses would get the same beneficial smoothing. That's why the second theory about VESC inductance measurement being off feels better to me. That would explain the lower efficiency at lower rpms, but higher at high rpms. 

PS, i did just buy one each of those current sensor breakout you found. They'll be interesting to test as a comparison to the sensor i'm already using. Can't get info on what that IC on the board is (25amp for example). There is also a cap on there for filtering i presume, which will limit bandwidth.
```

---
## \#208 Posted by: Petertaylor Posted at: 2019-02-05T22:25:25.751Z Reads: 73

```
PS, a friend who i talked to about this wanted a speed vs torque curve, because that's a more common way to look at motors, so i made one for him. Posting here in case it helps someone see the problem/phenomena differently.

![speed%20vs%20torque|690x354](upload://dTHYu4Nx6ceCyjcxjonrSgWoHv8.png)
```

---
## \#209 Posted by: Pedrodemio Posted at: 2019-02-05T22:38:55.680Z Reads: 70

```
Are your current limits never being reached? just the power limit of 400W? if so them the curve looks correct
```

---
## \#210 Posted by: Petertaylor Posted at: 2019-02-05T23:10:35.474Z Reads: 73

```
Not sure actually. I think the controller phase current isn't being capped. Also, i can't imagine there being enough difference between the two otherwise identical tests. 

Can test again with more wide open motor phase currents, but from memory, the duty cycle is between 30-70% during the test, and the battery current is 15a or so, so max motor current would only be 45a or so. Looks like cap was 60a.
```

---
## \#211 Posted by: Pedrodemio Posted at: 2019-02-06T01:08:26.252Z Reads: 75

```
If it was you should have some distinct sections 

To verify try to limit to something like motor current 10A and battery 5A
```

---
## \#212 Posted by: AlexBE Posted at: 2019-02-06T02:11:53.958Z Reads: 76

```
[quote="Petertaylor, post:207, topic:30928"]
The problem remains, why lower efficiency at lower RPMs? Switching frequency is the same, so the current pulses would get the same beneficial smoothing.
[/quote]

It's possible at low RPM the extra resistance negative overcomes the higher smoothing effect. Who knows.
```

---
## \#213 Posted by: Petertaylor Posted at: 2019-02-06T07:11:45.749Z Reads: 77

```
So i just measured the one motor where i got the strange effect via an Digilent Analog Discovery 2 in it's impedance analyser mode. 
https://reference.digilentinc.com/learn/instrumentation/tutorials/ad2-impedance-analyzer/start

Depending on rotor position, i get an inductance between 42uH and 25uH phase to phase at 20khz without long phase wires. Apparently Vedder wants half this value as a single phase number. Half this range (21-12.5uH) is still well above the measured inductance of 6.2uH on the vesc itself. 

At 20khz with the long phase wires, i get between 44uH and 28uH.

Maybe tomorrow i'll run a test with the average of these 

I think i'd doing the measurement right, i've used a variety of known resistance values, and have run compensation. Numbers seem good, as long as the method/device is good. 

Not the result i was expecting (i was expecting a lower inductance from what VESC measured, where the longer phase wires bumped it into the correct zone).
```

---
## \#214 Posted by: Petertaylor Posted at: 2019-02-09T20:26:16.125Z Reads: 77

```
Well, those new Team Blacksheep current sensors didn't *quite* work out.

Being that they are without any documentation at all, i started making assumptions, and moved a little too quickly. 
Turns out the V+ and GND pins aren't for power for the breakout, but rather are direction connections to the power source being sampled.

Smoke, fire.

Sweet, just what i wanted.
I was using the arduino as a 5v source, but most everything else was still plugged in.
Arduino, usb hub, ADC breakout, all confirmed dead. 
Not sure yet about the pololu current sensor, load cell sensor, load cell itself, rpm sensor, but i assume they're all dead, since they all connected to the arduino or usb hub, all run on 5v, but saw 32v. At least $60 worth of smoke, but more importantly, wasted time and effort. 

Anyhow. So much for saving time by using a breakout. Also means any further testing which was already starting to be on the back burner (pun intended) is now totally off the stove. I think i've got a few spares of some of these components, but not all.

Basically, no updates for a while i'd expect. Sorry y'alls.

Peter
```

---
## \#215 Posted by: AlexBE Posted at: 2019-02-10T08:36:46.686Z Reads: 74

```
Ouch. At least it's only $60 though. I have seen hundred thousand dollar PCBs destroyed by plugging the wrong voltage in the wrong place.
```

---
## \#216 Posted by: Hummie Posted at: 2019-02-10T17:06:36.509Z Reads: 76

```
[quote="Petertaylor, post:213, topic:30928"]
Depending on rotor position, i get an inductance between 42uH and 25uH phase to phase
[/quote]
Think u need take the rotor off if using an LC meter.  The Vesc tool also does it as you know but not as exact as a cheap 15$ LC meter.  I have two n give u one for 5$
```

---
## \#217 Posted by: Petertaylor Posted at: 2019-02-11T17:58:01.185Z Reads: 77

```
Somewhat amazingly, i had at least one spare of all the things that smoked.
I think i'm back up and running, but it's still back burner for me, so while i replaced everything and did individual tests, i didn't run everything at once.
```

---
## \#218 Posted by: Gamer43 Posted at: 2019-04-07T12:51:33.503Z Reads: 72

```
Hey guys, not sure if this is the appropriate place to post this, or if it is appropriate to revive this thread,

but I was just wondering, has anyone considered porting the VESC firmware to the STM32F765VG?
It has a very similar (but expanded, including a DFSDM) peripheral set, an M7 running at 216 MHz instead of a M4 running at 168,  and is only about $1-2 more expensive in single and bulk quantity. Aside from remapping the pins, I feel that porting the code should be relatively straightforward. The M7 has roughly double the CPU benchmark (but that take with a grain of salt, it relies on the M7 being dual issue, which means that will only happen without data hazards and optimal branch speculation, not to mention cache performance).

Basically, if we wanted to run the VESC's FOC algorithm at 70khz (or run two FOC algorithms concurrently at high speed, nudge nudge wink wink), I think this is the MCU to do it, since it doesn't add much cost in comparison to the cost of the entire controller.
```

---
## \#219 Posted by: Deodand Posted at: 2019-04-07T14:09:32.018Z Reads: 77

```
Think you forgot a 7 in there (STM32F765). Chibi supports F7 so in theory all the HAL stuff should port, some of the setup varies slightly but probably easy enough. The trickiest parts will be how similar the ADC capture compare stuff works and if the PWM setup with the timers is identical. If it isn't there's substantial work there. 

In my experience it's usually easier to improve code efficiency rather than switch to marginally faster MCU. Vedder has done a decent job generally with most of the algorithms not being chunky but there's probably room for improvement. I did a bit of profiling and the time for each operation (ADC capture, estimation, control, safety limits) are all pretty comparable so no crazy dominant piece to find easy gains but there's stuff here and there.

Depends how big the real world speed jump with the processor is. Another big factor in the speed of everything is just the ADC module performance in terms of resolution/accuracy vs. sample time/rate. If it is an improvemed module over the f4 that might be worth the move. Don't have time at the moment to read a comparison.
```

---
## \#220 Posted by: Gamer43 Posted at: 2019-04-07T21:57:58.813Z Reads: 76

```
The peripherals look almost identical, at least their setup does; the F765 has a few more features on its peripherals (e.g. 6 channels instead of 4 on timer 1, more/different trigger sources for the adc).

I also forgot to mention, the F765 also supports double precision floats, not sure the actual impact on performance, but more precision always helps. 

The ADC peripheral on the two look almost identical, aside from the trigger sources, the functional block diagrams are the same; however, because of the clocking scheme, the adc on the F405 can only run at 21 MHz, while on the F765, it can run at 27 MHz. While the adcs are the same, the F765 will have better performance since the adc can be clocked faster. For reference, the maximum frequency is 36MHz. To achieve this frequency, the CPU would have to be clocked at 144 MHz due to the way the prescalars are set up. 

As long as the source code can be written (or maybe the compiler is smart enough to do this for us) to minimize data and resource dependencies between consecutive statements and instructions (data dependencies not so much, since forwarding helps prevent stalls), the code will be able to take full advantage of the dual issue pipeline and achieve an effective doubling in performance. I'm not sure how feasible this is considering a lot of the VESC's calculations are floats and there is only one floating point pipeline in the Cortex M7. There's a separate ALU and MUL/DIV pipe, but MAC instructions will consume both of those resources. 

This is another reason why I say calculations should be done in fixed point arithmetic as much as possible. The ARM Cortex M7 has two fixed point pipes, one of which is capable of MAC instructions and embedded shifts (where a register or value arithmetic shifted left or right is passed as operand, I saw this done on an implementation of the abs() function). I.e. most, if not all, microprocessors have stronger fixed point performance in one way or another.
```

---
## \#221 Posted by: Deodand Posted at: 2019-04-07T22:12:00.852Z Reads: 78

```
Yeah I agree that fixed point would be awesome. I think just switching that alone would free up a lot of resources.

Six channels on timer 1 sounds interesting. Currently on the unity I use only the first 3 channels (high and low) of timers 1/8 to drive the 12 pwms needed for full sinusoidal motors. I wonder if you could setup and use only timer 1 instead.... Maybe even drive a third motor with timer 8. Would be insane 😂

 I wonder how much time would need to be invested to convert all the time critical algorithms to fixed point, then implement transform to float/double at all the external interface points.

Anyways the main use of all this would be driving super low inductance motors in tandem I guess. Or if you wanted your motor driver to also be doing some heavy lifting on some other algorithms.
```

---
## \#222 Posted by: Gamer43 Posted at: 2019-04-07T22:41:54.380Z Reads: 77

```
Dang, just checked, channels 5 and 6 on timer 1 are not mapped externally, they're are only useful for internal timing functions D: , and channel 4 does not support complementary output.

One possibly is also moving to the DRV8353 and using its internal dead-time insertion (up to 400nS, more than enough for most hardware), this would allow timers other than timer 1 and 8 to be used for PWM generation as complementary output is no longer necessary. 

I think converting Vedder's implementation from floating point to fixed point would be tantamount to writing a new algorithm honestly; he did everything in floating point because the algorithm is very straight forward to implement, it would take a lot longer to figure out how to preserve units, get everything to a common base/scale factor, and dimensional analysis to make sure fixed point arithmetic produces the correct results. This is probably the reason why in industry they don't bother with fixed point arithmetic when there's a FPU, not worth the development cost.

But, to optimize the algorithm doesn't require doing everything with integers, there are tricks here and there to reduce the number of floating point calculations needed, which I think I mentioned before as an example, when averaging multiple samples from the adc, accumulate them first as integers, then convert the total to a float, instead of converting each sample to a floating point immediately as they are received, since the samples all have a common scaling factor. The same could possibly be done for the transforms as well, since the current samples have a common scaling factor, and when a floating point scalar is introduced, then convert the samples to floating points. 

Although, now that I think about it, there might be a way to implement the observer using fixed point xD.

An application I could think of is a fully integrated quadcopter controller >:), one MCU does it all!
Or possibly extremely precise servo control algorithms and implementing higher order speed estimators.
Maybe IoT as well, the MCU has to control a motor and manage a UI and communication with other devices.
```

---
## \#223 Posted by: Deodand Posted at: 2019-04-07T22:49:33.793Z Reads: 73

```
Yeah maybe a dual controller with a durable touch display. No phone app needed and can display battery etc. Run it all off the MCU. That would be pretty awesome. Would be so sad when you broke it haha probably better modular.
```

---
## \#224 Posted by: Gamer43 Posted at: 2019-04-08T07:53:39.184Z Reads: 71

```
Maybe a removable display? Something that pops on and off like an arduino shield xD. And instead of TFT, use a set of PCB capacitive touch  buttons and a slider.

Also, I'm just curious, do you have any say in what hardware goes into the Unity? I was wondering if you guys would be open to hardware suggestions, like MOSFETs, op amps, etc.
```

---
## \#225 Posted by: Deodand Posted at: 2019-04-08T15:18:02.411Z Reads: 76

```
Yes I have a pretty big say in how the unity is made (I designed the board). The unity at this point is locked in but we will release a revision in time. Pin compatible fets could be swapped but we are pretty happy with the current performance. 

Always open to suggestions backed with solid engineering to move forward with new innovative stuff. I enjoy our discussions :slight_smile:
```

---
## \#226 Posted by: Gamer43 Posted at: 2019-04-09T00:12:36.522Z Reads: 70

```
@Deodand 

Oh, that's awesome. 

I was wondering if you guys considered using the TPW1R306PL,L1Q? I can't recall if it is indeed pin compatible with the MOSFETs you are currently using (they're ones from NXP or Vishay, right? If the package is 5-DFN, it should be). It has higher gate charge so it would suffer from higher switching losses (but that won't be too much of an issue at our switching frequencies, and not at all if the unity is already using larger gate resistors for slew rate control, since smaller resistors can be used in that case), but aside from the nice RDSon, it features double sided cooling. Maybe higher current versions of the Unity in the future might benefit from using those MOSFETs? The other downside is it is a bit pricey at $1.3 each in bulk quantity.

I'm just wondering, are you still using the AD8418 as the current sense amps? TI recently released the ina240, it's about the same price, has the same pinout, but is much more accurate (lower input offset, lower temperature drift, higher PSRR and CMRR). 

I also noticed that a lot of VESCs don't implement some form of transient suppression and this is a reason why a lot of them have their DRV8302 die, I was also curious if you guys added RC snubbers or some other way to manage transients (such as slew rate control)?


And same, I really appreciate that you take the time to discuss these things with me.
```

---
## \#227 Posted by: c10yas Posted at: 2019-10-31T06:52:31.555Z Reads: 30

```
I'm really sorry for bumping this topic but I wanted to ask something related to this topic.
I'm want to use SiC MOSFETs at 100kHz for a high power inverter. I intend to use VESC but from this thread doubt that I will be able to given that it seems to only work up to around 30-35kHz. TI instaspin on the F28069 processor would only hit 60kHz apparently which leaves me with the very hard solution of using a motor control library like the TI DesignDRIVE and running it on a Delfino processor like the F28377S to achieve the switching frequency I aim to reach. 
PS. I know my switching frequency is really high, I have validated the switching losses to be manageable and am using such a high frequency to reduce the size and weight of my DC bus link capacitors as well as reduce motor ripple current
```

---
## \#228 Posted by: TowerCrisis Posted at: 2019-10-31T07:33:37.339Z Reads: 30

```
Are you attempting to make a motor controller from scratch?

If so, I'd recommend the DRV8301-HC-C2-KIT dev board as a starting point. AFAIK the schematics are public for it. I'd pick one up and try it out, be weary that software support is basically non-existent unless you get in touch with TI. It has up to 200khz switching frequency out of the box.

Although, it appears like you have more experience in this realm than I do and would already know this.
```

---
## \#229 Posted by: Deodand Posted at: 2019-11-01T01:47:51.905Z Reads: 30

```
Latest vesc FW supports higher switching frequencies in software by reducing control to every other pwm cycle.
```

---
## \#230 Posted by: TowerCrisis Posted at: 2019-11-01T02:00:33.947Z Reads: 36

```
Hold up, do you mean this is supported in the stock firmware now? What's the upper bound for frequency? And wouldn't that have ramifications for hardware design? (Smaller caps)

Also, is there a page or patch note where I can read about this in depth?
```

---
## \#231 Posted by: Deodand Posted at: 2019-11-03T00:41:46.638Z Reads: 32

```
It will be constrained by the maximum average gate drive current of the DRV (30 mA I think) you can determine this by using the gate charge of the fets and the switching frequency. I think for most of the vesc based drivers I've looked at it somewhere around 60-80 kHz, but I'd have to run the numbers back again. 

Vedder implemented this trick with a #define so I don't think it's a formalized method. [take a look here.](https://github.com/vedderb/bldc/search?utf8=%E2%9C%93&q=FOC_CONTROL_LOOP_FREQ_DIVIDER&type=)

I don't think higher switching frequency eliminates the need for bulk caps. Even with extremely high switching frequency driving the motor can require instantaneous steps in current draw. I remember seeing somewhere else someone claiming a lot of efficiency is lost in the electrolytic caps but it's pretty easy to see that's false just by looking at which part of the ESC is getting hot (FETs not caps).

Higher switching frequency means higher switching losses so the bigger number is not always better, really depends on the motor.
```

---

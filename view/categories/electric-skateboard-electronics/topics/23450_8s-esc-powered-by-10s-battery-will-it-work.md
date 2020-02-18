# 8s ESC powered by 10s battery - will it work?

### Replies: 39 Views: 4223

## \#1 Posted by: TeknoAbu Posted at: 2017-05-19T10:19:05.201Z Reads: 163

```
Hi! I'm currently trying to build an electric skateboard. 

For the project, I bought a Turnigy Aerodrive SK3 6364 190kv electric motor (all links are 
in the bottom), and a Turnigy TrackStar 200amp ESC without being aware of the fact that the ESC was 8s.

I then found a Li-ion battery in some electric scooter I don't use anymore, and thought I could use that instead of buying a new one. But this battery is 10s Li-ion (36V) and the ESC is 8s LiPo (34V MAX). 

The battery fits perfectly for that motor, but apparently not for the ESC.

Does LiPo difference from Li-ion when talking cells, and will this even work in first place? 

Thanks in advance, and sorry for my obvious bad knowledge about electronics in general.

ESC: https://hobbyking.com/en_us/turnigy-trackstar-1-5th-scale-sensorless-200amp-8s-opto-car-esc.html

Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html
```

---
## \#2 Posted by: Print3r Posted at: 2017-05-19T10:24:12.197Z Reads: 160

```
8S ESC + 10S battery = magic smoke, then fire, lots of fire
```

---
## \#3 Posted by: Okami Posted at: 2017-05-19T10:27:20.443Z Reads: 161

```
Latest I found when someone has attempted to do this is on ebike scene:

https://www.electricbike.com/tangent-ascent-6kw-the-ultimate-mid-drive/

> But there is a problem: the Talon HV120 is designed for a maximum 12S LiPo battery pack – that’s 50.4v max, as shown on the company’s site here. In the e-bike world, we like to use 14S packs, which are 52v nominal. These have several advantages over using 48v packs (discussed in previous electricbike.com articles). But the problem when using these with the Ascent is that, fully charged, 14S packs put out 58.8v – way above the controller’s 50.4 maximum design spec. After completing the build, I first test-drove my Strive with a half-charged pack (about 50v), and everything worked perfectly.  Then, I fully charged the pack for a full off-road test drive the next day. However, when I tried to test the bike on the stand, I found that the motor would apply power for a fraction of a second, then cut out. Let off the throttle, then apply throttle again, and it’d do the same thing. Power would apply for a fraction of a second, then cut off. I thought something was seriously wrong with my kit – I didn’t know about the HV120s voltage limit. After readying up on the controller, I realized that I was probably over the max voltage the controller can handle. An e-mail to Dave DuBose confirmed my intuition, that a 14S lithium pack hot off the charger is just above the voltage limitation for the HV120.

> The next days were filled with extensive testing, to learn just where the controller’s high voltage limit lies. **I found that you can reliably feed 57.4v to the HV120 and it’ll work perfectly** – which is pretty amazing, considering the unit is designed for 50.4v maximum. The HV120 gives status beeps upon power-up that indicate any error condition, as well as telling you how many series cells are in the battery pack you have connected. In the case of my 14S pack at 57.4v, it always gives you 12 beeps – indicating a 12S pack. But this makes sense, as the unit is designed for a 12S pack maximum. If you feed it 58.8v, the controller just beeps twice upon startup. Anyway, 57.4v is the max. The positive side to this is that 57.4v is also, coincidentally, the exact voltage of a 14S pack charged to 90% – so you could implement a regimen of charging your pack to only 90%, which will greatly extend the life of the pack. The downside to this is that sometimes the pack still needs to be fully charged, to balance the cells. Also, you’ll need to purchase a charger that can charge to 90% – either the Luna Advanced Chargers can do this, or the Cycle Satiator from Grin Technologies.

Though controller is Talon ? / Castle creatons and it was stock 12s controller (48v-52v) and max he got was about 57v out of it to make it work.

Im actually surprised it just didnt burn or something but just gave an error code.

Ive heard a lot of people over volt regular ebike controller but with rc stuff it might be a bit different.

So yes, do on your own risks and know that it can go bad.
```

---
## \#4 Posted by: bartroosen12 Posted at: 2017-05-19T10:37:57.558Z Reads: 128

```
We can't tell if it works or not, you should test it!
10S vs 8S is only 8V difference so I don't think the esc will smoke instantly.
I've recently seen someone who connected a 8S battery to a 6S esc with no problems so I should really test it.
Do you have still warranty on the esc? Otherwise you can always send a RMA to hobbyking after the test :stuck_out_tongue:
```

---
## \#5 Posted by: Okami Posted at: 2017-05-19T11:03:23.634Z Reads: 123

```
yeh, if he attempts to do it, I would maybe go 'slowly'·.

Starting at 36v (50-60% of charge) then upping it to 80-90% of charge to see what happens.
```

---
## \#6 Posted by: Maxid Posted at: 2017-05-19T11:47:50.619Z Reads: 117

```
why? He is only stressing the ESC not the battery.
```

---
## \#7 Posted by: Print3r Posted at: 2017-05-19T11:50:16.843Z Reads: 113

```
I have blown two escs on my quad with over-current of 4As (pulling 16A on a 12A esc). I would assume that going similarly above the max-voltage will do similar.
```

---
## \#8 Posted by: Maxid Posted at: 2017-05-19T12:01:54.389Z Reads: 109

```
no - voltage is less of a problem than current. Current destroys traces while voltage (usually and in limits) does not affect them.
```

---
## \#9 Posted by: MoeStooge Posted at: 2017-05-19T12:20:33.814Z Reads: 104

```
I've been using the 200a trackstar @ 8s and enjoy it's reliability and performance. 10s would be bitchin. I say no guts no glory, go for it🤘
```

---
## \#10 Posted by: Okami Posted at: 2017-05-19T12:21:51.930Z Reads: 104

```
yeh.. amp limit is pretty high already, so lets hope they have designed some headroom for voltage too.. :D

Maybe he can add some caps or something, (if it works at all) to avoid the spikes / voltage fluctuations.

--

One more way would be to just cut and resolder connections to make it 8s battery but then the charger wouldnt work and it would cause more custom work, so if it works with 10s battery then that is probably the easiest solution now.
```

---
## \#11 Posted by: TarzanHBK Posted at: 2017-05-19T13:12:46.170Z Reads: 94

```
someone on here tried 8s on a 6s esc and got magic smoke.
If you wanna try it, go for it, but prepare to lose your ESC.
If you wanna keep it, don´t use it with higher voltage.
```

---
## \#13 Posted by: TeknoAbu Posted at: 2017-05-19T13:41:17.178Z Reads: 84

```
Thanks for all the replies, everyone! The difference from 10s to 8s sounds a bit less risky than 8s to 6s, but I won't sound like a smart person, I know close to nothing about electronics like these. But if magic smoke is the case, I'm not afraid of losing the ESC, and I'll test it for science whenever I get time in the upcoming weekend. Updating asap! :slight_smile:
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-05-19T13:53:14.325Z Reads: 79

```
Pls take a video, the first time you´ll use it. We love magic smoke here :smiley: :dash:
```

---
## \#15 Posted by: Okami Posted at: 2017-05-19T13:59:31.114Z Reads: 81

```
Would be cool, if you wouldnt 'slam' a fully charger battery right to the esc to see what happens :slight_smile:

Then again, u might as well do just this, if you intend to use it fully charged and dont fear of loosing esc straight away..

I would say it might work up to 9s, who knows, but with full 10s voltage there might be a problem.

 Consider that fully charged 10s battery outputs **42v**, while fully charged 8s voltage is below **34v**,

I would say 38-39v is your 'safe bet'' and 35-36v might still work reasonably well but then you dont get much capacity.

**Try to charge till 38.5v (~70% capacity) and only then plug in the esc..**

**Though I would probably plug it in at 35v, then at 36v and slowly go upwards..**

--

If we take high voltage lipos (4.35v voltage), then they are at 8x 4.35v = 34.8v.

Though im not sure if manufacturer designed it for high voltage lipos, so yeh, maybe start low and only then go till max voltage.

I dont know how big scooter battery you got, but if it is 6ah, and you charge it till ~70-80%, 4ah you will get out might still be a reasonable range

36v x 4 = ~140wh = 14km of distance or so (~8-9miles)
```

---
## \#16 Posted by: MoeStooge Posted at: 2017-05-19T14:08:40.942Z Reads: 72

```
Like @TeknoAbu pointed out. The trackstar is rated for 8s lipo. He is talking about 10s lion @ 3.6v per cel. So 33v to 36v. My money would be on this working.
```

---
## \#17 Posted by: Okami Posted at: 2017-05-19T14:10:50.462Z Reads: 69

```
3.6v is just nominal and is close to empty already.

More 'usable'' voltage / capacity is at 38-39v or so.

So, he still needs to 'up it' for about 5v.

I would recommend to check whenever esc gets hot and so on, when it works.. though someone who knows about mosfets and how these rc esc work should step in to describe what might actually fail here.
```

---
## \#18 Posted by: MoeStooge Posted at: 2017-05-19T14:13:52.509Z Reads: 63

```
I'm putting up 25$ towards your ESC if you smoke it. In a video . For science 👍
```

---
## \#19 Posted by: TeknoAbu Posted at: 2017-05-19T14:42:40.490Z Reads: 57

```
As @MoeStooge reminds me of here: The battery I'm using is NOT LiPo, and as far as I know, LiPo cells are 4,2V and Li-ion are 3,6V which means, that the difference is technically speaking only 2,4V or...? ...am I completely lost right now?
```

---
## \#20 Posted by: Okami Posted at: 2017-05-19T14:44:45.808Z Reads: 61

```
'Full range of li-ion'' is ~3.0v - 4.2v

For lipo, it is more like ~3.4v - 4.2v)

As said, please take out multi meter while you charge and stop at ~38-39v of battery voltage for your scooter battery.

At max it will be 41-42v which might be already too much.

----
How big is the battery @TeknoAbu ?
```

---
## \#21 Posted by: TeknoAbu Posted at: 2017-05-19T14:48:49.105Z Reads: 57

```
The battery I'm planning on using is a 10S2P Li-ion battery with 4,4Ah. The discharge rate does not seem to be mentioned on the battery itself.
```

---
## \#22 Posted by: Okami Posted at: 2017-05-19T14:51:11.543Z Reads: 55

```
mh, yeh 4.4ah is not the best to work with.. but 3ah might be also okay..

I imagine you might be able to run it at 70-80% of max charge (if I follow the logic of what I posted in 1st thread)..

80% = ~3.5ah
70% = ~3.10 ah..

Still usable and will yield about 10km range at least, if battery is in good shape and if it it even works.

Might not give you the max output, as these are probably not highest output cells I believe.

--

So, not to burn it on 1st try, @TeknoAbu I would suggest you to do this:

If you got voltmeter (u should have one, if you work on esk8 lol).. plug it in parallel with battery terminals while charging, then, when you see 38-39v, stop the charge.. the voltage will go back a volt or two but will later on remain stable.

If you really wanna use the board and dont want to burn the esc, you might as well charge till only 35-36v.

Just check in what condition / state / voltage the battery currently is... maybe it doesnt need any discharging or it is already too high.

--

You probably can charge / leave the battery at 34v but it wont give you a lot of range.. basically at 3.4v battery is at ~25% or so.. so in your case, maybe 1ah of capacity and would probably only work for about 3km or so.
```

---
## \#23 Posted by: TeknoAbu Posted at: 2017-05-19T14:58:50.110Z Reads: 47

```
Right, thank you kindly for the help! I'll follow your instructions, and film it - _for science!_ :smiley:. If the battery is totally unusable, I guess I just have to go and buy myself a battery that actually matches the ESC. :) . If so, what battery should I go with then?
```

---
## \#24 Posted by: MoeStooge Posted at: 2017-05-19T15:03:01.507Z Reads: 45

```
Yuup, @Okami is right and I stand corrected. The LiFeP04 is the 3.6v per cel.  My $25 is still on the table. Partial charge is a great idea. No guts no glory.
```

---
## \#25 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:06:07.946Z Reads: 44

```
You can exceed the max drain-to-source breakdown voltage of the mosfets on the board at which point you will get high current and magic smoke, so saying that voltage is no problem especially in upping the voltage on an 8S designed ESC is silly.

Why not up the battery voltage on the VESC from 12S to 14S? Voltage is no problem right?
```

---
## \#26 Posted by: MoeStooge Posted at: 2017-05-19T15:07:24.070Z Reads: 44

```
I run two 4s 10000mah multistar in series from hobbyking . Easy cheap charging.
```

---
## \#27 Posted by: Okami Posted at: 2017-05-19T15:07:43.070Z Reads: 45

```
@SimosMCmuffin so is there a way to physically inspect and read values to determine how much 'over-voltage' can the mosfets /parts sustain?

I know that one of the limits is probably capacitors itself :D but they usually should be at least a few volts higher right..(?)

--

@MoeStooge thanks for reminding of lifepo, but since he didnt mention it here and I dont believe he has one for escooter (for ebikes more popular) then i didnt even mention it here, yes with lifepo at 10s, it would work quite well actually because of lower voltage but lifepos usually are more expensive, bigger in size / less capacity.
```

---
## \#28 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:22:58.776Z Reads: 43

```
The El.cap voltages are easy to determine of course as they're written on them, but on the MOSFETs you would have to look at the model number on their package and find the datasheet and check what it says for maximum Vdss breakdown voltage.

Here's a datasheet shot for the IRFS7530 MOSFET used in the VESC:
<img src="/uploads/db1493/original/3X/1/4/1456ec1911ec01c171e5f0b78f912aabb435d3a4.jpg" width="690" height="389">
So even the though the VESC's MOSFETs are rated for 60V, the recommended battery voltage is 50.4 V (12S) to give a little overhead.

There is a economic reason why they do use as low Vdss voltage MOSFET as they can, as their component price will quickly start rising the higher current and voltage you go and even then the hobby ESCs use many lower current MOSFET in parallel to raise the max current capability and spread the heat generation over larger area. So an 8S ESC is most likely rated very close to the particular battery voltage.
```

---
## \#29 Posted by: MoeStooge Posted at: 2017-05-19T15:25:44.465Z Reads: 42

```
Trackstar manual says 33.6v max do not exceed.  My $25. Is still good.
```

---
## \#30 Posted by: Maxid Posted at: 2017-05-19T15:30:40.024Z Reads: 40

```
I said 
[quote](usually and in limits)[/quote] 

Slight overvoltages are far less likely to burn anything than slight overcurrent. If you actually exceed any component rating you can obviously destroy them - that should be common sense. The used components are typically a little overspecced however so that they can handle abuse (with voltage spikes and so on). The caps are not rated to 25.2V on a 6S ESC but a little more and so on.
I tried it myself with an 8S LifePo on a 6S ESC - no smoke but OV protection kicked in.
```

---
## \#31 Posted by: Okami Posted at: 2017-05-19T15:34:09.057Z Reads: 37

```
[quote="Maxid, post:30, topic:23450"]
I tried it myself with an 8S LifePo on a 6S ESC - no smoke but OV protection kicked in.
[/quote]

At what voltage was the Lifepo?

3.6 x 8 = 28.8v..

so about 4v more (25.2v - 28.8v = 3.6v precisely, if lifepo was at max or so)
```

---
## \#32 Posted by: MoeStooge Posted at: 2017-05-19T15:34:42.683Z Reads: 34

```
That's a 17% safety factor in the MOSFET.  And would be pushing your ESC 20% over manufacturer limit.  Sounds like fun.
```

---
## \#33 Posted by: Okami Posted at: 2017-05-19T15:37:57.652Z Reads: 37

```
@SimosMCmuffin besides mosfets, are there any other parts which might be 'regulated' and need to be operated in specific voltage?

Then @TeknoAbu could take a photo of his mosfets inside esc after or before he burns it :D though it might as well also give just over voltage error and not run properly, if it is smart enough :slight_smile:

I think someone had posted inside pics of dis-assembled FVT120.. might as well go there and see if mosfet number can be seen there.
```

---
## \#34 Posted by: SimosMCmuffin Posted at: 2017-05-19T15:51:45.240Z Reads: 38

```
Here's the manual for the OP's ESC:
https://hobbyking.com/media/file/885848202X363531X7.pdf

They stress not to use more then 8S voltages.

There are basically 4 parts that might break from the voltage. El.caps, MOSFETs, MOSFET gate drivers or voltage regulator for MCU. There might also be a TVS protection diode to protect from voltage surges/spikes and if you cross that diode's breakdown voltage it will basically short-circuit the battery terminals together and atomize the diode into the atmosphere in a couple milliseconds probably.

Of course the only certain way is to test and see if it works :wink:, but the voltage limits are there for a reason...
```

---
## \#35 Posted by: Okami Posted at: 2017-05-19T15:56:09.706Z Reads: 37

```
Mh, Thanks for clarifying things! TVS diode vaporization sounds fun! :D

Well.. If you saw my first post here, im a bit amazed at castle creations (talon?) esc, that it can still work a few volts higher and just beeps when in overvoltage then again, it is a completely different price group so we cannot be really sure that the esc @TeknoAbu used has any circuits which check the voltage.

I do know some of them check for voltage automatically so maybe they have a setting to sense over-voltage and not drive the mosfets, if the scenario is such.. this is why i recommend him to start slowly and see how the esc responds and not slam it with 8v higher voltage which might be too much in my opinion, otherwise they would rate it to 9s or something.

@SimosMCmuffin from what you said, it sounds like mosfet driver might also be quite prone to this, if it is close to the limit.. we see what happens with vesc and Drv quite a lot.. :D
```

---
## \#36 Posted by: MoeStooge Posted at: 2017-05-23T19:11:46.111Z Reads: 32

```
@TeknoAbu     Smoke, Fire, Cold feet?
```

---
## \#37 Posted by: TeknoAbu Posted at: 2017-06-20T20:07:03.620Z Reads: 30

```
Alright everyone, I have been super-busy with the massive amount of exams just until now, so I'm very sorry that I haven't been able to do something in the recent days.. anyways - update is here!

Just to summarize it all once again, I now tried to connect a 36V Li-Ion battery into my 34V max ESC. Quite simple of a result though. The fact is, that the ESC won't use the battery's power to run the motor. Compared to when I did a quick 14V setup with some old batteries this same day, the motor was running as intended. 

When I plugged the 36V battery in the following happened: 8 light beeps indicating 8 cells, one long deep beep indicating that the transmitter was connected succesfully, and then just the ESC rapidly flashing a red led. No magic smoke or anything (thank god), no hot wires, no hot battery and no power to the motor at all. The ESC just kept on flashing this red color. 

What has happened? Can the ESC actually detect if it's getting overvoltage? If possible, what to do now?
```

---
## \#38 Posted by: MoeStooge Posted at: 2017-06-20T21:44:40.594Z Reads: 30

```
Over Voltage Protection. I was rooting for you. Some of your better equipped ESC have this feature.
```

---
## \#39 Posted by: TeknoAbu Posted at: 2017-06-21T05:33:06.239Z Reads: 29

```
Right, I knew it... 

Do I have any possibilities by this time other than buying a new battery, or can I somehow remove the protection? 

If not, could you suggest a battery (or batteries)  that would fit my skateboard then?
```

---
## \#40 Posted by: MoeStooge Posted at: 2017-06-21T14:50:58.600Z Reads: 25

```
I run two 10000mah 4s in series on my trackstar. You could take apart your battery and re configure your cells if your up for a challenge. My battery cost was around 130usd. Some batt soul searching.
```

---

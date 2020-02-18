# VESC: How to get better brakes?

### Replies: 38 Views: 1385

## \#1 Posted by: Maxid Posted at: 2018-06-20T07:16:58.256Z Reads: 277

```
Hi all,

As most of you probably know by now I got a Lou board with a single hub motor that I upgraded with a Focbox.
I thought that braking would be improved but I still struggle to stop when going downhill or at low speeds.

My initial idea was to increase motor min to -85A and battery min to -10A but it didn't help and looking at the logs I don't even come close to the set values. 
Interestingly the motor current even switches from negative to positive while braking as visible in the attached logs. Is that normal? What setting should I try next to get this thing to stop?

I am using sensored FOC and the battery is a 10S1P. Firmware is the current @Ackmaniac version 3.102 if I remember correctly.

[img]upload://lKRXomOpWwkghhXvQfIWkKEp0kC.jpg[/img]
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-06-20T13:58:17.830Z Reads: 251

```
hm interesting. tat has sensor correct?
```

---
## \#3 Posted by: chocol4te Posted at: 2018-06-20T14:06:34.841Z Reads: 244

```
Even 5A on a 1P battery would be pushing it. Really the only solution is to add more cells in parallel to increase the total charging current.

Have you tried learning to footbrake?
```

---
## \#4 Posted by: Maxid Posted at: 2018-06-20T14:16:18.771Z Reads: 235

```
as you can see in the log my battery min setting is not the issue here. I am not even close to 5A
```

---
## \#5 Posted by: chocol4te Posted at: 2018-06-20T14:49:17.655Z Reads: 220

```
Just like how batteries can only deliver a certain amount of current before voltage drops, batteries can only accept a certain amount of current.
```

---
## \#6 Posted by: Maxid Posted at: 2018-06-20T14:55:44.085Z Reads: 215

```
I know - please be constructive towards the actual issue.
The voltage did not rise above 41V so there is still margin for the cells to take the current.
It also does not explain why the current reverses and becomes positive while braking.
The log shows the overall lowest battery min to be -2.59A and the lowest motor min to be -16.11A.

I don't care about the health of the cells and whats good for them - I would have never decided for a 1P solution anyway. But this is a commercial board that I can only modify so much and a bigger battery is not possible.
```

---
## \#7 Posted by: trampa Posted at: 2018-06-20T15:19:32.604Z Reads: 198

```
Motor min becomes more dominant at slow speed, while the battery min value defines the brakes at speed.
With -10A you don't get a lot of braking. Best way to set up your board with linear braking behavior is to use the same value for both, motor and battery min. The generated energy needs to go somewhere and that is your battery. If you don't allow the energy to shoot towards your battery, you have little to no brakes.

On top of that, your hubs have little (braking)torque.

Frank
```

---
## \#8 Posted by: jadatmag Posted at: 2018-06-20T16:03:31.616Z Reads: 188

```
So if I want to improve my braking on the Raptor 2 at speed; I would need to go from 10s4p to 10s4+p and flash other firmware on the focboxes to bypass the limit of -12A for battery min?

I basically want to be able to skid my wheels at full speed so I have all the control. At slow speeds, the wheels are actually able to skid already.

Can't we bypass the battery for braking and send the energy to bitcoin mining or thin air?
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-06-20T16:08:42.251Z Reads: 178

```
Probably the motor is saturating, you can’t get the current higher than what you are getting no matter the limits

How small is the motor?
```

---
## \#10 Posted by: Maxid Posted at: 2018-06-20T16:18:57.805Z Reads: 175

```
Don't really know - it's stock Lou. Smaller than my Jacob Hubs from the looks of it.
```

---
## \#11 Posted by: Maxid Posted at: 2018-06-21T06:46:51.096Z Reads: 154

```
But why is the current polarity switching? And I can't even reach -3A battery min - even though i set 10A. Why is that?
```

---
## \#12 Posted by: trampa Posted at: 2018-06-21T06:48:54.855Z Reads: 150

```
Are you using VESC-Tool, latest Version?

Frank
```

---
## \#13 Posted by: Maxid Posted at: 2018-06-21T07:00:05.910Z Reads: 150

```
I am using @Ackmaniac's current version (which is basically VESC-Tool)
```

---
## \#14 Posted by: trampa Posted at: 2018-06-21T07:14:46.605Z Reads: 148

```
There is a difference, and maybe now you get why Benjamin implemented the current settings as they are.
If your Amp flow differs greatly from your settings, something is wrong in the code base. 
You would expect that the Amp flow matches your settings, so that you can actually adjust the system correctly, matching your motor and battery and desired brake strength -  which is the case if you use Benjamin's Software/FW. He knows exactly what  he is doing! He coded the thing and has more knowledge about motor control than anyone else. There is a reason why things are the way they are....
All you need to do is flash the original FW and use VESC-Tool, adjust the currents (e.g. -40A motor regen and -25A battery min.). You can adjust the positive and negative ramping (in PPM tab) to get the desired smoothness in the throttle stick/trigger. And if that is not enough, you can use the throttle curves to fine tune things even further. I can get every single board to run smooth like butter. 

Frank
```

---
## \#15 Posted by: Maxid Posted at: 2018-06-21T07:28:07.910Z Reads: 140

```
Alright let's see if this really is a firmware issue. I will flash the original version and try again.
```

---
## \#16 Posted by: Ackmaniac Posted at: 2018-06-21T07:42:22.738Z Reads: 135

```
A video with the app where you do your braking tests would be very helpful. Then you can do another video with the original firmware.

What i can see so far is that in the attached picture the speed was relatively low. Guess your motor isn't a good  generators. And volts are also not visible in the graph. So a video would really help.

@trampa you think it is wise to recommend -25A battery min for a 10S1P battery?
```

---
## \#17 Posted by: trampa Posted at: 2018-06-21T08:18:28.707Z Reads: 137

```
If you want to figure out the brake settings, you need to know the exact Amp flow at a desired brake strength.
If the Battery can't handle the Amp flow for a couple of seconds, but you need the brake strength for safety, you need to work on the battery (e.g. use stronger/better cells, higher P count), or accept that the brakes are not good enough for a safe ride. The braking energy needs to go somewhere and that is the battery.  VESC-Tool will operate with the current you set. So it's quite easy to adjust things to match your battery strength or desired brake strength. In the end it comes down to hardware limitations. Usually the battery is the weakest link in the chain when it comes to braking strength. This is why we all run high P counts on our boards. 
If a manufacturer sells boards with a 1P battery setups, he either accepts that the battery is operated outside it's physical limits (creating a risk), or he accepts that the board doesn't have good brakes (creating a risk). 
This is typical for designs aiming at a certain sales price point. Technically wrong solutions are accepted to meet the pre-set sales price point, no matter of the outcome. It's all about bullshit marketing and fooling people around. 

Advertised top speed for the dual drive: 35Km/h, Battery is 36V , 3000mAh (1P), Power output 3KW
Obviously something is wrong with this product!
```

---
## \#18 Posted by: lrdesigns Posted at: 2018-06-21T08:22:58.788Z Reads: 131

```
[quote="Maxid, post:6, topic:59461"]
The log shows the overall lowest battery min to be -2.59A and the lowest motor min to be -16.11A.
[/quote]

My conclusion is that this is as much regen that this little motor can make. On my belted system if I downsize the motor pulley 2 teeth I get a noticeable increase in breaking power. So small motor with 1:1 ratio I don't have much hope. Sorry. 

Good luck with the software testing, I would be happy for you if I'm proven wrong.
```

---
## \#19 Posted by: Maxid Posted at: 2018-06-21T08:56:08.667Z Reads: 126

```
Well I'd be glad if it is in fact "just" a motor issue. But the current polarity thing bothers me and seems counterintuitive for me regardless of motor size or gearing ratio. As long as I brake I expect to generate current and have negative battery current. It might be low but it shouldn't become positive no?
```

---
## \#20 Posted by: Maxid Posted at: 2018-06-21T08:58:10.507Z Reads: 125

```
I can send you the logs or a video. But the Lou is not that stable at high speeds and I did not feel comfortable holding my phone up while doing full-stop brake tests. I did not post the full log simply because of the enclosed GPS location data. It's already illegal here so no need to push my luck ;)

Voltage wise the log shows no increase above 41V.
```

---
## \#21 Posted by: lrdesigns Posted at: 2018-06-21T09:14:06.718Z Reads: 117

```
[quote="Maxid, post:19, topic:59461"]
It might be low but it shouldn’t become positive no?
[/quote]

Yeah I think that is really weird. I got no good ideas to explain that.
```

---
## \#22 Posted by: Ackmaniac Posted at: 2018-06-21T10:30:50.903Z Reads: 110

```
When the motor becomes too slow to generate power the Vesc applies power to hold the motor. That happens when the motors duty cycle goes below 3%. Because at these low speeds the regenerative power would be so low that the brakes would have no effect.

@Maxid does the battery have a BMS?
```

---
## \#23 Posted by: Maxid Posted at: 2018-06-21T10:44:19.918Z Reads: 109

```
There is a PCB inside yes. But I guess it is charge only.
[img]upload://hv1kHQhn27iqNrMYQCeQfajHvng.jpg[/img]
```

---
## \#24 Posted by: Ackmaniac Posted at: 2018-06-21T10:55:14.125Z Reads: 105

```
These are awful cells for electric longboards. Specs say Max discharge 10A and max charge 2A.
But anyway for the moment my best guess is that the motors don't generate more power at these low speeds with that you tested it. Or the BMS shuts down and the voltage rises too high.
In 3.102 there is a feature that starts to reduce the brake current when the voltage is 1V belo the max voltage (57V by default).
Maybe you can send me the logs.
```

---
## \#25 Posted by: Benjamin899 Posted at: 2018-06-21T11:05:49.362Z Reads: 104

```
holy...someone rly used these in a skateboard, let alone 1p...wtf...even the LG HE2 are better and cheaper.
```

---
## \#26 Posted by: trampa Posted at: 2018-06-21T11:07:13.291Z Reads: 105

```
A tragic product.... 
Even if their motors would output half of the advertised rating, they would still drain 40A from a 10A rated battery. That is unscrupulous product design.
```

---
## \#27 Posted by: taz Posted at: 2018-06-21T11:11:28.825Z Reads: 105

```
These are quality cells. Panasonic NCR18650PF.
I have no idea why someone would use them on an eskate though as they are low current and not that cheap.
```

---
## \#28 Posted by: Maxid Posted at: 2018-06-21T11:24:04.078Z Reads: 104

```
Nobody knows - I am thinking of upgrading to 30Q but want to figure this behavior out first. These cells are also the reason why I said earlier that I don't care about their health.
```

---
## \#30 Posted by: Maxid Posted at: 2018-06-21T11:45:20.453Z Reads: 98

```
No since the battery min is not the issue here. the battery could take more energy (easily double of what it currently does) but the motor is not delivering that energy.
```

---
## \#31 Posted by: Sn4pz Posted at: 2018-06-21T11:46:02.482Z Reads: 95

```
oh, thanks for the explanation :)
```

---
## \#32 Posted by: lrdesigns Posted at: 2018-06-21T11:47:52.329Z Reads: 98

```
Not in this case, the motor creates the breaking force, then you can reduce this with vesc settings to be the max safe level for your battery. If your motor does not create enough back voltage changing the battery will make no difference.

In most of the diy setups on this forum the limiting factor is the battery charge rate. Large dual motors with gear reduction.
```

---
## \#33 Posted by: SimosMCmuffin Posted at: 2018-06-21T11:53:50.058Z Reads: 96

```
[quote="Ackmaniac, post:22, topic:59461"]
the Vesc applies power to hold the motor
[/quote]

Doesn't the VESC short-circuit the motor once the motor's ERPM drops below the configured ERPM level, to get that last intense brake at near stopping speed? I'm pretty sure it justs puts all low-side FETs on in that point. So it isn't actually using any power, as it's just recirculating the motor's EMF back to itself. Same effect as trying to turn a motor by hand while short-circuiting the phase wires together. This is not the same as trying to drive the motor in reverse.
```

---
## \#34 Posted by: Ackmaniac Posted at: 2018-06-21T12:00:50.586Z Reads: 92

```
And the current sensors detect this and that's what is visible in the logs as positive current at braking.
```

---
## \#35 Posted by: SimosMCmuffin Posted at: 2018-06-21T12:08:52.119Z Reads: 90

```
I suppose this is on the 4.xx HW? With it's low-side current shunts. on 6.xx HW they're high-side shunts.
```

---
## \#36 Posted by: Maxid Posted at: 2018-06-21T13:25:21.223Z Reads: 83

```
Yeah it's a Focbox so 4.12 based
```

---
## \#37 Posted by: uTZFu Posted at: 2019-10-16T22:24:34.389Z Reads: 23

```
Hey maxid - out of curiosity and since I ran into a very similar challenge (same vesc with Lou 1.0 single hub): could you increase your breaking torque by changing to the 30Qs significantly despite the challenge of the vesc not pushing the maximum current back to the batteries while braking? I wanted to test a 6s2P Lipo Setup next to see if higher current draw abilities does improve braking in my setup. Thanks in advance!
```

---
## \#38 Posted by: Maxid Posted at: 2019-10-17T19:41:11.304Z Reads: 17

```
I did not go the 30q route but changed the setup to a belt drive (my commute is/was uphill and the gearing just made sense)
```

---
## \#39 Posted by: uTZFu Posted at: 2019-10-17T20:17:02.845Z Reads: 16

```
Thanks mate! Guess I will need to test with the Lipos then to see if there is any effect - belt drive is an option I considered too - just wanted to try to keep the stealth look first with less maintenance :-)
```

---

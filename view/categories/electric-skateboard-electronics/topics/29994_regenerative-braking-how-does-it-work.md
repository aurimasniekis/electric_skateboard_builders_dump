# Regenerative Braking - How does it work?

### Replies: 39 Views: 5870

## \#1 Posted by: taycro Posted at: 2017-08-07T22:03:59.697Z Reads: 393

```
I am fairly new to the ESK8 community and I am working on building my first board. I have heard many things about regenerative breaking but I can't figure out how it works or how to incorporate it into a board.

Can anyone help me better understand how regenerative breaking works? I would really love to have it on my board.

Thanks for reading this. I could really use some help.
```

---
## \#2 Posted by: Decdog Posted at: 2017-08-07T22:15:09.243Z Reads: 391

```
http://www.electric-skateboard.builders/t/vesc-faq-regen-braking-configuration-bldc-tool-brake-force/353
```

---
## \#3 Posted by: Martinsp Posted at: 2017-08-07T22:15:14.452Z Reads: 386

```
You set it in the BLDC tool. There is a "battery min (regen)" that is a setting in Amps and you set the maximum Amps that you want your board to charge the battery when you break. You can set it to 0 and pretty much disable it I think but I have never try it so dont take my word for it.
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-07T22:15:16.174Z Reads: 373

```
Depends if the ESC supports it. The VESC and all its iterations do. If BEMF voltage generated overcomes battery voltage, current will flow into the pack as you brake. The amount of current is controlled by the Battery Min value on BLDC tool.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-08-07T22:42:35.199Z Reads: 350

```
So the voltage created while breaking has to be greater than the present voltage of the battery or it will not regenerate the battery?
If there was a way to control the BEMF voltage, then you could prevent regen braking from trying to overcharge the battery. Especially at lower pack voltages like 8s and 6s
```

---
## \#6 Posted by: Jinra Posted at: 2017-08-07T22:49:39.145Z Reads: 331

```
I think this would be achievable with a more advanced bms, but I'm no EE. if you could apply bemf voltage toward a lower S count you could theoretically regen at slower speeds as well.
```

---
## \#7 Posted by: gee Posted at: 2017-08-07T23:24:20.760Z Reads: 316

```
hmm I always wonder this. Let's say you got two lipo batteries in series with NO BMS and 80% charged. You started from the top of a mountain let's say. Does going down hill BALANCE charges your battery to 100%? I'm scared to go downhill because I don't have an bms and I don't know if it will mess up my battery voltage.
```

---
## \#8 Posted by: Jinra Posted at: 2017-08-07T23:26:24.826Z Reads: 294

```
If you're discharging through BMS it should balance charge if you're hitting the balance voltage (upper 4.1x volts), but honestly I don't see it drifting much at all during a single cycle. If it is drifting much, you probably have high resistance in one of the cell groups which indicates an issue with the cell and it should probably be replaced.

If you're bypassing discharging you won't be balance charging at all.
```

---
## \#9 Posted by: gee Posted at: 2017-08-07T23:35:59.024Z Reads: 282

```
So anyone without a BMS trying to go down a long hill should be careful because it doesn't balance charged is what you're saying?
```

---
## \#10 Posted by: solidgeek Posted at: 2017-08-07T23:39:23.230Z Reads: 278

```
As far as I understand the only advantage of discharging through a BMS is the max current safety it provides. If you bypass the discharging, and current runs back to charge the battery pack (regen), the BMS will balance out everything, as long as the charge connection is connected. Am I wrong?
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-07T23:44:02.865Z Reads: 269

```
Not at all, I'm saying cells don't really drift much during a single charge cycle, with or without BMS. You should be fine with the balance, unless something is wrong with a cell/cell group.

@solidgeek BMS's don't actively balance the pack as you go, meaning if you hooked up a 2s BMS to two cells, one at 3.8v and one at 4.0v it won't do anything. Each cell will stay at their respective voltage until you do a full charge on the 2s pack.
```

---
## \#12 Posted by: SilentException Posted at: 2017-08-08T13:08:43.164Z Reads: 250

```
Couple of thins are still unclear to me regarding this.

BMS has a separate charge and discharge port. When VESC pushes back during braking you're basically using discharge port to "charge". Not sure how the BMS copes with this? Does it even charge the battery?

Where is the VESC setting that prevents overcharge? Is that Maximum input voltage? Because I've heard that it is not good to touch that setting. On the other hand, blasting 57V to 6S pack would not do much good..
```

---
## \#13 Posted by: chaka Posted at: 2017-08-08T13:13:42.257Z Reads: 232

```
The best reason to use a BMS for discharge is it can shut your board down before dropping the voltage too low. Some builders are bypassing and using a simple in rush/controller switch but this can be dangerous for the battery if you get absent minded and continue to ride or forget to turn your board off.
```

---
## \#14 Posted by: Randyc1 Posted at: 2017-08-09T04:29:58.338Z Reads: 207

```
Does'nt the vesc do the same at the V we set  ?
```

---
## \#15 Posted by: chaka Posted at: 2017-08-09T04:45:51.286Z Reads: 202

```
No, it only disables the throttle/limp mode. The power will still be on and the system will continue to draw a small amount of power from the battery.
```

---
## \#16 Posted by: Silverline Posted at: 2017-08-09T05:37:45.892Z Reads: 196

```
What happens if you hit the bat max, during braking down a Hill ? Then the brakes stop working right ?
```

---
## \#17 Posted by: Jinra Posted at: 2017-08-09T05:59:04.858Z Reads: 196

```
Battery and motor min are the attributes for braking, and it depends on your BMS and whether or not  your discharging through it. Most BMS's backoff strategy is simply cut the load which will kill power to your VESC. If you're bypassing, the VESC doesn't know what "battery full" means and will simply keep dumping excess current into your battery if it's full and if your BEMF voltage is higher than the pack voltage.
```

---
## \#18 Posted by: Silverline Posted at: 2017-08-09T08:48:13.018Z Reads: 181

```
Let me put my question this way. I plan to use my bestech bms (80a) for both charging and load. Then if i have a fully charged battery , and starting on top of a Hill, and braking the entire time down the Hill, i would under normal circumstances with bypassd bms and voltage max at default 57v (i'm running 10s) going to overcharge my batteries right ? But because i use my bestech as the 'load' All so, the BMS would cut of and protect my batteries while i'm still being able to brake right ?
```

---
## \#19 Posted by: SilentException Posted at: 2017-08-09T09:10:35.858Z Reads: 173

```
I asked similar questions above but no one answered. First, it is questionable if BMS will even charge because you're essentially charging through discharge port. BesTech BMS' have separate charging port.
```

---
## \#20 Posted by: Jebe Posted at: 2017-08-09T11:24:36.490Z Reads: 165

```
Will charge but not balance charge.
```

---
## \#21 Posted by: rok Posted at: 2017-08-09T11:31:57.788Z Reads: 160

```
If i bypass BMS for discharging, does that mean my battery will get charged with regenerative braking but BMS won't balance the cells? In this case, is it better if i just set regen to 0?
```

---
## \#22 Posted by: SilentException Posted at: 2017-08-09T11:44:42.031Z Reads: 157

```
In that case I can only wonder what happens when you push for example 50V back through discharge port to the fully charged battery.
```

---
## \#23 Posted by: Jinra Posted at: 2017-08-09T13:16:34.588Z Reads: 156

```
if you're going faster than max speed of your board down the hill, yes you'll be overcharging while braking. If your bms cuts off power you may be without brakes going down.
```

---
## \#24 Posted by: PiratFPV Posted at: 2018-08-17T10:42:37.797Z Reads: 94

```
I noticed on VESC 6.6 that to have breaks I have to increase amperage in " Battery current max regan " otherwise break are not working , even if I got -60A at " Motor current max Break "
So how can I set breaks without recharging battery ?
```

---
## \#25 Posted by: mishrasubhransu Posted at: 2018-12-05T19:11:24.836Z Reads: 77

```
I had the exact though the other day. 
Say we have a 10S battery which is ~37 volts around the time of the ride
Say we have a 100KV motor
when we are riding it, the max rpm of the motor is 3700 RPM. Now lets just cost with no power to the motor. That 3700 RPM is going to produce a back emf of 37Volts, So when we braking under regen we "rectify"(because it's sinusoidal) that bemf and feed it to the battery. But the thing is, that 37 volt won't charge the battery. It has to be higher voltage. Unless VESC has a charge pump to increase that voltage to something higher. Does it?

So how does it exactly work?
```

---
## \#26 Posted by: mishrasubhransu Posted at: 2018-12-05T19:43:12.864Z Reads: 78

```
Okay, so it turns out there is a charge pump because the motor winding is itself an inductor. When you short and unshort the motor it produces a voltage higher than the backemf(due to motor rotation), now this higher voltage is rectified and used to charge the battery.  When this switching is going on 2 things happen:
1. When you short the motor you are doing non regen braking,
2. When you un-short the motor you are doing regen braking
Of course the regen braking only works when the bemf + induction spike > battery voltage.

From wikipedia:
"The key principle that drives the boost converter is the tendency of an [inductor](https://en.wikipedia.org/wiki/Inductor) to resist changes in current by creating and destroying a magnetic field. In a boost converter, the output voltage is always higher than the input voltage. A schematic of a boost power stage is shown in Figure 1.

(a) When the switch is closed, current flows through the inductor in clockwise direction and the inductor stores some energy by generating a magnetic field. Polarity of the left side of the inductor is positive.

(b) When the switch is opened, current will be reduced as the impedance is higher. The magnetic field previously created will be destroyed to maintain the current towards the load. Thus the polarity will be reversed (means left side of inductor will be negative now). As a result, two sources will be in series causing a higher voltage to charge the capacitor through the diode D.

If the switch is cycled fast enough, the inductor will not discharge fully in between charging stages, and the load will always see a voltage greater than that of the input source alone when the switch is opened. Also while the switch is opened, the capacitor in parallel with the load is charged to this combined voltage. When the switch is then closed and the right hand side is shorted out from the left hand side, the capacitor is therefore able to provide the voltage and energy to the load. During this time, the blocking diode prevents the capacitor from discharging through the switch. The switch must of course be opened again fast enough to prevent the capacitor from discharging too much."
![image|250x262](upload://1XCO7ZKcWDIchmVOsOKirFrvOaz.png) 

https://en.wikipedia.org/wiki/Boost_converter
```

---
## \#27 Posted by: sayekim Posted at: 2018-12-06T10:52:30.999Z Reads: 62

```
You break something, then it regenerates and then you break it again and it regenerates again. This would be the future. 

@b264 I fixed the title for you.

Who am I kidding. I did it for me.
```

---
## \#28 Posted by: SkateYS Posted at: 2019-01-30T20:57:08.378Z Reads: 47

```
Does anyone knows an effective way to disable regenerative breaking??? I'm using FOCbox!
```

---
## \#29 Posted by: Hummie Posted at: 2019-01-30T21:03:38.602Z Reads: 44

```
So u can brake without charging by shorting or is it just part of the regen process at high speed..it seems. u need to do regen to brake as the energy has to go somewhere.
While there all kinds of bms typically people use the discharge type where if a cell goes over a set voltage,maybe 4.2, then that cell alone is discharged super slow with a resistor.  Whether you’re braking or charging will be the same mechanism for balancing
```

---
## \#30 Posted by: linsus Posted at: 2019-01-30T21:10:54.085Z Reads: 39

```
Why the hell would you want to disable the brake?..and dont give me that crap that it puts your pack out of balance.
```

---
## \#31 Posted by: mishrasubhransu Posted at: 2019-01-30T21:32:08.199Z Reads: 42

```
I don't recommend doing this, because energy is purely wasted as heat in the motor winding and the mosfets but basically you decrease the battery reverse current.
```

---
## \#32 Posted by: mishrasubhransu Posted at: 2019-01-30T21:33:33.843Z Reads: 41

```
Yeah, you can brake without regen. Set your battery reverse current to 0 Amps. But that means increased heat in motors and mosfets.
```

---
## \#33 Posted by: SkateYS Posted at: 2019-01-30T21:34:30.183Z Reads: 39

```
😂come on body! I'm trying to see if my cells will still go unbalanced without that regenerative thing! This sh*t still happens on my brain new lipo Pack! I already can't charge it all the way anymore 🤷‍♂️
```

---
## \#34 Posted by: linsus Posted at: 2019-01-30T22:05:38.644Z Reads: 37

```
sounds more like a bad bms/charger issue then anything to do with the brakes
```

---
## \#35 Posted by: Hummie Posted at: 2019-01-30T22:10:29.665Z Reads: 36

```
U put each cell up to a multimeter? But I didn’t read the thread! That’s be my start

Not using the regen you wouldn’t be involved with the battery. No regeneration of energy back to battery

A video of u showing us would get to the bottom
```

---
## \#36 Posted by: Hummie Posted at: 2019-01-30T22:15:58.560Z Reads: 37

```
What would produce highest regen?

Wouldn’t it be a huge amount of heat produced without regen and kill fets quickly? I heard that somewhere but though it was assumed we were always regaining as much as possible. 

Would having a motor’s waveform more a certain shape better to suit the esc get better regen?
```

---
## \#37 Posted by: mishrasubhransu Posted at: 2019-01-30T22:21:25.482Z Reads: 35

```
Braking at high speed, low battery voltage and having a large regen battery current.

But of course you know that setting too high of a regen battery current would damage the battery. That too high of a current depends on battery type and cells in parallel.
```

---
## \#38 Posted by: Hummie Posted at: 2019-01-30T22:26:04.459Z Reads: 37

```
[quote="mishrasubhransu, post:37, topic:29994"]
Braking at high speed, low battery voltage and having a large regen battery current.
[/quote]

I’m forgetting the name but how does setting the motor brake current effect regen?
```

---
## \#39 Posted by: mishrasubhransu Posted at: 2019-01-30T22:32:18.028Z Reads: 37

```
The motor braking current is directly proportional to the braking force as long as the temperature limits and the regen limits are not hit. 

If you set that low, you'll have weak braking.
```

---

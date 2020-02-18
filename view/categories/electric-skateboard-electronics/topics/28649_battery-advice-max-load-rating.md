# Battery Advice &ndash; max load rating

### Replies: 20 Views: 1484

## \#1 Posted by: HunterC Posted at: 2017-07-26T02:05:34.620Z Reads: 134

```
I'm going to get this 192 kv motor -- https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us -- but I'm not sure on a battery.
I found this one -- https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html1 -- It seems good, but won't it surpass the max load rating on the motor?

Thanks for the help.
```

---
## \#2 Posted by: SORRENTINO Posted at: 2017-07-26T02:17:31.049Z Reads: 133

```
I have the Zippy 5000mah 5s 40c. I think they are about a few bucks more but they are definitely a better buy then those 20c lipos.
```

---
## \#3 Posted by: SORRENTINO Posted at: 2017-07-26T02:18:00.398Z Reads: 130

```
https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-40c.html
```

---
## \#4 Posted by: HunterC Posted at: 2017-07-26T02:22:15.709Z Reads: 128

```
The max load on the motor I chose is 80A. Doesn't that battery also surpass the max load? What motor do you use?
```

---
## \#5 Posted by: wafflejock Posted at: 2017-07-26T02:25:09.644Z Reads: 122

```
Full potential of the battery isn't ever hit (ideally) the ESC will control how much power flows to the motor based on the throttle input, basically you want the battery rated for higher amperage than the ESC and the ESC to be rated for higher amperage and voltage than the motor.  If the ESC tries to draw more power than the batteries can deliver they will heat from their internal resistance and create more voltage sag and eventually would burn up.

With batteries typically you can't go above 12S in terms of voltage (50V) because the components on the ESC can't handle higher voltage.  At some point if you push too many amps through the motor coils they will overheat the motor but so long as you stay in the rated voltage for the motor it won't pull more amps than it can handle (assuming it has airflow around it and isn't being pushed to it's limits)
```

---
## \#6 Posted by: SORRENTINO Posted at: 2017-07-26T02:28:43.077Z Reads: 118

```
Yes the battery does surpass the motor max amps. I have the sk3 149kv motor. I just suggested the zippy 5000mah 40c because it has a higher c rating then the ones you posted and few a few bucks more I think they are worth it. A better battery with better matched cells and lower IR will last longer down the road. That is why I suggested the zippy.
```

---
## \#7 Posted by: HunterC Posted at: 2017-07-26T02:34:35.724Z Reads: 110

```
Alright, thanks. So then would you say that this is a good trio? -- motor  https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html?___store=en_us -- VESC diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/ -- battery  https://hobbyking.com/en_us/turnigy-5000mah-5s-20c-lipo-pack.html1
```

---
## \#8 Posted by: nalviggi Posted at: 2017-07-26T03:05:16.648Z Reads: 105

```
Hi so I am building my first electric skateboard and I have a few questions. First so I have the battery (http://www.ebay.com/itm/222573838441) and I want to know how I connect it to the VESC and then to the motor. I think I need a VESC male to male connector for the 2.4 ghz remote but do I need connectors from the battery to the VESC and then the VESC to the motor? My motor is 190 kv and is linked below. Please let me know what you guys think and thanks for your help!

Motor: diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355-190kv/
```

---
## \#9 Posted by: wafflejock Posted at: 2017-07-26T03:41:53.089Z Reads: 92

```
Yup looks fine you can double up those 5S to make a 10S that's the same setup I have except only 149kv sk3 motor otherwise the same.  5S by itself is pretty low voltage which means you need relatively high amperage to achieve the same wattage (power) so typically better to go as high voltage as your comfortable with use the esk8 calc to see what kind of top end you'll likely get given your chosen parts.  Believe the estimate is 10Wh = 1km so 5S*3.7*5Ah=92.5Wh or about 9.2km or about 5.5miles.  At 10S with 5Ah I can get over 12 miles on flat.
```

---
## \#10 Posted by: Namasaki Posted at: 2017-07-26T03:42:19.562Z Reads: 88

```
[quote="HunterC, post:7, topic:28649"]
Alright, thanks. So then would you say that this is a good trio?
[/quote]


20C is weak, you would be much better off taking @SORRENTINO advice and getting the 40C.
And you are planning to run two 5s batteries in series for 10s correct?
Because 6s is really the minimum for E-boards.
12s is the max
10s is what many would call the sweet spot.
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-26T03:43:45.913Z Reads: 79

```
Just got my metr Bluetooth modules so will have some actual data with these soon but seem to be fine to me so far but definitely doesn't hurt to go higher with the max discharge on the batteries.
```

---
## \#12 Posted by: HunterC Posted at: 2017-07-26T03:45:17.647Z Reads: 76

```
yes, I plan on having 20 wired in series for a 10s. I didn't plan on getting the 40c or anything higher than 20c because I thought it would be over the max loading for the motor.
```

---
## \#13 Posted by: HunterC Posted at: 2017-07-26T03:50:58.810Z Reads: 73

```
Thanks a lot for your help, I have been caught on this for a while. Most of the advice I have gotten has been pretty ineffectual. 
One last thing, Namasaki & SORRENTINO advised to go for battery with 40C rating, because 20C would be too weak, would you agree?
```

---
## \#14 Posted by: Namasaki Posted at: 2017-07-26T03:52:34.009Z Reads: 73

```
You have the wrong idea.
The battery does not determine how much current flows through the system.
Neither does the motor.
The Vesc determines how much current goes to the motor and how much current is pulled from the battery.
If the battery is ratted for a lot more current than you pull from it, then it will not have to work as hard.
it will stay cooler and last longer and the voltage will sag less.
```

---
## \#15 Posted by: wafflejock Posted at: 2017-07-26T03:56:53.245Z Reads: 65

```
Yup higher c rating just means more overhead like @Namasaki just wrote up higher C means can handle more amps drawn from the battery without overheating or stressing the cells basically higher is better (too low can be dangerous but can't be too high on the supply side, problem is only if the ESC draws more to drive the motor than the battery can supply)
```

---
## \#16 Posted by: HunterC Posted at: 2017-07-26T04:05:41.810Z Reads: 62

```
I understand that fine, but I also don't want to burn out the VESC. I was under the impression that since the VESC does limit the current that pulses through the motor, having a battery with a greater discharge output would wear the VESC quicker.
```

---
## \#17 Posted by: Namasaki Posted at: 2017-07-26T04:18:25.164Z Reads: 62

```
[quote="HunterC, post:16, topic:28649, full:true"]
I understand that fine, but I also don't want to burn out the VESC. I was under the impression that since the VESC does limit the current that pulses through the motor, having a battery with a greater discharge output would wear the VESC quicker.
[/quote]


Having a battery capable of high current output will absolutely NOT wear out the Vesc or anything else.
My builds have Lipos that are 5000mah / 60C-120C

Think of your battery as being like your bank account.  Having a lot more battery than you need is just like having a lot more money than you need.

The battery is basically your E-board's bank.

Oh, and the Vesc doesn't just control current to the motor, it also controls current flow from the battery.
And the battery does not output current. Current is drawn out of the battery by the Vesc.
```

---
## \#18 Posted by: HunterC Posted at: 2017-07-26T04:21:31.490Z Reads: 61

```
Okay, I see. I imagine you only have that problem when your motor pulls more than the ESC can handle.
Thanks for the advice guys. @wafflejock @Namasaki
```

---
## \#19 Posted by: Namasaki Posted at: 2017-07-26T04:24:16.018Z Reads: 66

```
[quote="HunterC, post:18, topic:28649"]
Okay, I see. I imagine you only have that problem when your motor pulls more than the ESC can handle.
[/quote]

Here is where the Vesc outshines conventional Esc's
The Vesc in current control mode, controls how much is drawn from the battery and how much goes to the motor. Then the motor will only use what the Vesc allows.
Conventional Esc's are not so.

I guess you could say that the Vesc is not just a motor controller, It's a complete system controller.
And you the operator choose all the current limits in the software settings (BLDC Tool)
```

---
## \#20 Posted by: wafflejock Posted at: 2017-07-26T04:44:16.881Z Reads: 61

```
Read some build threads to get an idea of how people wire things and what connectors they use in general bullet connectors or xt-90 or xt-60 are common connectors used beware different diameter bullet connectors.  If comfortable with soldering and electronics can just solder some things directly as well like the motor to the vesc.  If you still have questions after reading for a bit make a new topic but all the basics are here use the search.
```

---

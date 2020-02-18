# Downsides of High kV Motors?

### Replies: 29 Views: 4886

## \#1 Posted by: NickTheDude Posted at: 2016-10-10T00:25:40.237Z Reads: 393

```
So after looking at @VladPomogaev's data on watt usage, it seemed like the potential wattage of the motors we are using is much higher than it has to be. So I went looking and found a 5045 450kV Turnigy SK3, and it was rated at 1260 watts. From what I've seen 1260 should be enough, especially if you are running dual motors.

Using the esk8 calculator, I found that if you use a 6s li-ion pack, and a 40:12 gearing ratio, you would be able to hit a weighted top speed of 40km/h. 

Since you'd be running 6s, you would have more space to run cells in parallel, helping solve issues with low discharge rates of li-ions. Also lower discharge li-ions have higher capacities.

Also, since BLDC motors have higher efficiency when they are at higher rpms, the large reduction ratio helps the system be more efficient.

As far as I can tell the only thing stopping something like this from working is the ESC. However I've heard the VESC v6 will be able to accommodate much higher kV motors as well as higher current.

So what gives? Why does high voltage/low kV seem to be the standard for high performance boards? It seems like we could be lowering the cost and weight of our boards with this kind of setup. Or am I missing something?
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-10T00:29:12.503Z Reads: 385

```
Higher kv motors tend to have less copper in the stator, which in turns means less power/torque. Higher voltage leads to less amp draw and better efficiency due to less energy lost through heat. That's why high voltage + lower kv is a good combo for this hobby.
```

---
## \#3 Posted by: Hillso Posted at: 2016-10-10T02:06:19.141Z Reads: 371

```
does high kv motors always tend to have less copper in the stator? or you mean smaller motors tend to have less copper in them? I say that because low kv motors have more turns so the wires are thinner so there is higher resistance so higher heat. for example, look at the resistance, max amps and watt values of these two motors: http://www.hobbyking.com/hobbyking/store/__18184__Turnigy_Aerodrive_SK3_6374_149kv_Brushless_Outrunner_Motor.html
http://www.hobbyking.com/hobbyking/store/__18129__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor.html

@NickTheDude I think 40:12 gearing ratio might be problematic because you have small contact area between the belt and the motor pulley. may be fixed with a tensioner.
I think that generaly low kv motors are more effecient, because they have lower resistance, for example, look at big and heavy are bicycle hub motors that are less powerfull than rc motors.
```

---
## \#4 Posted by: VladPomogaev Posted at: 2016-10-10T02:33:05.172Z Reads: 331

```
Jinra nailed it. Also, keep in mind that my power consumption tests were done on perfectly flat land. 

In order to go up a hill, your power consumption increases according to W = mass x acceleration due to gravity x speed of climb + regular power consumption at a certain speed. Meaning that in order to climb a 10m hill in ~20 seconds, the average person would be pulling an **additional** 343 watts, on top of the power they use to move along that hill. Since motors and ESCs are not 100% efficient, the actual power consumption is even greater.

Once again, that's why cheap boards use low powered motors, it's because they can't go up hills. Also, @Hillso is right, there's a limit to how much you can bend a belt (or chain) while keeping the grip and not destroying the belt in the process.
```

---
## \#5 Posted by: irexjr Posted at: 2016-10-10T03:59:55.529Z Reads: 297

```
Why are the motors we use between 150kv and 300kv but then there is a whole area of motors which are like 2000kv +?

Why such the big jump in KV and what could those 2500kv motors potentially provide over lower kv like 200kv. (My local RC shop only sells 1000kv+ motors)
```

---
## \#6 Posted by: Jinra Posted at: 2016-10-10T04:03:51.852Z Reads: 286

```
higher kv motors are used for planes/heli's. They need a lot of rpm per volt since they use less batteries due to weight limitations. There's not nearly as much resistance to spin a propeller vs propel a human.
```

---
## \#7 Posted by: NickTheDude Posted at: 2016-10-10T04:30:51.555Z Reads: 280

```
So if you had two boards, one with the 149kV motor, and the other with the 192kV motor, and they were both geared for the same top speed, would they not have identical performance?

The reason I think that a high kV motor would be more efficient is because of the graph below. Is the heat lost from the higher amp draw is enough to cancel out the gain in efficiency that comes with higher RPM?
http://static.micromo.com/media/wysiwyg/Motor_calculations_graph1.png
```

---
## \#8 Posted by: Jinra Posted at: 2016-10-10T04:35:47.646Z Reads: 265

```
Higher RPM may be more efficient if you were going a constant speed. However, with esk8, you're constantly slowing down and speeding up. The longer you spend overcoming resistanc, the more amps you pull and the worse your efficiency. Not to mention, high speeds run into a lot of resistance which will increase current draw exponentially.
```

---
## \#9 Posted by: NickTheDude Posted at: 2016-10-10T04:45:48.387Z Reads: 257

```
Does that not apply to both high and low kV motors though? Or does the relationship between amp draw and efficiency get worse as you increase kV?
```

---
## \#10 Posted by: Jinra Posted at: 2016-10-10T04:48:08.185Z Reads: 253

```
Well, like I said earlier, higher kv motors tend to have less copper due to the thicker windings. You can't fit as much copper in there with big windings, much easier to fit more copper with thinner windings, which result in lower kv. More copper = more torque = gets you up to speed faster. 

You can try accelerating or going up hills with a high kv motor, but I doubt you'll get up to speed in a reasonable time, assuming your motor or esc doesn't burn out first.
```

---
## \#11 Posted by: NickTheDude Posted at: 2016-10-10T04:54:19.291Z Reads: 243

```
Isn't the lower torque compensated for by the gearing though? I get that the higher kV motors tend to have less copper, but in the examples @Hillso had, the higher kV motor is listed as having a higher wattage than the lower one.
```

---
## \#12 Posted by: Jinra Posted at: 2016-10-10T04:56:10.579Z Reads: 234

```
There are a bunch of things that affect torque to varying degrees. While gearing is important, motor size (ie copper content) is more so.
```

---
## \#13 Posted by: Hummie Posted at: 2016-10-10T14:58:04.323Z Reads: 218

```
U can get the same copper in regardless of kv.  If anything you should be able to get more in with higher kv as it needs less turns so less insulation but it's splitting hairs.   Most manufacturers use multistrand copper and many windings in parallel so don't have to bend a big wire.  If u did bend a big wire instead of the multistrand you could get a motor with lower resistance to inductance and more copper and a better motor. 

A motor can put out the same power regardless of the kv.  Running a high kv and fewer volts and more amps is just as good as long as the esc can do it and your battery wires are thicker.  You get the same torque to heat ratio in the motor regardless, which defines the motor's limits
```

---
## \#14 Posted by: Hillso Posted at: 2016-10-11T00:53:52.894Z Reads: 194

```
I have a question. current limit of a motor determined by heat? what determines voltage limit? Thanks.
```

---
## \#15 Posted by: Hummie Posted at: 2016-10-11T02:51:05.884Z Reads: 193

```
The wire enamel. And the bearings more so.  The bearings max speed
```

---
## \#16 Posted by: bigpianist Posted at: 2016-10-13T05:16:04.608Z Reads: 186

```
I'm using 2 of these motors on 6s with 2 vescs :smile: great power and speed and don't get too hot. Would recommend :joy:
```

---
## \#17 Posted by: NickTheDude Posted at: 2016-10-13T10:49:44.870Z Reads: 184

```
Really? What kind of gearing around you running? Top speed?
```

---
## \#18 Posted by: bigpianist Posted at: 2016-10-13T12:58:00.409Z Reads: 172

```
Currently I'm using 12t-32t, 60k limitied erpm on the VESC with 70mm wheels, but I'm upgrading to kegels 36t soon. I'm 75kg and it takes me up pretty steep hills, and the top speed is insane - like 50+km/h
```

---
## \#19 Posted by: Tuomalar Posted at: 2016-10-13T13:19:36.211Z Reads: 169

```
What motor u use?
```

---
## \#20 Posted by: bigpianist Posted at: 2016-10-13T13:44:15.880Z Reads: 171

```
The little turnigy sk3 5045s
```

---
## \#21 Posted by: webst Posted at: 2016-10-13T13:50:12.249Z Reads: 167

```
Can somebody do the math and elaborate on this build?
```

---
## \#22 Posted by: NickTheDude Posted at: 2016-10-13T14:07:40.728Z Reads: 167

```
Plug 450kV, 6S, 32:12 gearing and 80mm wheels into the equation and you get a theoretical top speed of roughly 55km/h, that's without weighting. However, the maximum ERPM on that setup is 68040, and the his VESC is set to limit it to 60k. So his top speed should be a little lower.
```

---
## \#23 Posted by: NickTheDude Posted at: 2016-10-13T14:54:38.415Z Reads: 168

```
So I've finally done enough research to be able to fully understand (at least I hope I do) the blog post written by Vedder about this topic. Basically, at the same rpm, two motors, one with 150kV and one with 300kV will have the exact same efficiency/losses, but the 300kV motor will be pulling double to current. So in theory, the motor kV only matters when choosing voltage. BUT, since our ESC's will have the same resistance regardless of the kV of the motor, losses are much higher on the ESC with higher current/higher kV motors. This is why using the lowest kV possible is an ideal setup. 

He also points out that other losses start to build up exponentially around 60k ERPM. So, we should be picking a voltage/kV setup that will give us a maximum ERPM of 60k. 

Using this, I found a 5055 motor from may tech with 190kV. Running at 12S, this would get a max ERPM of 57456 which is nearly perfect, and the low kV would mean lower losses on the ESC. The motors are rated for 1170 watts. So I think these motors and 12S would be the ideal dual motor setup. Of course we still need some data on watt usage while hill climbing and the like, but I think 2340 should be enough right?

Thanks to everyone who helped explain all of this :slight_smile:
```

---
## \#24 Posted by: TarzanHBK Posted at: 2016-10-14T06:21:31.037Z Reads: 161

```
good to see that people do their research :+1:
@chaka is a big fan of double 50mm systems
```

---
## \#25 Posted by: Aggdaddy Posted at: 2016-11-16T00:53:22.711Z Reads: 155

```
I have a 300kv dual motor setup running 4.12 dual vescs, split servo, no can bus on 10s battery.

This is on a belt driven mountainboard that was built with the 300kv motors and dual VESC's on 10s from the builder.

I also have a bamboo GT, that has smaller motors, but the torque from the bamboo GT is much greater than on my 300kv motor board.  Granted they have different size wheels and I don't have the all terrain conversion  to put on bamboo GT,  but I think there would still be a big difference in torque if they had similar wheels.

I haven't taken the mountain board to the limit, it just keeps accelerating past my accustomed speed limit of 22mph of the Bamboo GT.    Gets scary going that fast.
```

---
## \#26 Posted by: darkkevind Posted at: 2016-11-16T01:18:48.644Z Reads: 155

```
I have an idea... why not run dual motors with different KVs?

Use a low KV motor to start off and get up hills, and when you're on the flat and want speed, switch electronically to the high KV motor to take over!

Vedder could even incorporate that in to the VESC where it has two motor outputs, one for high KV one for low KV and depending on amp draw, send power to the relevant motor?
```

---
## \#27 Posted by: Jinra Posted at: 2016-11-16T01:31:21.524Z Reads: 154

```
it's been done!

http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---
## \#28 Posted by: NickTheDude Posted at: 2016-11-16T01:31:28.738Z Reads: 151

```
I forget who, but someone actually tried this. If I remember correctly they said it had a similar effect to something like a sequential turbo setup in a car.

Edit: Jinra beat me to it :P
```

---
## \#29 Posted by: FredSaberhagen Posted at: 2016-11-16T01:34:39.313Z Reads: 149

```
That would be smart, put one of them on a one-way bearing as well so you don't have the drag of both belt setups (But still have some braking power)
```

---

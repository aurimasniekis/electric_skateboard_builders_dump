# Rumor has it, Next Gen Metroboard may use VESC

### Replies: 27 Views: 1532

## \#1 Posted by: onepunchboard Posted at: 2017-11-04T03:53:56.416Z Reads: 244

```
I just found out, new metro may use vesc hardware, from vesc project forum. But since Duty cycle mode is not well supported, (brake is not as strong as current mode, no regen) 

it's deal breaker for them apparently.

I used hobby esc, I like the duty mode for controlling speed, but the brake is really weak. tho there is a trick

Have anyone used Duty on VESC? 
Are they that bad?
```

---
## \#2 Posted by: evoheyax Posted at: 2017-11-04T04:16:37.619Z Reads: 236

```
Why do you even need duty cycle mode?

Watt control mode  thanks to @Ackmaniac is the best way to run your motors, hands down.

The thing is if any board company comes along like this, they will likely cheap out and use shitty quality vescs and have a lot of issues. It's not cheap to get good vescs, and that will destroy the profits of any board company like this, so they won't do it.
```

---
## \#3 Posted by: Titoxd10001 Posted at: 2017-11-04T04:18:11.182Z Reads: 227

```
Duty Cycle mode is unusable on vesc. As soon as you let go of the trigger it brakes automatically, it has no coasting. Duty mode is a feature I really miss which I think literally every other esc has whether it be for RC cars or other e-skateboards. Vesc has current mode which I guess people don't mind.
```

---
## \#4 Posted by: chuttney1 Posted at: 2017-11-04T04:20:45.355Z Reads: 213

```
They still can because some work has been done in motor control at this scale. The 4.12 firmware for the VESC is open source so it's useful.
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-11-04T04:21:26.173Z Reads: 204

```
Duty mode can control speed. so if u max out @ 30mph, half way throttle will have 15mph. 
I found it easier to control the board.

Well, no coasting sucks. Big no for me than
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-11-04T04:22:40.697Z Reads: 192

```
me too, I really like duty mode, tho I don't mind current
```

---
## \#7 Posted by: evoheyax Posted at: 2017-11-04T04:24:16.827Z Reads: 190

```
I find it more important to have a smooth acceleration. This is why watt control mode is good. You know that for example, say max watts is 1000 per motor, at 50%, you have 500 watts, at 25%, 250 watts, or full throttle has 1000 watts. It's easier to control than current mode and way more predictable.
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-11-04T04:27:48.592Z Reads: 182

```
Yeah, I know. But I don't limit the watt. So I really don't feel much different from the original fmw.
Maybe tiny bit torquy. and low end is a bit smoother.
```

---
## \#9 Posted by: evoheyax Posted at: 2017-11-04T04:33:09.820Z Reads: 178

```
I defiantly noticed a difference. I had more power at different points on the acceleration curve. It was unpredictable, especially at higher speeds. Watt control mode fixed that. Can you imagine doing what NVG does, 60 mph on that little throttle range with duty cycle? It's uncontrollable.

Limiting the watts doesn't mean you'll necessarily hurt performance. The key is to know what you can pull safely, and set it to that. It's another mechanism to better protect your motors too. Most motor manufacturers give data on max wattage, but not max amps.
```

---
## \#10 Posted by: Titoxd10001 Posted at: 2017-11-04T04:37:11.953Z Reads: 171

```
Yeah current/watt mode is like whatever. I feel like I'm not in control with those modes. With duty it feels like there is more torque at low speeds and when there is more load like going uphills or off-road. And it's really controllable at high speed. With watt I probably use 25% throttle and I can wiggle it and it basically does nothing lol. But I doubt Duty will make its way to the vesc as vedder doesn't like that mode and neither does ackmaniac.
```

---
## \#11 Posted by: onepunchboard Posted at: 2017-11-04T04:39:25.905Z Reads: 163

```
Duty cycle is very predictable tho, NGV is right direction for that speed master. They may have to careful with sudden amp spike in the beginning, but from what I experienced, duty cycle is more controllable once u used to it. 
I get that current is like driving gas car,
but the duty is like setting the speed using button, which I found more predictable on fingers.
```

---
## \#12 Posted by: evoheyax Posted at: 2017-11-04T04:48:37.124Z Reads: 156

```
see, I feel like torque is better way of controlling than speed. When you have a 1 cm throttle range, and a top speed of 60 mph, just 41% of the throttle will give you 25 mph. 8mm of play, to go 25 mph, is crazy... 

With watt control mode, when your at your cruising speed, you let off (like a car) and apply a lower current to maintain your speed. That's the most predictable way to ride, at least for a high torque board like I ride. Duty cycle with the power I have under my feet could kill me.
```

---
## \#13 Posted by: onepunchboard Posted at: 2017-11-04T05:00:16.483Z Reads: 146

```
no, you can let go with duty and it will coast too. I'm not sure why u referring to 1cm throttle range, but I can tell you that it's enough range. people use chopsticks u know, with 50 muscle movement.

Duty can still work like current, since it doesn't go full speed in 1s. it still need acceleration. It just feel jerky in the low speed, cuz it tries to use full amp.

More problem I see is the resistance in belt/hub motor in high speed.

Soon as I pass 30mph, if I let go throttle, board loose the speed rapidly. I almost fall.

@ I went up to about 47mph, higher u go less acceleration u feel, so it's not bad.

U really have to try man
```

---
## \#14 Posted by: evoheyax Posted at: 2017-11-04T05:19:08.650Z Reads: 140

```
[quote="onepunchboard, post:13, topic:37311"]
Soon as I pass 30mph, if I let go throttle, board loose the speed rapidly. I almost fall.
[/quote]

This is the problem I experienced.

I've never personally tried duty cycle above 25 mph before, but even then, It tried so hard to throw me off. This is the biggest risk we have an eboard in my mind. It's how I messed up my ankle.
```

---
## \#15 Posted by: onepunchboard Posted at: 2017-11-04T05:23:27.811Z Reads: 139

```
ouch, that sucks man. Well I went to using vicious grip tape to drop deck to lock myself. Hope u get well.
```

---
## \#16 Posted by: Blasto Posted at: 2017-11-04T05:33:21.626Z Reads: 140

```
I’m simplifying things here

Duty cycle: constant voltage, variable current

Current control: constant current, variable voltage
```

---
## \#17 Posted by: b264 Posted at: 2017-11-04T05:37:29.386Z Reads: 140

```
[quote="evoheyax, post:2, topic:37311"]
The thing is if any board company comes along like this, they will likely cheap out and use shitty quality vescs and have a lot of issues.
[/quote]

If any company on Earth didn't cheap out on their stuff, I'd expect it to be Metroboard.  Have you inspected their products?
```

---
## \#18 Posted by: onepunchboard Posted at: 2017-11-04T06:08:53.075Z Reads: 128

```
its other wy around i think
```

---
## \#19 Posted by: hornet90 Posted at: 2017-11-04T06:21:40.590Z Reads: 130

```
I have a metroboard as well as a diyboard,The Metroboard is a workhorse very well built
breaks are super strong i love it the lads in Metroboard build great stuff.....
```

---
## \#20 Posted by: Jinra Posted at: 2017-11-04T07:20:04.972Z Reads: 124

```
Why can't we have a mix? Have the throttle work like current control, but have duty cycle limited depending on position of the throttle.
```

---
## \#21 Posted by: onepunchboard Posted at: 2017-11-04T07:27:33.189Z Reads: 114

```
well I dont know how to write code and not electro mechanic 🤔
```

---
## \#22 Posted by: Titoxd10001 Posted at: 2017-11-06T08:05:11.962Z Reads: 96

```
The user should be able to decide if they want to use Duty Cycle(with coasting) mode or current/watt mode. The few that can make it happen is @trampa  and Benjamin and @Ackmaniac
```

---
## \#23 Posted by: Okami Posted at: 2017-12-09T19:07:30.419Z Reads: 82

```
Hey, thanks for all the side info abour duty / current / watt mode but so does it mean that metroboard has chinese esc inside?

 Im really curious since one user not long ago pointed out that there are not that many boards with vesc inside.. besides pulseboard, arcboard and raptor of course
```

---
## \#24 Posted by: onepunchboard Posted at: 2017-12-09T19:24:13.404Z Reads: 77

```
not sure nnever opened one. but they arnt using chinease pcb for sure. i think they have in house board
```

---
## \#25 Posted by: BasWoods Posted at: 2018-05-19T12:22:53.084Z Reads: 51

```
They have In house
```

---
## \#26 Posted by: BasWoods Posted at: 2018-05-19T12:24:07.143Z Reads: 50

```
Yeah metro board uses really good quality products in their builds. I won’t lie it looks Alittle ugly inside but that thing will last you for years.
```

---
## \#27 Posted by: BasWoods Posted at: 2018-05-19T12:26:57.154Z Reads: 48

```
[quote="Blasto, post:16, topic:37311, full:true"]
I’m simplifying things here

Duty cycle: constant voltage, variable current

Current control: constant current, variable voltage
[/quote]

Wait, so you can program a vesc to keep a constant current but lower the voltage so you can coast without the board trying to throw you off?

Or do you need duty cycle for that? I’m not too familiar cause with hub motors you coast regardless.
```

---

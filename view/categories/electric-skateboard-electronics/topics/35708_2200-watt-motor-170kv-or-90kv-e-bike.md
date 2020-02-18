# 2200 Watt motor 170kv or 90kv - e-bike

### Replies: 26 Views: 2173

## \#1 Posted by: benfa94 Posted at: 2017-10-16T22:12:09.441Z Reads: 199

```
I know this forum is mainly for esk8 but i think they are pretty similar, i'm building my first e-bike and i need to choose the motor, i want to reach about 20mph so 2200W should be enogh, my question is should i got for a 90kv or 170kv, in both case i need to gear down the motor and given the same Watt with the right gear i should reach same speed/torque ration. is there any advantage in a motor spinning faster? i red somewhere that brushless motor works better at rpm is it true?
```

---
## \#2 Posted by: GrecoMan Posted at: 2017-10-16T22:13:24.976Z Reads: 199

```
i did not say it runs BETTER at high rpm, I said it ran more EFFICIENT at higher rpm
```

---
## \#3 Posted by: Orin635 Posted at: 2017-10-16T22:13:27.405Z Reads: 194

```
I know very little but I'd assume the 170kv. also, depends on what hills you want to climb?
```

---
## \#4 Posted by: benfa94 Posted at: 2017-10-16T22:14:41.698Z Reads: 186

```
i was not talking about you :D that's something i red around, i appreciate your help, i just want more opinion, i would prefer running low rpm to be more quite
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-10-16T22:21:56.292Z Reads: 170

```
The motor you choose is dependent on what batteries you're going to use. If you're going with a standard vesc to control the motor, you're limited to a maximum of 12s. If you have a different controller in mind, then you may be able to go higher.

For a given wattage, running at a higher voltage will require less current, which means less heat.

The power of a motor is rpm*torque. Torque is determined by current. 

Running higher voltage, means you run higher rpm. Higher rpm means you need less torque for the same power.

Less torque means less current.

They're all connected!

To get the most out of your motor, it's best to run it as high speed as possible. This means high KV.

If you're only going to go for 8s, you definitely want to go with the higher KV.
```

---
## \#6 Posted by: benfa94 Posted at: 2017-10-16T22:57:02.866Z Reads: 141

```
i think something is not right, if the motor have the same Watt the maximum output power is the same so if i use a 1.8 time gear at the 90kv motor i should obtain the 170kv. is there anything special about brushless motor that make them more efficien at high speed as @grecoman say?
```

---
## \#7 Posted by: GrecoMan Posted at: 2017-10-16T23:28:50.943Z Reads: 127

```
It takes more amps to get up to speed (way more) than to stay at speed.  Once you hit max efficiency (about 95% duty cycle) the board will draw waaaaaaay less amps than if you were constantly stopping and starting.
```

---
## \#8 Posted by: benfa94 Posted at: 2017-10-16T23:38:34.848Z Reads: 125

```
i will adapt the gear to the motor, let's say i use a 3.7:1 gear for the 170kv and a 2:1 for the 90kv motor, the final wheel kv will be about 45 kv for both configuration and 2200W, is there any advantage in one of the 2 configuration or the are equivalent?
```

---
## \#9 Posted by: Boardnamics Posted at: 2017-10-17T01:44:14.331Z Reads: 122

```
Definitely 90kv. Problem with ebikes is that since the wheels are so big, they require a massive reduction. Our standard 83mm longboard wheels are significantly smaller than the, what is it, 24 inch bike wheel? E bikes are a lot more torque low rpm than that of our outrunner motors which are more low torque high rpm by comparison.

You are going to find you will need a crazy low gear ratio.
```

---
## \#10 Posted by: Nix Posted at: 2017-10-17T01:45:47.621Z Reads: 117

```
Maybe this could help?
https://electricbike.com/forum/
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-10-17T03:08:03.767Z Reads: 110

```
Welcome to the esk8 forum.

See below a quote from one of the major esk8 companies on the forum. He explains why running a motor close to 60k erpm provides the best efficiency by balancing low rpm copper losses with high Rpm iron losses.

[quote="trampa, post:89, topic:35056"]
RPM/Losses/gear reduction

Now we know that copper losses are proportional to the square of the torque produced by the motor, and at low RPM and high load they are dominant. As RPM increases, other losses start to add up exponentially. In my experience, these losses start to get significant around 60k electrical RPM, which for a 14-pole motor is about 8570 mechanical rpm (most 50mm+ outrunners have 14 poles, some unusual ones have 18). Because of the square relation, it is desirable to run at as high speed and low torque as possible as long as we stay below 8.6k RPM. To express the square relation in some numbers, having double the RPM and half the torque at a certain power output will cause four times less losses. The lesson from this is that: make sure the top speed you design the skateboard for is at around 8.6k rpm on the motor if you are using an 50mm-60mm outrunner.
[/quote]

Considering the above, I would suggest calculating your ideal KV as follows.

60,000erm/(Voltage x motor pole pairs) = Ideal KV

Example: 48V battery with a 14pole motor(7 pole pairs)

60,000/(48x7) = 178KV
```

---
## \#12 Posted by: trampa Posted at: 2017-10-17T03:40:53.543Z Reads: 90

```
Your gearing is usually limited, so 1:2.5 is realistic.
You can easily calculate the motor rpm for the desired top speed and you know your voltage, which should be as high as possible (12s).
This in combination will tell you the ideal KV.

The vesc-project has a nice calculator: www.vesc-project.com/calculators

120-170kv is the range you should look at. Lower KV motors draw less amps and are better for the esc and battery. 

Frank
```

---
## \#13 Posted by: onepunchboard Posted at: 2017-10-17T06:06:12.999Z Reads: 74

```
I think of e bike as assisted bike. we all have very efficient drive at low speed (aka legs).
so my theory is e bike should focus on top speed and assisting for hills.
```

---
## \#14 Posted by: trampa Posted at: 2017-10-17T06:20:01.156Z Reads: 72

```
Just did the maths for you

12S battery , 14/37 transmissinon ( e.g. HTD 5M belt drive), 90mm wheel
40 km/h top speed (very fast) desired.
>> motor KV =145

Frank
```

---
## \#15 Posted by: benfa94 Posted at: 2017-10-17T08:24:00.183Z Reads: 70

```
Thanks! that was exactly what i was looking for,.
Now i just need to choose a good sensored motor, i was looking at ollin but the 170kv is out of stock, alien power system has some good motor, any suggestoin on the brand? same for the vesc, i need som suggestion, i think i will stay between 120kv and 180kv with a 8/10s battery to leave some sapce for improvement in the future
```

---
## \#16 Posted by: BigBoyToys Posted at: 2017-10-17T08:28:33.048Z Reads: 70

```
I just had 4 motors custom built by Alien power and I cant say anything but good things about the customer service I received. Excellent communication, very experienced and knowledgeable staff, and fair prices.
```

---
## \#17 Posted by: benfa94 Posted at: 2017-10-17T08:29:45.569Z Reads: 68

```
what vesc did you use? that seems to be the part more likely to fail
```

---
## \#18 Posted by: BigBoyToys Posted at: 2017-10-17T08:32:06.044Z Reads: 70

```
Ive had excellent experiences with the Enertion FOC box. Ive also been using the VESC 6's from Trampa since they were released in Beta without any problems. Both companies have provided great customer support as well.
```

---
## \#19 Posted by: trampa Posted at: 2017-10-17T15:02:16.071Z Reads: 60

```
http://www.trampaboards.com/136-kv-2400w-dc-brushless-motor-6364-61-p-12967.html

Frank
```

---
## \#20 Posted by: benfa94 Posted at: 2017-10-17T16:44:22.177Z Reads: 53

```
that looks really good but the price is way higher than the competition, i think i will go for a alien power system 3300W 130kv for around 80/90 pound,  i don't see why this motor is twice the price
```

---
## \#21 Posted by: onepunchboard Posted at: 2017-10-17T16:46:39.150Z Reads: 53

```
i believe thise are handwind motor.
```

---
## \#22 Posted by: benfa94 Posted at: 2017-10-17T16:49:37.614Z Reads: 53

```
is there any real advantage?
```

---
## \#23 Posted by: onepunchboard Posted at: 2017-10-17T17:56:51.155Z Reads: 48

```
presision and reliability i guess. I dont think it's usful for personal ev per the price
```

---
## \#24 Posted by: trampa Posted at: 2017-10-17T20:09:11.314Z Reads: 45

```
Nice high end magnets, high temp. copper, Jap precision bearings, hardened axle shaft, hand would to max copper fill, dual keyway, filter disc, A4 stainless all the way through.
Quality drives the price up, but these ones are very powerful and long lasting motors.

Frank
```

---
## \#25 Posted by: benfa94 Posted at: 2017-10-17T22:37:12.647Z Reads: 40

```
i will start with cheaper component, if i will manage to brake them i will go for vesc 6 and tramp motor, right now i need to find a vesc to be delivered in UK without waiting for months and with good quality to support foc + sensored at 8/10s
```

---
## \#26 Posted by: saul Posted at: 2017-10-18T04:53:31.948Z Reads: 37

```
if you're on big wheels you want as low kv as possible. 90kv is good.

http://calc.esk8.today/
my calc will work for you, just find wheel size in mm. 700c(29") is about 622mm.
15/120 90kv 10s = 27 mph. 
pretty good.
```

---

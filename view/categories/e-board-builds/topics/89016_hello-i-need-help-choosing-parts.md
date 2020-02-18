# Hello, I need help choosing parts

### Replies: 5 Views: 212

## \#1 Posted by: Torill Posted at: 2019-04-01T20:29:05.577Z Reads: 82

```
Hi!

I’m planning on building my first esk8 and I need help knowing which parts I should choose to get the specs I want. I’ve spent my whole weekend researching diy esk8, but feel like I still have a lot to learn.

I live in Norway and there is a couple of restrictions here when it comes to electric skateboards, one of them is that the board needs some sort of barrier or to be built in such a way that the max speed will only be 20 km/h (ca. 12 mph). There’s also some steep hills around where I live, I mean not quite San Fransisco type of hills, but it sure does feels like that some times. I would guess the steepest ones are about 15-20% gradient. I’m thinking that I will be riding at 12 mph most of the time and would like to get up the hills without slowing much down. 

My best guess so far is that I need good torque so maybe two 6374 motors (or will 6355 work?), and I need a battery with low s and high-ish p, so maybe ideally a 4s6p battery(?). But my concern about a weak battery is that it won’t be able to get me up the hills fast enough or up the hills at all. Does anyone know how I can build a board that will get me up the hills at 8-12 mph but still not ride any faster than 12.4 mph on flat ground?

To summarize, the specs I would like is:
- Max speed: 20 km/h (12.4 mph)
- Range: 25 - 50 km (ca. 15 - 30 miles)
- Max weigh (of the board): 20 lbs
- Being able to carry 90 kg (200 lbs) comfortably up a steep hill (good torque)

Thanks
```

---
## \#2 Posted by: Superflim Posted at: 2019-04-01T21:23:07.506Z Reads: 62

```
get 10s. You won't regret.

dual 6355 will be plenty for most people.
```

---
## \#3 Posted by: rusins Posted at: 2019-04-02T00:16:16.142Z Reads: 54

```
You can limit the max speed through software for the VESC, so your theoretical top speed shouldn't matter too much

For the hills you described, dual 6355 motors would be just fine, but Norway does have some extreme hills, so if you want to go traveling and tackle those I would go for dual 6374 (even if just to reduce the heat in the motors). To maximize torque even more (and because you really don't need speed), I might even go for a gear drive so that you don't have any belt slip issues, and can get a good gear reduction ratio. (Or, you go for big urethane wheels so that your wheel pulley can be big, while the motor pulley remains small. TorqueBoards new 110mm wheels would be a good option ;) )

Off topic:
I was in Norway 2 years back and took my regular longboard with me to sight-see the city of Bergen on my own, and nearly died by going down a fairly steep hill which suddenly turned into a 40° death-slope downwards :grimacing: (it gets even steeper than shown in the picture, trust me.)
 ![hill|690x318](upload://qrENFjdMD5BhPC2SJiGF0buDoKP.jpeg) 

I didn't have a helmet with me (wasn't planning on downhilling lol, the path just went there), so had to bail by riding into that grassy area on the right in that picture. Tore my hoodie, jeans, underpants and shirt, but it was worth it, because even a few meters more could have been fatal. Many lessons were learned that day.
```

---
## \#4 Posted by: meesie Posted at: 2019-04-02T11:37:27.030Z Reads: 36

```
i would suggest going for 10S or 12S. go for 6374 at 170KV for even smoother hill climbing (and better braking) and then gear it down to your desired max speed. this way you get the most torque out of your build.

you'll need to take your battery in account too by the way. if you want to climb hills your motors are going to want to pull a lot of amps. i'd recommend at least 10s4p or 12s3p. the more batteries in parallel the more amps you can get out (**and in!!**) of it.
```

---
## \#5 Posted by: jeorghe Posted at: 2019-04-02T14:16:56.897Z Reads: 27

```
I can suggest this configuration:

- 10s battery  ( hobbyking big discount now ...)
 2X https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c-xt90.html?___store=en_us
or
2X https://hobbyking.com/en_us/turnigy-high-capacity-10000mah-6s-12c-multi-rotor-lipo-pack-w-xt90.html

- 2 Turnigy SK3 149KV (Big torque) https://hobbyking.com/it_it/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
- 15/72 gear ratio  ( near to 30 km/h)
- Flipsky dual 6.6 or dual 4.12 (50A limit) .
- Motor mount ask ti @idea in this forum ;)
```

---

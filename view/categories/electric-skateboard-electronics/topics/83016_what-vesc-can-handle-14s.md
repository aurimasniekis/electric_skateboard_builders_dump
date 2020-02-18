# What vesc can handle 14s?

### Replies: 18 Views: 1106

## \#1 Posted by: Noob-at-building Posted at: 2019-02-03T11:14:16.401Z Reads: 228

```
I was thinking of possibly using these [APS 63100 Outrunner brushless motor 140KV 4500W](https://alienpowersystem.com/shop/brushless-motors/aps-63100-outrunner-brushless-motor-140kv-4500w/) from alien as an over kill board.
but the main issue is finding a 14s vesc, and recommendations?
i would run it at 14s if i can, i would make this into an ATB using a trampa deck with pneumatic wheels.
```

---
## \#2 Posted by: taz Posted at: 2019-02-03T11:31:42.732Z Reads: 216

```
You did not set a budget so...

https://www.trampaboards.com/single-vesc-75v-300a-in-cnc-t6-silicone-sealed-aluminum-box--the-most-powerful-vedder-electronic-speed-controller-ever-p-26293.html
```

---
## \#3 Posted by: Noob-at-building Posted at: 2019-02-03T11:38:03.143Z Reads: 212

```
can you run 2 motors with that, or does it have to have all 3 running?
```

---
## \#4 Posted by: taz Posted at: 2019-02-03T11:41:09.092Z Reads: 210

```
It is a single vesc. The reason for the multiple wires is to keep them flexible.
This means you will need two of them for a dual setup.
It was not designed as an esk8 specific controller hence the price and current capability
```

---
## \#5 Posted by: Noob-at-building Posted at: 2019-02-03T11:42:28.356Z Reads: 208

```
would you recommend running two single ones for a dual setup
```

---
## \#6 Posted by: taz Posted at: 2019-02-03T11:44:48.875Z Reads: 199

```
Most of us are running 2 single vesc based escs for a dual setup.
The dual escs such as the Unity have only recently hit the market.
```

---
## \#7 Posted by: Andy87 Posted at: 2019-02-03T12:10:32.724Z Reads: 192

```
https://vesc-project.com/node/339

https://www.electric-skateboard.builders/t/cheap-vesc-vesc-4-12-redesign/81344?u=andy87

But one question, why not to run the motors on 12s? What’s the problem?
```

---
## \#8 Posted by: Noob-at-building Posted at: 2019-02-03T12:31:39.767Z Reads: 176

```
i want more power, an i also want to test 14s out since i have a 12s board already
```

---
## \#9 Posted by: Andy87 Posted at: 2019-02-03T12:42:59.694Z Reads: 177

```
Ok.
You know the basics of repairing motors?
Because it’s very likely that you will need that at one or the other aps motor 😉
```

---
## \#10 Posted by: starstuck8 Posted at: 2019-02-03T21:22:08.990Z Reads: 140

```
Just for us craaazy boooyz who would even think of this, what causes them not to be durable?
```

---
## \#11 Posted by: Battosaii Posted at: 2019-02-03T21:29:50.194Z Reads: 138

```
Nothing about him or his uses

APS motors have a reputation for poor quality.
```

---
## \#12 Posted by: starstuck8 Posted at: 2019-02-03T21:31:27.007Z Reads: 139

```
Geez. I wouldn't want to be giving aliens a bad name when they land!
```

---
## \#13 Posted by: Jacobee Posted at: 2019-02-03T21:58:39.962Z Reads: 134

```
Most VESCs are rated to 60 volts. 14 times 4.2 is 58.8 so it would be possibility using a focbox or other vesc the problem is voltage spikes from braking so I think it would be okay if you ran 14s without breaks and used some disc breaks or something to stop. All that said I still wouldn't recommend 14s. 12 or 13s and high amps will get you plenty of power.
```

---
## \#14 Posted by: ninTHIENdo Posted at: 2019-02-03T22:16:42.234Z Reads: 124

```
https://youtu.be/5MFjzSP5Oiw

Here’s a good video of what to do if you get those motors, and the previously mentioned trampa 75v 300a would probably be the best VedderElectronicSpeedController, developed by Ben Jamin’  Vedder.
```

---
## \#15 Posted by: Minim Posted at: 2019-02-03T22:25:48.049Z Reads: 117

```
Is there a special kind of epoxy that should be used? For my hub motors I would need something that can handle heat because it get really hot in there :P
```

---
## \#16 Posted by: Noob-at-building Posted at: 2019-02-04T00:41:14.960Z Reads: 105

```
Therese always a place to learn :slight_smile:
```

---
## \#17 Posted by: Andy87 Posted at: 2019-02-04T01:54:07.410Z Reads: 106

```
That’s good.
And they have a good customer service.
If something broke contact them, with a bit luck they will replace it.
```

---
## \#18 Posted by: Andy87 Posted at: 2019-02-04T02:45:44.631Z Reads: 104

```
Let’s say, I have 9 of motors from them.
4 of them are broken.
1 had a broken magnet after I made motor detection.
1 had a defective bearing
2 others had broken magnets during the first 300km.
If you hit over 40km/h you get a high pitching noise from the 6384 motors I have.
That’s all issues which can be fixed if you know how, but that shouldn’t be non the less.

Other reported issues I heard from,
The retainer ring gets lose and slightly lose windings which cause strange noises while driving.
The 80xx motors don’t have silicon phase wires and the big bearing seems to be low quality.


I would first check if the motors run without issues when you get them and then directly do what @ninTHIENdo already linked.
You can read it up here too

 https://www.electric-skateboard.builders/t/ice-crusher-16ply-holypro-4w-chain-drive-mtb-4x-6374-170kv-aps-quad-escape-steering-damper/65823/119?u=andy87
```

---

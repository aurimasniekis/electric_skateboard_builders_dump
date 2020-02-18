# Is this setup/build viable?

### Replies: 8 Views: 859

## \#1 Posted by: nordlicht Posted at: 2017-09-25T12:00:26.255Z Reads: 105

```
Hello there,
first off, I already made a elongboard with a 150A turnigy ESC, 2x3s 4000mAh LiPos in series, a 2kW Motor from hobbyking and a RC controller. I bought the belts online and crafted a distance piece to mount the motor on the truck.
It works pretty fine, I have 8km riding distance with a top speed of 32km/h on flat level.

Now I want to design a new board within a project at the uni.
What I want:
- board needs to be silent (HUB are a must-have here)
- motors need to be sensored
- range should be above 20km
- top speed should be atleast 40km/h, 50 would be a dream.
- Lithium **ION** batteries. LiPo's are too dangerous in my opionion. Also charging is easy with integrated BMS 

About the battery: I thought about building my own battery, doesnt seem to be too complicated.
I'd use 18650's 30q and would use them 12s3p
[here is the datasheet](https://batterybro.com/products/samsung-30q-inr1865030q-3000mah-15a)
they have 3,6V, 15A continous discharge current and 3000mAh.
Using them 12s3p, i would be at 
43.2V
45A discharge cintinous (you can easily double that for t<10s)
and 9Ah (3*3Ah, since it's 12s3p right?)
I need to spot weld nickel strap on there, which shouldnt be much of a deal (my uni got some good equipment).

As for the BMS, kind of unspectacular, I want to use 
[this](http://www.batterysupports.com/44v-48v-504v-12s-100a-12x36v-lithium-ion-lipolymer-battery-bms-p-393.html) battery management system for 12s Li Ion, don't think there can be much trouble, right?

Everyone on the internet who is into DIY e-longboards sais "the vesc" is the best.
[I assume you are talking about this esc, right?](collections/esc-speed-controller/products/torque-esc-vesc-bldc-electronic-speed-controller)
**Does this thing support 2 motors at the same time?** I read somewhere (dont find the thread anymore :confused:) that it does, I would wonder than how to connect the Hallsensors and where to connect the other motor, since they can't be used parallel?
**If not, I would simply buy 2 of those vesc, or do you know a better option for twin motors?**
Also: most ESC have a ventilator to keep the mosfets cool, I think I'll just install a silent vent powered by the 5V port there to increase the lifespan.

And last but not least for the motors I want to use Maytech ones from alien power systems:
[Link to the motors](http://alienpowersystem.com/shop/brushless-motors/63mm/sensored-hub-brushless-motor-for-longboard-maytech/)
I simply copypaste the specs from the website:


----------

MOTOR: 9555 _(pretty sure here is a typo and they want to say: MOTOR: 9355)_
KV: 60
MAX POWER: 2000w
WIRE WINDS:
MAX AMP: 50
ESC: 100A
MAX VOLT: 12S
RESISTANCE (Ohm):
NO LOAD CURRENT: 0.4A
SIZE: 93×55
WEIGHT (g):
POLES:
SENSORS: Yes


----------

So those specs (basically just the power and amperage) are for both motors, right? 2kW on a single one would be too extreme and also too expensive in that size, I expect.
Also what kind of confuses me, is that I'm not able to find this motor somewhere else on the internet. [Not even here on there own website.](http://www.maytech.cn/en/product/e-skateboard/e-skateboard-motor/hub-motor-for-e-skateboard)
The 9055 is a completely different motor (basically, just 200w less, and 3mm in diameter)
I decided for Maytech motors instead of Torque one, because the alienpowersystems guys are usually only having "the good stuff". I read some good and bad reviews for both motors on the internet.
My decision of thos motor is not 100% done yet, it just needs to be a sensored HUB motor with really low KV (this is also a a reason why i decided for maytech over torque, maytech has 60kv, torque got 75kv). If you know some other good HUB motors, I'm open!

Do you see some mistakes in the setup or parts I dont really need/would need (except the RC-control of course :stuck_out_tongue: ?

Since this is part of a university project, I can easily upload a tutorial for ppl who are less into electronics afterwards.

Thanks for reading and (hopefully :heart_eyes: )replying,
Nordlicht
```

---
## \#2 Posted by: raven Posted at: 2017-09-25T12:42:56.283Z Reads: 72

```
Hi do you know why the motor has a crinking sound
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-09-25T13:56:27.699Z Reads: 69

```
You probably won't be hitting 40km on 60kV hubs. 75kV would probably do it.

Also those hubs likely won't be getting you anywhere near 2000W each without overheating.

A 12S3P of Samsung 30Qs will definitly get you in excess of 20km range. Probably closer to 30 if not higher.

And yeah you'll need to use two VESCs with either split PPM or a canbus cable.
```

---
## \#4 Posted by: Colson003 Posted at: 2017-09-26T00:53:24.438Z Reads: 55

```
With the 130kv torque hub motors you can hit 38mph seen here: https://www.youtube.com/watch?v=_5iQlEIksqs
```

---
## \#5 Posted by: nordlicht Posted at: 2017-09-26T15:30:21.080Z Reads: 43

```
Hi, 
thanks for your answers! Why do I need to connect the VESCs with can or PPM? Can't I simply connect the RC receiver to both VESCs?
```

---
## \#6 Posted by: nordlicht Posted at: 2017-09-26T15:30:51.438Z Reads: 43

```
I don't really know =/
```

---
## \#7 Posted by: mkeboard Posted at: 2017-09-26T15:44:57.652Z Reads: 44

```
What @NickTheDude was referring to was a split PPM cable, so yes you are essentially connecting the reciever to both VESCs. This thread:

http://www.electric-skateboard.builders/t/y-piece-or-canbus/26461

goes into detail about peoples' experiences with both canbus and split PPM.
```

---
## \#8 Posted by: nordlicht Posted at: 2017-09-26T18:35:29.376Z Reads: 39

```
Ah alright, I didn't know that PPM refers to the RC-control :stuck_out_tongue_closed_eyes:
```

---

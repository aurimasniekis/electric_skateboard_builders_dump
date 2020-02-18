# Board isn’t performing like it should

### Replies: 30 Views: 409

## \#1 Posted by: HarrisCarvel Posted at: 2019-01-24T13:21:36.493Z Reads: 165

```
Hi guys,
My new board has recently been assembled and it isn’t get the performance it should. It has 2 torque boards 80A 260kv motors which I think r 4000W each max. Also it is running two vesc 2.0 and a 12s2p battery from torque boards. The wheels r 200mm. The hearing ration is 16T:72T. So I plugged these numbers into the vesc tool and started increasing the brake power and throttle curve along with the calculated Erpm max and A max. I still need to change the A from 50:60 to 80:80 for the motors and battery draw however last time I increased it there was no noticeable difference. The board doesn’t have torque and seems really fast but calcs say it should go 54 whereas I have gone 40 and thing it will probably not accelerate past 45. Lastly it doesn’t want to go faster than 22mph at 30% or below. Any ideas what I can do to increase the torque? And improve the speed at low battery power?
```

---
## \#2 Posted by: ju5t Posted at: 2019-01-24T13:30:28.885Z Reads: 153

```
test the power output with a voltmeter ensure the battery is putting out enough valts and amps for 45 and dual motors.

Then you need to test the motors and ESC.

you can do this with either a second ESC or motors to figure out which part is faulty.

This is most likely the battery or ESC if both motors spin at same speed.
```

---
## \#3 Posted by: Sebike Posted at: 2019-01-24T13:30:45.599Z Reads: 145

```
I don't know what cells you have in that battery, but 80 A batt max is too high for a 12s2p pack and your cells might overheat and get permanent damage, plus, they probably can't even put out that high of a current.

Edit... If you have two motors and set current to 80 batt amps, that means you try to pull a total of 160 amps from your battery. No good. 
If you have 30q or 25R cells in your pack, batt max per vesc should be 15-20 A max.
```

---
## \#4 Posted by: Komamtb Posted at: 2019-01-24T13:36:04.004Z Reads: 122

```
you do have way too small P count for a dual drive with 200mm wheels.
```

---
## \#5 Posted by: HarrisCarvel Posted at: 2019-01-24T13:48:47.203Z Reads: 116

```
What is p count?
```

---
## \#6 Posted by: HarrisCarvel Posted at: 2019-01-24T13:49:25.289Z Reads: 114

```
/ torque boards says 12s2p battery can handle 80a output so could I set 40a battery pull and 40a motor pull?
```

---
## \#7 Posted by: HarrisCarvel Posted at: 2019-01-24T13:49:51.322Z Reads: 102

```
How exactly do you test the ESC? I don’t fully understand that part.
```

---
## \#8 Posted by: Sn4pz Posted at: 2019-01-24T13:55:35.337Z Reads: 98

```
Yeah that's a negatory cheif. No way a diyelectric pack can handle 80a w 2p... You proabably have 40a max with 2p, and it would be the panasonic lion cells if you didn't select 30q 🤷

E: I misread the vendor, but corrected my thoughts to show for it
```

---
## \#9 Posted by: HarrisCarvel Posted at: 2019-01-24T14:12:21.746Z Reads: 90

```
Ok thanks very much. So I’m still kinda new to this. I have a dual setup so on each individual vesc do I set the motor pull and battery pull to 40:40 or 20:20 on each vesc?
```

---
## \#10 Posted by: HarrisCarvel Posted at: 2019-01-24T14:16:37.860Z Reads: 92

```
![image|281x500](upload://iFZffsY1MqWZuG0HEDllZqaoSZm.jpeg) ![image|281x500](upload://22jyc22cFeK2DgFxRK4uHceyp9s.jpeg) 
These are two photos of the battery pack. It says 30A continuous output 80a max. So what should me exact vesc setting for the motor pull and battery pull be per vesc?
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-01-24T14:31:57.736Z Reads: 82

```
20 20 on each vesc, or 15 15 if you want to conserve a little power and save it for extending the range a little
```

---
## \#12 Posted by: HarrisCarvel Posted at: 2019-01-24T14:35:20.794Z Reads: 82

```
Ok thanks! Will that improve my torque or braking issue at all. Also for strong brakes should I set it close to the battery output Amps so 20 on each vesc?
```

---
## \#13 Posted by: ninTHIENdo Posted at: 2019-01-24T14:48:22.674Z Reads: 80

```
Increasing your motor max current will increase your torque...be careful and play with vesc settings within your limits
```

---
## \#14 Posted by: Sebike Posted at: 2019-01-24T15:10:26.041Z Reads: 75

```
What the specs sais is that the bms can handle 80A peak and 30A continuously.. 

The 30q cells will give you 40A max in this configuration (2p). So, considering you are running discharge through BMS, which has a 30A limit, set each esc to 15A batt max.

To increase low end torque, set motor max higher. Try upping this setting until you're satisfied, 
A 70 A motor max will make the total available watts (650 W) usuable from 21-100%  on your throttle.

Edit  didn't consider dual motors and 12s....
```

---
## \#15 Posted by: Sebike Posted at: 2019-01-24T15:22:45.860Z Reads: 71

```
p count = how many cells in parallell configuration in your battery. Your battery has 12 cells in series and 2 cells in parallell, which gives you 12 times 2 cells in total. This increases voltage times 12 and total amp output and total capacity (Ah) times two.

More cells in parallell and series will increase max watts.
```

---
## \#16 Posted by: HarrisCarvel Posted at: 2019-01-24T16:11:45.660Z Reads: 67

```
Awesome, thanks for the help. However I have already done some settings similiar to that and it doesn’t have the specs like I think it should. So I’m thinking of the testing the battery and ESC. And idea how to test the ESC?
```

---
## \#17 Posted by: Acido Posted at: 2019-01-24T16:15:21.041Z Reads: 66

```
no they cant continuously
maybe for 2-3 seconds they can
```

---
## \#18 Posted by: Sebike Posted at: 2019-01-24T16:28:39.121Z Reads: 67

```
You have 650 W available per motor. You have huge wheels and a relatively high kv motor. I wouldn't expect torque to be terrifying on this build. 

On the other hand I myself don't have any real life experience from 200 mm wheels with 270 kv motors and a 2p battery, so don't know what torque that'd be capable of.

Not sure what you mean by testing the ESC.. You mean if it's faulty or not?
```

---
## \#19 Posted by: evoheyax Posted at: 2019-01-24T16:38:57.315Z Reads: 61

```
Get a better battery and ESC and you'll get many times more torque. You can't get more watts than your battery can provide and speed controller can handle. Up both of these you'll get better torque.
```

---
## \#20 Posted by: HarrisCarvel Posted at: 2019-01-24T16:44:10.889Z Reads: 60

```
Yah I want to see if it is faulty ESC
```

---
## \#21 Posted by: evoheyax Posted at: 2019-01-24T16:50:55.184Z Reads: 57

```
It's probably fine, these settings are very low compared to what many of us are building. That mixed with not the right kv motor and gearing setup as mentioned before, limits your torque. You have 2 things limiting you. First, your battery can't do many amps. But up that, and your esc's can't do more than 30 each continuous. Up both of those and you'll be able to get way more power out of it. Right now, at 15 amps each, you can only pull 750 watts per motor (or 1500 watts total).

But li-ion is limiting in that way. You need high p count's or your stuck with very low settings. Each p is 20a, If you had focboxes instead those vescs, and a 12s5p instead of a 12s2p, you could run 50 battery amps per motor, and 100 motor amps per motor, and then you could pull 2500 watts per motor, 5000 total, and you would have a much better setup. Also, fixing your gearing might be the cheapest solution, but I would only expect modest gains from that.
```

---
## \#22 Posted by: HarrisCarvel Posted at: 2019-01-24T16:58:37.192Z Reads: 57

```
The vescs can pull 50A continuous. So does that mean my max motor A is 50?
```

---
## \#23 Posted by: evoheyax Posted at: 2019-01-24T17:16:06.348Z Reads: 54

```
Good luck with that. I’m telling you from years of real world experience and vedder himself, they can do 27 continuous before they start to have out of control heat growth.

Think of it like this. You have certain amount of watts. Watts are amps * voltage. So you run at 50 volts, then 15 amps in the battery, that means you can do 750 watts max. The esc runs the motor at low voltages and high amps, so say 7.5v and 100 amps.  Don’t confuse motor and battery amps, they are different but also affect each other. It starts with battery amps. If those are set too low, you can set your motor amps super high and won’t notice any difference. Because the power for esc to minipulate just isn’t there. But once your esc has the power from the battery, the esc can limit how many watts (through controlling amps) the motor will see, so as not t burn up the motor and make things controllable (too high of a setting can make your wheels spin out for example).
```

---
## \#24 Posted by: HarrisCarvel Posted at: 2019-01-24T17:22:54.610Z Reads: 50

```
Ok thanks for all ur professional advice. Once I get the money I will upgrade everything. However, can you recommend a place to get a 12s5p battery preferably like this one: 
![image|281x500](upload://eyVGwZwUsX7bXSjP3cMFvGfGemT.jpeg) 
Or is this one good?
Also is this a good focbox to use?
![image|281x500](upload://xEi8mpHUIrpjZWl5oyih26KRfPq.jpeg)
```

---
## \#25 Posted by: Jacobee Posted at: 2019-01-24T17:32:14.931Z Reads: 48

```
I wouldn't really recommend a battery from alibaba. You're gear ratio is to high (it will get you about 36mph max according to the calculator) for how small your battery is. Try gearing your board for lower speed (smaller motor pulley & bigger wheel pulley)

Edit: I originally had calculated for 190 kv motors with 260kv motors the calculator says 51mph
```

---
## \#26 Posted by: evoheyax Posted at: 2019-01-24T18:08:57.886Z Reads: 47

```
I would look into psychotiller’s battery services. And yes that is a good esc.

I would first fix your gearing though as it’s the cheapest solution to improve your situation. It won’t be night and day better but better.
```

---
## \#27 Posted by: rolloo Posted at: 2019-01-24T18:23:54.316Z Reads: 47

```
**260KV**. Ratio **4.5:1**. Wheels 200mm.? 
Gear ratio (Motor KV) is to high.
```

---
## \#28 Posted by: TowerCrisis Posted at: 2019-01-24T19:13:42.875Z Reads: 45

```
Just to clarify, motor amps has no relationship to battery amps.

You can set your motor amps to whatever you want as long as it stays within the specifications of the motor. This will affect low speed acceleration and braking.

Your battery amps will affect higher speed acceleration and braking. It should be determined by the battery specification.

This "disconnect" between their effects is because the vesc will modulate voltage depending on throttle. At 50% duty cycle, a vesc drawing 20A from the battery will actually be outputting 40A at half the voltage to the motor. This is a bit of an oversimplification because of the DC -> 3 phase conversion, but you get the point.
```

---
## \#29 Posted by: Santino Posted at: 2019-01-24T20:02:47.215Z Reads: 42

```
Another option is to sell those high Kv motors and get 130Kv to 150Kv, and change pulleys (motor 13 or 14 teeth and 66T wheel) if you want to use 200mm wheels... Therefore you could use lower amps to each motor (lower Kv motors works great at lower amps getting tons of torque). I am at 60 amp motor max with 150kv with 200mm wheels, but I started at 40 motor amp with tons of torque..The lower the Kv, the higher the torque... Hope it helps, good luck!
```

---
## \#30 Posted by: meesie Posted at: 2019-01-25T08:35:39.651Z Reads: 32

```
this it what it says on diyelectricskateboard's website: * **Built-in Battery Management System (BMS) ($60 VALUE)**  - BMS is rated for 30A Continuous Amp Output and 80A Peak Amp Output.

it's the BMS that can hande 80A. your pack can only handle 30A. 15A per paralel connection. as you have two focboxes, each focbox may only be set at 15.
```

---

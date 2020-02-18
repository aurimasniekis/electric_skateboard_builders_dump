# Will high motor max lead to voltage sag

### Replies: 12 Views: 228

## \#1 Posted by: SquidKingRabbit Posted at: 2019-08-27T07:36:10.541Z Reads: 80

```
Hi so I am running 6364 245kv motors with 7s4p li-ion battery. 

I set the value of motor max to 70a and battery max to 40a. I find that after few minutes of riding, the motors get quite hot and I don't have the same torque as before. 

So am I getting voltage sag due to overheating of the motors or maybe it has something to do with my batteries?

Thanks
```

---
## \#2 Posted by: Andy87 Posted at: 2019-08-27T08:18:20.028Z Reads: 75

```
You have temp sensors?
If so and your motors get hot than it’s not voltage sag. It’s just your vesc, throttling down to save your motors from getting destroyed.
```

---
## \#3 Posted by: SquidKingRabbit Posted at: 2019-08-28T16:32:06.470Z Reads: 47

```
temp sensors as in the sensor wires from the motor right? if yes, then no I do not have temp sensors. just 3 phase wires connected to the vesc

anyway should motors get hot to the touch when climbing hills? also what will decreasing my motor max do? less torque? less hill climb ability?

thanks andy
```

---
## \#4 Posted by: Andy87 Posted at: 2019-08-28T19:25:18.552Z Reads: 42

```
everything under 80 degrees Celsius is ok.
If you don’t have temp sensors than 100 degree should handle most motors. Over that you run risk to damage them.
Do you know the amp rating of your  motors?
Also which vesc you use and what your settings for bat max, min?
You run a very low voltage with your 7s. What is your battery cut off?
The reason why I ask is that it can be that your vesc is throttling down due to overheating of the vesc it self or due to running into battery cut off.
```

---
## \#5 Posted by: Santino Posted at: 2019-08-28T23:49:28.465Z Reads: 35

```
I think you are using high kv motors with low voltage, that probably stress the battery and your motors too because of low voltage capability. I would increase to a 12s  battery and a lower kv motor (130kv-170kv range), if your plan is to do hard riding and hillclimbing...Esc must be able to handle 12s and high amps...Also choose the right gearing for your needs...
```

---
## \#6 Posted by: SquidKingRabbit Posted at: 2019-08-29T06:16:25.305Z Reads: 23

```
my motor max amp rating is 80a

i am using vesc 4.12, firmware 2.18

battery max is set at 40a
battery min is set at -9a

battery cut off start 22.4v
battery cut off end 21.7v

![vesc%20settings|690x329](upload://i4dydxyeGSbU75AtuqkqUtooOFp.png)
```

---
## \#7 Posted by: SquidKingRabbit Posted at: 2019-08-29T06:17:33.352Z Reads: 21

```
i will take your suggestions for future upgrades. but for now since i am a student and this is what i have, i will just make do with what i have got. 

thanks santino
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-08-29T06:26:14.646Z Reads: 20

```
No, you are not getting voltage sag. 
Your vesc is heating up due to hard use (hill climbing) and reaching the thermal protection limit. (The vesc has a temperature sensor onboard, as well as connections for external ones in the motors.)
Yes, your motors will get hot when climbing hills.
No, it has nothing to do with your batteries.
Decreasing your motor max will reduce the torque your motors have under heavy load at low-to-moderate speed (hill climbing and accelerating from a standstill).

If you want to climb hills with greater ease and you don't have the resources to upgrade to 10S or 12S (Don't go 12s with vescs based on stock 4.12 hardware, that ends in streetface), then your best bet is to lower your gearing: Smaller motor pulley, and/or bigger wheel pulley. This will reduce your top speed and increase the torque you have for hills.
```

---
## \#9 Posted by: Andy87 Posted at: 2019-08-29T06:57:05.185Z Reads: 20

```
I‘m not often agree with @MysticalDork :stuck_out_tongue_winking_eye: but he is totally right here.
With 4.12 hw and bat max 40A it’s probably your vesc which throttle down due to overheating. Don’t use 12s on 4.12 hw as long as it’s not a focbox. 10s would be a good suggestion thou.
If you can’t upgrade your battery, for now my suggestion would be to adjust your bat max to 30A and try to mount your vescs in a way they get air flow or attach an additional heat sink.
```

---
## \#10 Posted by: Andy87 Posted at: 2019-08-29T07:01:48.782Z Reads: 21

```
One additional suggestion.
Undo the „limit max erpm with negativ torque“
![image|404x499](upload://cKSpvBdiNwLIhLK8RBxHAlJqzD9.jpeg) 

With your setup you will not run into any issues as you will not hit the max erpm limit anyway, but for future, what it would do is to slam in brakes if you hit max erpm, so at your top speed your vesc would start to brake. Something you don’t want to have usually.
```

---
## \#11 Posted by: SquidKingRabbit Posted at: 2019-08-29T07:29:35.643Z Reads: 18

```
@MysticalDork @Andy87

hey thanks for all the information and suggestions!
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-08-29T08:19:03.611Z Reads: 18

```
Yeah, that's a veeeery dangerous setting to have checked. It can even kick in if you're going down a hill and you exceed the maximum ERPM even if you can't exceed it on flat ground. Streetface is no fun.
```

---

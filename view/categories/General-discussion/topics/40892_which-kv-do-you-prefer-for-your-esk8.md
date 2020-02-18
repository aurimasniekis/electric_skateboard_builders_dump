# Which KV do you prefer for your ESK8?

### Replies: 12 Views: 1070

## \#1 Posted by: Luuke Posted at: 2017-12-13T08:07:59.522Z Reads: 205

```
Hi,
what is your prefered KV for your ESK8?
I am curious what is your oppinion on that. Please tell me the Voltage of your batterie as well.

At the moment I think 230 KV should be the best for a 10S Setup.

Reason to ask is, that I am thinking about to order one custom 6374 KV motor (or 2 x 6355 for dual drive).
Other option would be to buy some more motors and resell it here for non profit. But therefor I have to know which KV are favored.
```

---
## \#2 Posted by: pennyboard Posted at: 2017-12-13T08:11:09.765Z Reads: 205

```
https://www.electric-skateboard.builders/search?q=kv%20for%2010s

I have no preferred KV. 

My preferred method of getting information, however, is to Search for it first before immediately asking a question.
```

---
## \#3 Posted by: Luuke Posted at: 2017-12-13T08:18:12.211Z Reads: 202

```
Ok, thank you!
I know which KV I could use based on the ERPM limit.
Also I know which motors are available on the market (SK3, TB etc.)

But I want to know your personal prefered KV.
```

---
## \#4 Posted by: FredrikHems Posted at: 2017-12-13T08:54:14.802Z Reads: 186

```
That depends entirely on voltage. for a 6s build 250 is a good one, but at 12s you want a lower one like 170
```

---
## \#5 Posted by: pat.speed Posted at: 2017-12-13T09:03:37.863Z Reads: 182

```
Ummm 10s and 230kV is over the erpm limit. You should stay under 60k with that setup max is 66k
```

---
## \#6 Posted by: Luuke Posted at: 2017-12-13T09:50:16.777Z Reads: 170

```
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":230,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":32,"wheel-size":80}|
Yeah, you are right!
I just checked it with this tool. But ERPM is calculated with 3,7V per Cell, not 4,2V
This leads to a max ERPM of 68k. But since you will never reach 100% of the theoretical Motor speed, that's still ok. You just have to take care at the bench, where you have no load. But you can solve that by limiting the ERPM to 60k for the VESC.<img src="/uploads/db1493/original/3X/b/a/babf89d26b454eb9232e2968455a8fd90843f6b7.jpg" width="690" height="157">
```

---
## \#7 Posted by: ATLesk8 Posted at: 2017-12-13T12:48:59.983Z Reads: 144

```
I've only got a few belt drive boards but my motors are 190kv at 10s3p and it runs like a champ with no lack of hill climbing torque and no signs of heat
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-12-13T12:56:08.841Z Reads: 143

```
Killer Velociraptors are my favorite KV. 
<img src="/uploads/db1493/original/3X/3/f/3f2c9ed59dae4af6bbc912246e4c6be6cd9b4c3c.jpg" width="625" height="500">

But i'll settle for 190 if i have to.
```

---
## \#9 Posted by: saul Posted at: 2017-12-13T15:24:37.780Z Reads: 130

```
[quote="Luuke, post:1, topic:40892"]
about to order one custom 6374 KV motor
[/quote]

I'm pretty sure the min is 50x-100x for custom kv.
but if you're going for it. try something different.
plenty of 170, 190, 200, 245....
maybe like 220. or 140...
and of course there is delta vs wye. 
almost all motors are delta...
```

---
## \#10 Posted by: Luuke Posted at: 2017-12-15T16:04:16.126Z Reads: 109

```
Good argument!
So 220KV would be the best option!
```

---
## \#11 Posted by: Mathias Posted at: 2017-12-15T17:38:48.648Z Reads: 100

```
Not necessarily. This limit is only for not destroying your VESC. What the optimum KV for you is is defined by how fast you want to go. Choosing a too high KV will mean that your motor runs too slow / at a too high torque load and that will lead to a significant decrease of your range since the efficiency is low! 
A custom motor puts you in a good position. Most motors that you can buy off the shelf have way too high KV for typical ESkate gear reductions. Then people have to get tiny motor pulleys, which leads to skipping belts and so on and so forth. 

You should decide for a gear ratio with a decent number of motor pulley teeth. Then decide for a top speed, and calculate what KV you need assuming that this speed is about 90% of the no load speed of your motor at the voltage that you use. This way you get a perfect torque-speed balance. Even if you live in a flat area and you think you don't need a lot of torque, a low KV motor will run more efficiently because it runs closer to the no load speed, and you'll get the maximum range out of your battery.
```

---
## \#12 Posted by: uigiroux Posted at: 2017-12-30T19:36:41.726Z Reads: 67

```
How are you able to order a custom 6374???  Can you choose also between delta and wye?  Ohhh please tell me this is possible...
```

---

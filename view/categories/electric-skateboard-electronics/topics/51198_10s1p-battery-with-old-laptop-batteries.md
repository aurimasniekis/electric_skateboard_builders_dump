# 10s1p battery with old laptop batteries

### Replies: 17 Views: 952

## \#1 Posted by: MaxMalouf Posted at: 2018-04-04T10:25:17.798Z Reads: 174

```
Hi all,

Over the past few days, I've made a very simple 10s1p battery pack out of old 18650 batteries mainly for testing purposes and a bit fun. 
I am using an old BMS. 
8 out of the 10, 18650's are the same type of battery and came from the same laptop battery. The last 2 batteries came from a different battery are a different type. 
with 2 batteries being different from the other 8, I am finding when charging the pack, that those 2 batteries get overcharged up to 4.30v and the other 8 cells are at 4.10v.
is this a broken BMS?
or does your battery pack have to be made out of cells that are the same?

Thank you in advance, Max.
```

---
## \#2 Posted by: Acidfie Posted at: 2018-04-04T10:29:27.548Z Reads: 167

```
they should be the same
```

---
## \#3 Posted by: MaxMalouf Posted at: 2018-04-04T10:34:20.022Z Reads: 163

```
dam, that's a bummer, alright thanks
```

---
## \#4 Posted by: Pedrodemio Posted at: 2018-04-04T10:41:25.944Z Reads: 158

```
Do they have any numbers on letters on the side? Laptops battery have very low discharge on most cases, in a 1P setup it may not be enough to get to any meaningful speed

And what Esc are you using?
```

---
## \#5 Posted by: Apolo Posted at: 2018-04-04T10:49:18.794Z Reads: 141

```
There's no way you can use laptop batteries
```

---
## \#6 Posted by: TarzanHBK Posted at: 2018-04-04T11:17:57.271Z Reads: 136

```
Most of Laptop batteries are about 5A discharge. With 1p, well your discharge is 5A (under best condition, more like 3A because of old batteries). I don´t think i could even accelerate with this pack, if i´d stay in the limits.

I think you used an ESC with much higher settings and just killed the cells..
```

---
## \#7 Posted by: MaxMalouf Posted at: 2018-04-04T11:17:59.357Z Reads: 129

```
Mainly for testing purposes.
```

---
## \#8 Posted by: MaxMalouf Posted at: 2018-04-04T11:19:13.807Z Reads: 126

```
I haven't used the pack yet. I have a vesc.
```

---
## \#9 Posted by: TarzanHBK Posted at: 2018-04-04T11:21:21.268Z Reads: 120

```
Don´t use it than. Or set the vesc to 3A and see how that goes, you most likely won´t kill the pack this way.. but man.. just use them for a powerbank or something!
```

---
## \#10 Posted by: MaxMalouf Posted at: 2018-04-04T11:21:50.311Z Reads: 115

```
yeah gotcha hahaha
```

---
## \#11 Posted by: pat.speed Posted at: 2018-04-04T11:40:28.203Z Reads: 103

```
I’d say your bms does not balance the cells or if it does the balance voltage is 4.35v which is common for a Chinese bms
```

---
## \#12 Posted by: Acido Posted at: 2018-04-04T11:55:42.985Z Reads: 96

```
Laptop batteries have a very low discharge rate, too low for eskate
```

---
## \#13 Posted by: Apolo Posted at: 2018-04-04T13:17:43.141Z Reads: 81

```
You won't even be able to properly test a motor with it
```

---
## \#14 Posted by: krloz Posted at: 2018-04-04T13:45:06.837Z Reads: 70

```
I feel like people are nor reading this part at all

[quote="MaxMalouf, post:1, topic:51198"]
mainly for testing purposes and a bit fun.
[/quote]

He's not using it in An esk8. And he certainly won't be if at all he tries.
On the other hand.  With different cells you won't get a balanced pack obviously. You might have a faulty bms or maybe it's simple that bms is set up to overcharge protect ayy 4.3 (imo way high to be safe). One thing you could try is charging the pack was way slower. Like at 0.1A or 0.05A to give the bms more time to balance
```

---
## \#15 Posted by: Namasaki Posted at: 2018-04-06T00:46:57.371Z Reads: 58

```
As mentioned by @Apolo and @TarzanHBK , Laptop batteries are too low output for esk8. 
They would not be adequate even for testing, especially a 1p pack.
Also charging cells to 4.3v can be dangerous.
And taking a battery designed to deliver 3-5a and trying to pull 30a from it might cause the cell to overheat to the point that they go into thermal runaway. If that happens, you better have a fire extinguisher handy.

If you are just practicing battery building, then they are fine for that but don't try to test it with an esk8.
```

---
## \#16 Posted by: b264 Posted at: 2018-04-06T00:49:20.781Z Reads: 55

```
[quote="Apolo, post:5, topic:51198, full:true"]
There’s no way you can use laptop batteries
[/quote]

There certainly is -- if you use at least 72 of them in a 6S12P setup
```

---
## \#17 Posted by: Fiori Posted at: 2018-04-06T01:23:38.778Z Reads: 49

```
The BMS(or most of them) doesn't usually balance the cells super quickly. You should manually balance all of them individually, and then test again(generally you would do this before building the pack..).
```

---

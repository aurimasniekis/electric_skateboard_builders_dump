# Are esk8 calculators wrong?

### Replies: 8 Views: 758

## \#1 Posted by: Aborn Posted at: 2017-09-08T16:05:42.964Z Reads: 130

```
I'm a bit confused, i'm looking to find out whether i should get a 36, 38 or 40T wheel pulley with a 15T motor pulley.

I've used this calculator: http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":85,"motor-pulley-teeth":15,"wheel-pulley-teeth":38,"wheel-size":97}|

But i've noticed it calcuates the rpm with Nominal Voltage * motorKV

The nominal voltage of a li-ion cell being 3.6 V

But, a fully charged cell is 4.2 V which would mean my topspeed on a fully charged battery is a lot higher than what this calculator tells me right?

[36V 37 km/h topspeed(weighted) ](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":10,"motor-kv":190,"system-efficiency":75,"motor-pulley-teeth":15,"wheel-pulley-teeth":38,"wheel-size":97}|)

[43V 44 km/h topspeed(weighted)  (closest i could get to 42V)](http://calc.esk8.it/#{"batt-type-lipo":0,"batt-cells":12,"motor-kv":190,"system-efficiency":75,"motor-pulley-teeth":15,"wheel-pulley-teeth":38,"wheel-size":97}|)

I feel like the calculator is misleading, if i can actually go 7 km/h faster than what it tells me, given that my battery is fully charged?

I do know that voltage sac is not taken into account, but i dont know by how much, and my point should still stand.
```

---
## \#2 Posted by: Boardnamics Posted at: 2017-09-08T16:11:15.223Z Reads: 121

```
It uses nominal as a good indicator. Of course you will go faster in full charge but I wouldn't be worried. Nominal voltage will be closest to your average voltage throughout the cycle. Not to mention voltage sag
```

---
## \#3 Posted by: BigBoyToys Posted at: 2017-09-08T16:21:23.997Z Reads: 104

```
All my boards go slightly slower than the calcuator predicts even at full charge.
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2017-09-08T16:27:11.700Z Reads: 96

```
[quote="BigBoyToys, post:3, topic:32626"]
All my boards go slightly slower
[/quote]

I wonder why big boy? Hahahah lol JK I couldn't resist I'm an ass I know
```

---
## \#5 Posted by: Jinra Posted at: 2017-09-08T16:34:48.905Z Reads: 88

```
Check out discharge graphs for pretty much any cell. You'll see that with even smaller current draw, the cell instantly sags a fair bit lower than 4.2v/cell. Nominal is a better measure of speed even at full charge.
```

---
## \#6 Posted by: NickTheDude Posted at: 2017-09-08T16:36:13.545Z Reads: 88

```
It also doesn't take into account that the maximum duty cycle for the VESC is 0.95.
```

---
## \#7 Posted by: jmasta Posted at: 2017-09-08T16:38:54.828Z Reads: 85

```
They're not wrong. They are a simple guess. And they are a pretty good one at that.

The efficiency parameter is just a fudge factor. We use these kinds of scaling factors in engineering all the time. Is it 100% accurate? Absolutely not. But it works 

When I was designing my board, I derived my own calculator similar to what you see online. However I mistakenly used full 4.2V voltage and my calculations were way off. Using nominal voltage with a 80% efficiency provides a much better estimate. You can go ahead and use 4.2V, but you will be wrong, just like I was :smile:
```

---
## \#8 Posted by: BigBoyToys Posted at: 2017-09-08T16:39:00.349Z Reads: 79

```
U got me there hahaha
```

---

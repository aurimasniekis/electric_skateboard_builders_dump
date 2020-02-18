# What is motor efficiency?

### Replies: 20 Views: 3069

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-11-24T05:07:34.653Z Reads: 295

```
What is motor efficiency?
As seen below:
http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html
```

---
## \#2 Posted by: JuniorPotato93 Posted at: 2016-11-24T07:14:32.294Z Reads: 289

```
Well the technical answer is the mechanical work output divided by the electrical power input, due to friction losses and internal resistances and lots of other things, the mechanical work out is always less.
```

---
## \#3 Posted by: IDVert3X Posted at: 2016-11-24T09:32:28.203Z Reads: 276

```
Belts have high efficiency (90-98%, usually 95%).
I prefer to use 92% for my calculations.
```

---
## \#4 Posted by: saul Posted at: 2016-11-24T10:42:41.424Z Reads: 262

```
but for accurate speed calc you need to account for road friction, wind, rider weight, imperfect alignment...

based on the various setups i've tried by swapping motors/batteries/wheels/drive ratios and comparing with predicted results aka science,  70 - 80% is the way to go for single drives... 92% is optimistic...and just crazy if you were selling based on that...
```

---
## \#5 Posted by: IDVert3X Posted at: 2016-11-24T10:46:48.234Z Reads: 249

```
I said 92% just for the belts, not for the whole setup. Of course you need to count in many other variables.
```

---
## \#6 Posted by: saul Posted at: 2016-11-24T10:59:35.897Z Reads: 238

```
and this is why i added some more variables, dont want newbies to think hubs are 100% efficient because they have no belts. lol
```

---
## \#7 Posted by: Eboosted Posted at: 2016-11-26T08:06:02.526Z Reads: 204

```
Have you messured the efficiency of a system with dual motors?, I wonder if the efficiency will be the same as in single setups.
```

---
## \#8 Posted by: NewbieBoardBuilder Posted at: 2016-11-27T05:12:39.673Z Reads: 196

```
[quote="JuniorPotato93, post:2, topic:13577"]
mechanical work output divided by the electrical power inpu
[/quote]

I don't get this... is this an equation?
```

---
## \#9 Posted by: JuniorPotato93 Posted at: 2016-11-27T05:32:44.762Z Reads: 186

```
Yes it is.  It's a fairly well known one in mechanic engineering in terms of motor or electrical/mechanical  efficiency
```

---
## \#10 Posted by: NewbieBoardBuilder Posted at: 2016-11-27T05:44:05.538Z Reads: 181

```
Can you repeat the equation in a mathematical terms equation? Like x/y=z
```

---
## \#11 Posted by: saul Posted at: 2016-11-27T05:55:08.707Z Reads: 176

```
I have only ran single. dual should be more efficient, especially for heavy riders (i'm only about 160lb). but can be geared for higher speed instead.
in the end gearing is the biggest factor.
```

---
## \#13 Posted by: NewbieBoardBuilder Posted at: 2016-11-27T06:02:13.454Z Reads: 170

```
[quote="JuniorPotato93, post:2, topic:13577"]
mechanical work output divided by the electrical power input,
[/quote]

Can you repeat the equation in a mathematical terms equation? Like x/y=z
```

---
## \#14 Posted by: wmj259 Posted at: 2016-11-27T08:11:39.140Z Reads: 160

```
There is actually not much of an equation for mechanical efficiency as it is unitless,  times 100%to get a percentage 
ME=(Mechanical Work Output) /(electric energy entered) *100%
```

---
## \#15 Posted by: JuniorPotato93 Posted at: 2016-11-27T16:48:15.158Z Reads: 149

```
Efficiency  = (mechanical work out , Watts) / (electrical work in,  Watts)
```

---
## \#16 Posted by: wmj259 Posted at: 2016-11-27T16:50:21.991Z Reads: 147

```
That would give you an efficiency over 100%. You will be putting in more electrical work to get less mechanical work out.
```

---
## \#17 Posted by: JuniorPotato93 Posted at: 2016-11-27T16:57:03.347Z Reads: 142

```
Yes,  you're a right it's the inverse of what I wrote.  Let me update that.
```

---
## \#18 Posted by: NewbieBoardBuilder Posted at: 2016-11-27T19:06:35.884Z Reads: 140

```
So what is the true equation then?
```

---
## \#19 Posted by: wmj259 Posted at: 2016-11-27T19:18:42.262Z Reads: 136

```
What me and @JuniorPotato93 wrote, 

Since you have watt divided by watt,  it becomes unitless,  so basically it becomes a ratio of comparison of what is less efficient to what is 100% efficient if the motor output exactly what was inputted. 
The best way to use this formula would be through experimental data of inputting a certain amount of energy/power from the battery and measuring on a dynamo type machine what the output is.
```

---
## \#20 Posted by: wmj259 Posted at: 2016-11-27T19:21:42.717Z Reads: 136

```
Basically it won't be 100% or even close to 95-96% if we consider air resistance frictional yadayadayada.... So far the only thing even close to 100% efficiency would be a resistance heater used to heat homes. Which come close to 99-99.99%
```

---
## \#21 Posted by: EnderWiggin Posted at: 2016-12-01T08:41:58.982Z Reads: 132

```
Hey Newbie If you look at my spread sheet I made, the equation for efficiency in that is correct but it is also theoretical. Real motor efficiency depends on many different factors. This is still a questions that I have not answered very well in the spread sheet yet. 
E% = (Pout / Pin) *100   or E% = Wout / Win
Ex. 800/1000=.8 -> .8*100 = 80% efficient
Pout = τ * ω
Pin = I * V
so 
if 100% efficiency  Pout = Pin or  τ * ω = I * V

Pout – output power, measured in watts (W);
Pin – input power, measured in watts (W);
I – current, measured in amperes (A);
V – applied voltage, measured in volts (V).
τ – torque, measured in Newton meters (N•m);
ω – angular speed, measured in radians per second (rad/s).
Resource: [Simple Motor Calculations](http://simplemotor.com/calculations/)
Let me Know if you have any more questions.
```

---

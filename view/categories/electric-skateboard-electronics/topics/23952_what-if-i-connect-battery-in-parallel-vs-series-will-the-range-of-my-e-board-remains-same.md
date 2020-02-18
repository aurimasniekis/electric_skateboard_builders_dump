# What if i connect battery in parallel vs series. will the range of my e board remains same?

### Replies: 16 Views: 910

## \#1 Posted by: Monty Posted at: 2017-05-26T17:20:53.512Z Reads: 135

```
I have issue rewarding this i have 4pc 3s 5000mah lipo i am connecting them in series to make 12s pack but the capacity will remain same but in parallel capacity will 4 Times  so both will give me same range or diff . . Urgent help pls
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-26T17:29:59.280Z Reads: 135

```
3s I too low voltage for E-boards. 
And to answer your question, yes your range will not increase if you take from voltage and give it to capacity.  Or visa Versa. 
I have actually tested this theory and here are my results:
12s / 5ah = 10 miles
6s / 10ah = 10 miles

This test was based on same riding conditions and style
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-05-26T17:32:30.982Z Reads: 133

```
12S will give you a 4 times higher speed than 3S. But let's say you ride with the 12S only the same speed. Then the 3S will give you a tiny little bit less range because the 4 times higher current heats up the battery cables from the battery to the ESC. But 3S isn't usable. 6S would be more practice. 

In reality the 12S system will be less efficient because with the higher speed you will ride the board harder faster. 

It's the same with single and dual drive. People think the dual drive needs 30% more energy but in reality they ride a dual drive much harder which results in a higher energy consumption.
```

---
## \#4 Posted by: Vaulter92 Posted at: 2017-05-26T20:06:31.501Z Reads: 104

```
Someone at my university is riding 3s with a 25 bucks hobby king car ESC for 1.5 years now and he is fine with that.
I would make it dependent on your desired velocity.
```

---
## \#5 Posted by: Bataleon Posted at: 2017-05-26T20:10:19.831Z Reads: 99

```
That's awesome. Do you know what motor and gear ratio he is running?
```

---
## \#6 Posted by: Vaulter92 Posted at: 2017-05-26T21:13:59.966Z Reads: 92

```
I don't know about the hearing ratio.
He printer the pulleys and the motor mount though. It's some 5055 motor but he rewound it so no clue about the kv
```

---
## \#8 Posted by: Bataleon Posted at: 2017-05-26T22:15:19.690Z Reads: 81

```
I run 10s and wouldn't want anything less. But it's awesome how builders can piece together an eBoard that works for their situation, in the above instance: a cash-strapped student needing something to get him around university campus. Beats an old shitty car any day.
```

---
## \#9 Posted by: Namasaki Posted at: 2017-05-26T22:17:00.362Z Reads: 78

```
oops, my mistake, I though you where the guy asking about putting his 4 3s lipos in parallel.
```

---
## \#10 Posted by: Bataleon Posted at: 2017-05-26T22:18:32.415Z Reads: 74

```
Nope, I'd rather run them in series :smile:
```

---
## \#11 Posted by: Namasaki Posted at: 2017-05-26T22:22:01.940Z Reads: 68

```
I heard that,
I'm running 10s now and it's kinda mellow after running 12s with dual direct drives.
```

---
## \#12 Posted by: Monty Posted at: 2017-05-27T21:49:41.241Z Reads: 49

```
How to do that?
```

---
## \#13 Posted by: Monty Posted at: 2017-05-27T21:56:54.319Z Reads: 51

```
I read some one said that the range remain same but actually what hapen if i am on 6s 10000mah lipo and my speed is  20kmph then on 12s 5000mah lipo my speed is double 40kmph then i will able to cover same distance with high speed hence the speed will remain  same.
 6s =20kmph complete 10 miles in 1 hr.
12s =40kmph complete 10 miles in 30 min
```

---
## \#14 Posted by: Namasaki Posted at: 2017-05-27T23:14:44.086Z Reads: 49

```
Your distance is determined by watt hours available and watts drawn. 
Watts= voltage x amps 
Watt hours= voltage x amp hours
50v x 5ah =250 watt hours
25v x 10ah = 250 watt hours 
This is why, when you take away volts to increase amps, the song remains the same. 
6s full throttle will be like 12s at half throttle. 
Naturally if you run 12s at full throttle, you will be drawing more watts. Except for other factors that weigh in like momentum.  Momentum will help you to use less watts if your on flat ground and not riding against a strong wind.
```

---
## \#15 Posted by: Monty Posted at: 2017-05-28T03:39:33.164Z Reads: 42

```
I want 40 km range board any idea how.much mah pack in nees of 12s
```

---
## \#16 Posted by: Namasaki Posted at: 2017-05-28T03:49:29.395Z Reads: 42

```
40km or 24miles is a lot of range.
It will depend on many factors, your weight, riding conditions, riding style, gearing, voltage sag
I can only guess based on my own experience.
So here is my best guess for 40km or 24mi
12s and 10ah might get it with a belt drive and battery capable of at least 125a continuous
```

---
## \#17 Posted by: laurnts Posted at: 2017-05-28T03:58:09.544Z Reads: 39

```
What Namasaki said its true, distance = power = watt (voltage x mah). As simple as that.
However If i am not mistaken, running on full erpm are quite known to be efficient as BLDC motor benefits from that.
```

---

# I think I made my first build mistake

### Replies: 20 Views: 1278

## \#1 Posted by: Mattmccrary8 Posted at: 2017-04-05T12:04:49.451Z Reads: 158

```
I changed up my initial build and bought 2x5000mah5s batteries making it a 10s batt. I bought a turning 260kv motor which is going to fry my TB VESC isn't it? Should I wait to run it or buy a different out runner?
```

---
## \#2 Posted by: Mattmccrary8 Posted at: 2017-04-05T12:05:11.304Z Reads: 159

```
I don't want to fry everything is there any safe way to run this?
```

---
## \#3 Posted by: krloz Posted at: 2017-04-05T12:12:46.169Z Reads: 151

```
Not an expert here but the common practice is to limit Max and min(negative) erpm to 60000 (this is a safe value) on the bldc tool.
At least for starters. Anyone else want to weigh in?
```

---
## \#4 Posted by: Mattmccrary8 Posted at: 2017-04-05T12:25:39.999Z Reads: 140

```
Ya I've read about that but once I do that wouldn't the motor be pointless, I'd lose all speed and stuff limiting that? I was wanting to get 25-30mph that's why I went with the 260kv

I'm completely new to all of this so bare with me lol
```

---
## \#5 Posted by: flatsp0t Posted at: 2017-04-05T12:46:56.004Z Reads: 120

```
Yes, you will need a different motor. 190kv is the max you can safely run on 10s.
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-04-05T12:47:10.698Z Reads: 118

```
like @krloz mentioned, you could limit erpm to 60.000 and will be fine.
But a 190KV would be optimal
```

---
## \#7 Posted by: arussellsaw Posted at: 2017-04-05T12:49:03.512Z Reads: 115

```
i have a 245kv with 10s (2x zippy 8000mah 5s) that i'm about to build, what is the risk here? providing i limit my erpm?
```

---
## \#8 Posted by: flatsp0t Posted at: 2017-04-05T12:50:06.517Z Reads: 111

```
Well, if you coast over 60k erpm downhill you could still fry your vesc.
```

---
## \#9 Posted by: arussellsaw Posted at: 2017-04-05T12:52:35.048Z Reads: 112

```
how does coasting factor battery in? would coasting above 60k erpm fry the vesc regardless of battery?
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-04-05T12:52:42.522Z Reads: 108

```
you have to tick "limit erpm with negative torque" to avoid that. That way the vesc starts braking not not exceed that limit
```

---
## \#11 Posted by: arussellsaw Posted at: 2017-04-05T12:54:17.139Z Reads: 105

```
does anyone know what calculations i'd need to do to work out the speed at which i'd hit 60k erpm? 

i have 80mm wheels, 36t wheel 16t motor

does the motor factor in? it's a 245kv SK3, will have to find out how many poles
```

---
## \#12 Posted by: flatsp0t Posted at: 2017-04-05T12:55:57.875Z Reads: 101

```
Well, then cou cant go faster even downhill.
BORING.
And also not really safe.
If i remember correctly i saw someone who broke his vesc downhill anyways.  Because it coud not keep it below 60k and fried while braking.
```

---
## \#13 Posted by: flatsp0t Posted at: 2017-04-05T12:56:22.293Z Reads: 99

```
7 pole pairs.
```

---
## \#14 Posted by: arussellsaw Posted at: 2017-04-05T12:56:52.877Z Reads: 96

```
i live in London, so not a lot of huge hills. it'll mostly be flat or gentle hills
```

---
## \#15 Posted by: mmaner Posted at: 2017-04-05T12:57:08.924Z Reads: 93

```
[quote="arussellsaw, post:11, topic:20345"]
does anyone know what calculations i'd need to do to work out the speed at which i'd hit 60k erpm?
[/quote]



http://calc.esk8.it
```

---
## \#16 Posted by: arussellsaw Posted at: 2017-04-05T13:00:32.215Z Reads: 90

```
thanks @mmaner i'd looked at  that before but never noticed erpm

http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":10,"motor-kv":245,"system-efficiency":80,"motor-pulley-teeth":16,"wheel-pulley-teeth":36,"wheel-size":80}|

looks like i would hit 30mph weighted at ~63k erpm. that seems plenty to me.

it will be interesting to discover how effective braking is with a single 245kv motor
```

---
## \#17 Posted by: TarzanHBK Posted at: 2017-04-05T13:01:14.876Z Reads: 86

```
of course that could happen if you go downhill like a pro.
It´s not the best solution, but if you stay in standard speeds and won´t buy a new motor it should work.

Best idea would be a suiting motor.

https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#18 Posted by: krloz Posted at: 2017-04-05T14:32:52.610Z Reads: 71

```
If you go to a lower kv motor to be safe about the erpm you Will have to adjust gearing if You want to keep the Max speed as a 190kv motor Will be slower at the same S count. But doing this you Will be able to reach Max speed without hiting erpm limit. Anyway set the limits and tick negative Torque as you could still damage the vesc going downhill with a 190kv. I guess
```

---
## \#19 Posted by: Bazingazunga Posted at: 2017-04-05T14:47:23.668Z Reads: 64

```
To echo everyone else and put it in laymans terms:

If you limit the ERPM to 60,000 your VESC will be fine. It stops it you from going too fast to fry it.
Larger kv motor's are able to go faster, with the sacrifice of torque.
By limiting your ERPM, you lose this benefit, whilst not having the benefit of low end torque (due to a high kv).


But yes, if you limit the ERPM you will not fry your VESC.
```

---
## \#20 Posted by: Mattmccrary8 Posted at: 2017-04-05T16:06:28.415Z Reads: 49

```
Ya I just ordered a 190kv motor from TB.
```

---

# What do you guys think of this Motor-Battery-Mount Solution?

### Replies: 7 Views: 723

## \#1 Posted by: Geddi Posted at: 2017-04-03T21:02:25.552Z Reads: 168

```
I was thinking about going for a single motor build. 
8s Battery setup
Turnigy Aerodrive SK3 - 6354-260kv
VESC
If I limit the erpm to 60000 then I want my topspeed to be arround 8000 rpm. 
8000 / 260kv = 30.76V
With my battery Setup I get 8*3.7 =29.9V.
This way I still have a saftey net. And 8s should be fine with the vesc right? I know 10s is recommend, but 10s really doesnt fit a build with a tight budget. I was going for 12s initially, but then I would have to come up with a different charging solution.
Am I thinking this the right way?
```

---
## \#2 Posted by: saul Posted at: 2017-04-03T22:25:09.359Z Reads: 144

```
I have 8s with 245. I would not go any higher in kv. lower is actually better. around 200kv.
topspeed depends on rpm, gear ratio,wheels, so 8krpm means nothing lol.

8s with a balance charger works, but you still need at least 50A cont. battery.
[8s build #1](http://esk8.today/guides/build-guide/)
```

---
## \#3 Posted by: Geddi Posted at: 2017-04-03T22:56:51.946Z Reads: 130

```
Well,

260kv * 28.8v = 7488rpm = 52416erpm 
I will use 32 tooth wheel pulley and 15 tooth motor pulley and 83mm wheels.
The continous output for lipo's is ah * C rating and that would be 5*25= 125. 
Please tell me if I am doing this completely wrong
```

---
## \#4 Posted by: aha_96 Posted at: 2017-04-03T23:15:46.377Z Reads: 115

```
Sounds about right! 25C batteries are perfectly fine for your build
```

---
## \#5 Posted by: IsTalo Posted at: 2017-04-03T23:23:44.916Z Reads: 111

```
6354 isn't small for a single drive?
```

---
## \#6 Posted by: saul Posted at: 2017-04-04T07:44:34.480Z Reads: 86

```
[quote="Geddi, post:3, topic:20218"]
260kv * 28.8v = 7488rpm = 52416erpm I will use 32 tooth wheel pulley and 15 tooth motor pulley and 83mm wheels.The continous output for lipo's is ah * C rating and that would be 5*25= 125.
[/quote]

yes looks right, check my site for calculators, i walked throught some calculations also.[quote="IsTalo, post:5, topic:20218, full:true"]
6354 isn't small for a single drive?
[/quote]
its fine, unless you are a very big rider >250lb.
and more portable, 6374 is almost a pound more weight.
```

---
## \#7 Posted by: Namasaki Posted at: 2017-04-09T23:18:39.709Z Reads: 60

```
When you calculate for erpm limit. You need to use full charge voltage of 4.2v per cell.
8s x 4.2 = 33.6v x 260kv= 8736rpm x 7= 61152 erpm
33.6v x 245kv=8232rpm x 7=57624 erpm
It is my understanding the lower KV produces more torque so you could very well wind up getting equal or better performance with the 245kv. and not have to worry about the erpm limit.
```

---

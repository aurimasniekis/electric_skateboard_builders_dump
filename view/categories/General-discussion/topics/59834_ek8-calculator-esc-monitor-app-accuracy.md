# Ek8 Calculator / ESC Monitor App accuracy

### Replies: 10 Views: 473

## \#1 Posted by: DavidBanner Posted at: 2018-06-23T15:47:41.074Z Reads: 120

```
How accurate have you found the esk8 calculator and the ESM monitor app to be ?

Here is the calculator which my specs
http://calc.esk8.it/#{%22batt-type-lipo%22:1,%22batt-cells%22:10,%22motor-kv%22:190,%22system-efficiency%22:90,%22motor-pulley-teeth%22:15,%22wheel-pulley-teeth%22:60,%22wheel-size%22:152}|

the calculator is saying my top speed should be 28.16 mph weighted. 

Now I just took my new build out for a test run and the ESC Monitor App is saying I hit 28.5 mph and I wasn't really pushing the board which felt like it had a whole lot more left in it.

I am wondering how closely the calc is to real world performance? Or possibly the ESC monitor App isn't accurate?
```

---
## \#2 Posted by: BoostedBuilder Posted at: 2018-06-23T15:50:24.106Z Reads: 109

```
Did you use 90% efficiency? Pretty accurate for my boards at 85%.
```

---
## \#3 Posted by: DavidBanner Posted at: 2018-06-23T15:51:36.218Z Reads: 106

```
I actually bumped it up to 90% as the figures seem too low
```

---
## \#4 Posted by: professor_shartsis Posted at: 2018-06-23T16:05:02.341Z Reads: 94

```
it would appear the ESK8 calc simply multiplies the calculated no load speed times whatever % you choose for “efficiency...”

so if you choose 90% efficiency, the weighted speed shows 90% of the no load speed.

this is technically a different meaning of efficiency than mechanical watts / electrical watts = conversion efficiency %

you can set the weighted speed to any value between 0 and no load speed by setting the “efficiency” value to any desired % value...
```

---
## \#5 Posted by: jens_c Posted at: 2018-06-23T17:15:14.024Z Reads: 74

```
if your battery's are fully charged you get an extra 5 v thats problably why

sorry for bad english
```

---
## \#6 Posted by: Ackmaniac Posted at: 2018-06-23T17:20:41.477Z Reads: 71

```
Your top speed is is most dependent on your motors kv. So if you easily reached 28 mph then it could be that there is the end. Of course downhill is a little more possible but if you change your gearing you would reach 35 mph easily.
The motor can only produce power when it is feed with a higher voltage than the motor is already running with. If that voltage is already reached then it can't produce any more and vice versa can't go faster.
```

---
## \#7 Posted by: Battosaii Posted at: 2018-06-23T18:55:16.565Z Reads: 56

```
Yea calculator said my set up with 16/60 pullies on 6 shooters top speed is 32mph but my GPS said I topped out at 37mph and got over 30 regularly. It's a bit off for me too
```

---
## \#8 Posted by: DavidBanner Posted at: 2018-06-23T19:06:28.732Z Reads: 48

```
@Battosaii thanks for the info. it's good to know I am not the only one.

From my testing today I think this board could easily do 35 mph, I was deliberately taking it easy as it was the first proper test run and I wanted to limit the speed in case of failure.
```

---
## \#9 Posted by: Battosaii Posted at: 2018-06-23T19:08:44.705Z Reads: 43

```
Haha yea best to take it easy I didnt try to top out till my 3rd or 4th ride with no problems I between.
```

---
## \#10 Posted by: mccloed Posted at: 2018-06-23T20:20:41.629Z Reads: 37

```
Another factor would be BLDC vs FOC. I usually bring the efficiency down to 80 - 85% for FOC,  as you loose a little top end. The calculator listed in the first post seems to be pretty accurate with my current set-up.
```

---

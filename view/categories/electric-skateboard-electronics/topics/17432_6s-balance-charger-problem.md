# 6s balance charger problem?

### Replies: 6 Views: 484

## \#1 Posted by: nick191 Posted at: 2017-02-09T07:01:11.455Z Reads: 43

```
hi all i have got a new balance charger for my 3s 500mAh turnigy 20-30c lipo and it says 11.1 volts on the battery. my charger says shut off at 5000mAh which is good but is says end voltage 12.6 and thats way over is it good what im doing i dont want to do it too much i haven't let it go till shut off just 11.1 any recommendations.
```

---
## \#2 Posted by: Alextech Posted at: 2017-02-09T07:04:43.626Z Reads: 43

```
It goes off nomial Voltage, In this case 3.7v (LiPo) 3.6v (Lion) 3.3v (LiFe) Your Charger is fine! Its suppost to charge to a Lipo's Max Voltage (4.2V) so you take 4.2v x 3 = 12.6v
```

---
## \#3 Posted by: nick191 Posted at: 2017-02-09T07:06:26.979Z Reads: 42

```
so leave it and charge it right up until it shuts off
```

---
## \#4 Posted by: Alextech Posted at: 2017-02-09T07:07:59.868Z Reads: 36

```
Well a good rule of thumb is always monitor Lipo's when charging. Keep an eye out for Puffying this a sign of a bad battery or Charger, But your charger is doing its Job.
```

---
## \#5 Posted by: nick191 Posted at: 2017-02-09T07:09:07.612Z Reads: 32

```
thanks heaps
```

---
## \#6 Posted by: treenutter Posted at: 2017-02-09T20:01:39.790Z Reads: 16

```
@nick191 You can also program it to charge below 4.2 if you want; it will extend battery life. Look up "discharge curve" for LIPOs and you'll see that you get very little out of a full charge to 4.2. Most of your usage will be at the nominal voltage. Also, if you're using an ESC w regen braking, charging below your max voltage will help to avoid triggering a shutoff due to ovecurrent.
```

---

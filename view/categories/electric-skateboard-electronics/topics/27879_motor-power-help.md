# Motor power help

### Replies: 9 Views: 369

## \#1 Posted by: DaffieT Posted at: 2017-07-17T20:59:40.250Z Reads: 38

```
Hey can anyone help, Im building an e longboard and have been having trouble getting the speed up, I am using two 3s 5000 man lipos and a 6374 190kv motor from torqueboards, and the motor just isn't going fast enough, I am familiar with bdlc tool and have configured it to what i think is correct, any suggestions? More power, different motor, or vesc configuration error?
```

---
## \#2 Posted by: psychotiller Posted at: 2017-07-17T21:06:52.395Z Reads: 37

```
Are you running your batteries in a parallel or series configuration? Also, 190kv isn't going to be fast even if you series up your batteries @6s
```

---
## \#3 Posted by: Martinsp Posted at: 2017-07-17T21:08:32.532Z Reads: 37

```
I suggest you to do the kv math and see if you get the RPM in the realtime data you calculated. If you do then you have to increase voltage to get more RPM. Or if you want more speed you can change your gearing ratio.

Also, post pictures of configuration.
```

---
## \#4 Posted by: DaffieT Posted at: 2017-07-17T21:12:06.836Z Reads: 33

```
Batteries are in parallel, i will post pics in a sec
```

---
## \#5 Posted by: Martinsp Posted at: 2017-07-17T21:15:43.400Z Reads: 32

```
at that low voltage you will get 2394 RPM @4.2V so there is your problem :D
```

---
## \#6 Posted by: DaffieT Posted at: 2017-07-17T21:16:55.865Z Reads: 30

```
so do i just need more power?
```

---
## \#7 Posted by: Martinsp Posted at: 2017-07-17T21:20:08.290Z Reads: 27

```
well more importantly you need more voltage to get more RPM. try connecting the batteries in series (and adjust your values in BLDC correctly) you should get twice the RPM.
```

---
## \#8 Posted by: DaffieT Posted at: 2017-07-17T21:21:19.970Z Reads: 25

```
OK thanks :grinning:
```

---
## \#9 Posted by: Martinsp Posted at: 2017-07-17T21:21:48.743Z Reads: 25

```
No problem :)
```

---

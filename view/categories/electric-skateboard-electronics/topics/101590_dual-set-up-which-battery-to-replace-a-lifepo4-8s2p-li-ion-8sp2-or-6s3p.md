# Dual set-up: Which battery to replace a LiFePo4 8s2p? Li Ion 8sP2 or 6S3P?

### Replies: 12 Views: 180

## \#1 Posted by: PaleRider Posted at: 2019-09-10T16:54:55.341Z Reads: 47

```
Hi,
I have a LiFePo4 8s2p from Leiftech (LT1X 24v) and I want to replace it with a Li Ion Battery. (some says it is a 7s but there is definively 8x2 cells one mine)

Which one would be the best:
a 8s2p a little more powerfull than the original one, or a 6s3p for more range?
Or something else?

My set up is a dual single vesc with 2X 400KV motors.

Thanks for your advices :slightly_smiling_face:

PS: which charger to go with the battery?
```

---
## \#2 Posted by: Sn4pz Posted at: 2019-09-11T17:11:04.167Z Reads: 38

```
To upgrade to any higher battery than what you have currently, youll need to either

a) buy a beefier vesc that will handle higher ERPM (400kv x 8s x 28.8v/ 33.6v is rather unsafe) 

or b

b) Essentially change your entire drivetrain, by buying typically used motors, as well as matching pulleys at their correct gearing and etc

failure to do so will probably result in a broken board, you're currently pushing your hardware pretty hard
```

---
## \#3 Posted by: PaleRider Posted at: 2019-09-11T18:36:00.596Z Reads: 34

```
Actually, my set-up is the original one from Leiftech (the e-Freeboard).

I'm changing it for 2 single vesc Mini 4.20 from Flipsky and that's why I need to change the battery too.
Do you think a 6S would be safer than a 8S?
```

---
## \#4 Posted by: Winfly Posted at: 2019-09-11T18:52:26.160Z Reads: 32

```
Keep in mind that LiFePO4 max voltage is 3.6 whereas li ion 18650 is 4.2. so 6S li-ion will somewhat match your original voltage.

As for erpm 4.20 is vesc4 based probably capped at 60-80k. 

25.2V x400kv x7(assumed 14poles motors) = 70k. 

So I'll keep it at 6S if I were you. 8S with 400kv your mini4.20 will not handle the erpm.
```

---
## \#5 Posted by: PaleRider Posted at: 2019-09-12T12:49:54.661Z Reads: 22

```
And what about a 7S?
```

---
## \#6 Posted by: Winfly Posted at: 2019-09-12T19:38:18.448Z Reads: 19

```
I guess the answer is. you will cap your 4.20 at somewhere between 60-80k erpm and that would be your top speed. you can however go 6-8S if you want. higher S the better. However, you should be aware of the erpm limit behavior of VESC in general so you dont get jerked and fall at highspeed.
```

---
## \#7 Posted by: PaleRider Posted at: 2019-09-12T22:08:35.376Z Reads: 17

```
Ok I understand now.
I should limit the erpm to 60000 in vesc-tool to protect the vesc, but doing this will limit the interest to get a 7s or 8s instead of a 6s (no gain in speed).

I guess the best move would be to change the battery and the motors too.
Getting something with less KV, so I would be able to keep top speed with a 8s and gain some torque (actually there is no torque: you have to push start the board!)
```

---
## \#8 Posted by: Winfly Posted at: 2019-09-12T23:49:50.191Z Reads: 16

```
[quote="PaleRider, post:7, topic:101590"]
limit the interest to get a 7s or 8s
[/quote]

Yes. But going 7S and 8S still has the benefit in range b/c more battery cells and higher voltage = less current draw
```

---
## \#9 Posted by: PaleRider Posted at: 2019-09-13T02:32:24.574Z Reads: 15

```
Which one will have more range between 6s3p and 8s2p?
```

---
## \#10 Posted by: PaleRider Posted at: 2019-09-14T13:02:55.481Z Reads: 12

```
Obviously there is more cells in the 6s3p, but you suggested there is range advantage to a 8S due to the voltage.
More voltage: more speed, but more range too?

Is there any advantage to go 8s2p over 6s3p in my case as I will limit the erpm to 60k?
Thanks.
```

---
## \#11 Posted by: Sn4pz Posted at: 2019-09-14T13:24:50.039Z Reads: 10

```
8s2p gives more torque, but you basically have half the range than if you went 6s3p, and stayed at the same amps. The sag at 8s2p is really gonna be bad, and at some point (probably 25%) you'll just stop riding because it's either too slow, or it's making weird sounds. 

I think 6s3p is the better choice, especially with your current part configuration. If you want to go crazy a 7s4p would give you very satisfactory performance based on what you had previously
```

---
## \#12 Posted by: PaleRider Posted at: 2019-09-14T14:09:38.291Z Reads: 9

```
OK thanks.
I'll go 6s3p.
```

---

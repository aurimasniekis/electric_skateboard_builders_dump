# Same motor, different KV, and different Torque Nm?

### Replies: 8 Views: 903

## \#1 Posted by: thetechtrader Posted at: 2017-11-09T16:08:29.714Z Reads: 109

```
I'm looking at TP Power motors 5870 series, and the guy selling them says the lower KV motors in this series have more MUCH MORE torque.

250kv 6.9NM 100A
330kv 5.4NM 120A
360kv 4.9NM 135A
http://tppower.com/S_UploadFile/20161229104850629.jpg

I thought motors of the same diameter and design had the same Nm no matter the KV?

Question, do lower KV motor with the same diameter and design have more copper and thus they will have more Nm than higher KV to a certain extent? and this is the reason for higher torque?
```

---
## \#2 Posted by: onepunchboard Posted at: 2017-11-09T16:10:32.430Z Reads: 97

```
lower kv gets more torque per amp
```

---
## \#3 Posted by: thetechtrader Posted at: 2017-11-09T16:18:17.841Z Reads: 90

```
yes thank you, and I do get that, but does the same size diameter motor max out at the same total torque Nm no matter the Kv?

250kv version at mad power would still give 4Nm , and so would the 360kv version maxing out at 4Nm?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-11-09T16:21:33.977Z Reads: 83

```
generally lower kv has much torque in low rpm, and brakes. it has thiner copper wire so has more copper mass in same space and make it stronger electro magnet
```

---
## \#5 Posted by: NickTheDude Posted at: 2017-11-09T16:22:15.278Z Reads: 81

```
Some say that since you need smaller wire you're able to fit more copper which would allow you to get more torque output... However I'd look at the listed weight of the motors, if their relatively close to each other I'd assume their torque output would be very similar. However the amperage bottleneck usually isn't the motor, it's the ESC or batteries so in that case you'd be able to get more torque from lower kV.
```

---
## \#6 Posted by: thetechtrader Posted at: 2017-11-09T16:23:26.679Z Reads: 75

```
Thank you guys... Really appreciate it!
```

---
## \#7 Posted by: thetechtrader Posted at: 2019-10-28T01:15:43.571Z Reads: 28

```
New Question on Motor Poles and current, need help understanding please!

Given the same motor dimensions, kv, volts, and propeller/wheel how does the number of poles affect the amps/current under load. 

one motor has 6 poles, the other motor has 10 poles.

how would the 10 pole perform? smoother rotation? more torque for sure, but would it draw less Amps with same load as it does not need to work as hard?
```

---
## \#8 Posted by: Boardnamics Posted at: 2019-10-28T07:23:17.901Z Reads: 23

```
Ehh poles just helps with smoothness of torque delivery. It is somewhat similar to adding more cylinders to a car engine you could say. There is more switching going on.

Adding to the poles increases torque but lowers rpm. So yes it would draw less amps under the same torque load but the overall power output would be the same

Maximum power capability in our brushless motors matters most on overall motor volume more than anything. It's why motors of the same size have very similar power outputs. Build quality and material only yield additional % efficiency and, add reliability too
```

---

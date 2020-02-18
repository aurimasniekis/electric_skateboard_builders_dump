# Fast ramping down in both directions

### Replies: 9 Views: 714

## \#1 Posted by: supernova Posted at: 2016-08-23T21:18:55.898Z Reads: 92

```
Hi,

I have my Vescs for my robot project. I have managed to get reasonable control from them but find that the motor ramps down slowly, this is fine for a board but I would like my robot to change direction faster. Ie when i let go of the throttle i want the wheel to stop spinning quickly. Which setting on the Vesc should I change?

Thanks
```

---
## \#2 Posted by: mishrasubhransu Posted at: 2016-08-23T21:23:10.556Z Reads: 90

```
what sort of control are you using> Current, Duty Cycle, PID velocity?
```

---
## \#3 Posted by: supernova Posted at: 2016-08-23T21:38:41.273Z Reads: 83

```
Hi, I am using current
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2016-08-23T21:42:56.176Z Reads: 82

```
Go to **Motor configuration->advanced->Max Current Ramp Step**(under Backoff and Ramping). Increase that value until you get desired effect. 

What's your present value?
```

---
## \#5 Posted by: supernova Posted at: 2016-08-23T21:51:31.600Z Reads: 75

```
Hi, its currently set at 0.04 (max current ramp step)
```

---
## \#6 Posted by: DeathCookies Posted at: 2016-08-24T06:45:41.606Z Reads: 56

```
[quote="mishrasubhransu, post:4, topic:8194"]
Go to Motor configuration-&gt;advanced-&gt;Max Current Ramp Step(under Backoff and Ramping). Increase that value until you get desired effect.
[/quote]

Does this also results in a punchier / harder / faster acceleration?
```

---
## \#7 Posted by: mishrasubhransu Posted at: 2016-08-24T13:55:33.408Z Reads: 41

```
If it's set to 0.04 at 1Khz(1000Hz) means that at every 1/1000 sec the current can change by a max of 0.04A. So basically if you instantly command a change of  20Amps to the controller it will take 20/0.04 = 500milli second = 0.5 seconds to achieve that commanded current. 

By change in Amps I mean, you could start at 0 Amps and instantly command 20 Amps or you could start at 10 A and instantly command 30A.

So it controls how fast you reach your desired current(in effect acceleration on flat ground).
```

---
## \#8 Posted by: mishrasubhransu Posted at: 2016-08-24T13:57:40.778Z Reads: 41

```
Did it help?
```

---
## \#9 Posted by: supernova Posted at: 2016-08-24T21:12:50.856Z Reads: 32

```
Hi,

I selected duty cycle, and now the ramping is much more aggressive, thanks!
```

---

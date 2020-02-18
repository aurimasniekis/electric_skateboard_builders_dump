# BEMF coupling explained?

### Replies: 5 Views: 899

## \#1 Posted by: DougM Posted at: 2017-10-24T04:42:55.945Z Reads: 102

```
Can anyone explain (or give me a pointer to an explanation) what BEMF Coupling actually is and how I would know what good numbers are vs. bad numbers?

I'd like to know what to look for as I test a batch of motors.

Thank you,
```

---
## \#2 Posted by: Okami Posted at: 2017-10-25T17:23:40.207Z Reads: 77

```
@Hummie or @chaka might know.. Not really knowing about this either, personally :)
```

---
## \#3 Posted by: Hummie Posted at: 2017-10-25T18:09:37.973Z Reads: 70

```
I know what bemf is but would like to know what the coupling is about.  I just do the vesc test and plug in the results without a problem.  I think the coupling number incorporates a lot and would tell you a lot.  I'd like to know!

if you don't know the bemf is the voltage produced by the motor and the faster spinning the higher voltage.  max speed would be your kv times your voltage because the back emf is as high as the input voltage so no more current can flow.   you'd want it to be balanced on all teeth and phases and I'm guessing the coupling is about that.
```

---
## \#4 Posted by: DougM Posted at: 2017-10-25T20:24:32.276Z Reads: 57

```
My best guess is that for a given rotational speed you measure the BEMF voltage returning.  This would allow you to calibrate the input to the ADC on the processor to create a baselilne.

But this is just a guess.
```

---
## \#5 Posted by: Jinra Posted at: 2017-10-25T20:25:56.990Z Reads: 56

```
I bet @Ackmaniac knows!
```

---

# Maytech 6374 170kv spinning both ways?

### Replies: 9 Views: 140

## \#1 Posted by: Nedtrampz Posted at: 2019-06-13T03:59:28.514Z Reads: 50

```
The motor is sensored. It has been set up sensorless due to problem. The setup with sensor was screaming high pitch sounds n lock up so im doing sensorless. 

The motor spins both ways even using current no reverse with brake. Pissing me off i just wanna go ride but scared it will backfire on me.
```

---
## \#2 Posted by: tardyparty7 Posted at: 2019-06-13T04:03:03.430Z Reads: 49

```
can i see pictures of your settings? i don't think it's the motor, you could have some settings wrong.
```

---
## \#3 Posted by: Nedtrampz Posted at: 2019-06-13T04:17:12.848Z Reads: 46

```
Can u suggest what settings maybe wrong? What pages of settings to take pics of? 

As far as i know everything should be fine ive set motors up many times without this trouble. 

Using the new vesc tool which is bit different. But i re did my trampa motors the other day which went fine.
```

---
## \#4 Posted by: Skunk Posted at: 2019-06-13T04:24:34.618Z Reads: 44

```
So your non sensored set up spins both directions? 

Is this only on the bench?

I thought non sensored setups were supposed to do that? 

That's why you have to push off before you go so motors know what way to go.
```

---
## \#5 Posted by: Nedtrampz Posted at: 2019-06-13T04:27:32.763Z Reads: 42

```
Ive had someone else say that too but ive run sensorless trampa motors for nearly a year and thsy never spun the wrong way unless i changed a phase or invert on vesctool
```

---
## \#6 Posted by: Nedtrampz Posted at: 2019-06-13T04:28:39.859Z Reads: 40

```
When measuring flux linkage on tool it should spin. I just tried it again then and it didnt spin. But did finish successfully
```

---
## \#7 Posted by: Nedtrampz Posted at: 2019-06-13T04:33:00.410Z Reads: 41

```
Ok wtf i have just discovered something. 

The reading for resistance / inductance i got from using motor setup wizard was:  25.2 (R) & 13.6 (L)

But when i just use the detection tools i get: 1168 (R) & 25.87 (L)

I think the dodgy wizard has done something. 

The first time i ran it yesterday i got sensor readings but it was fucked when i tried to spin the motor
```

---
## \#8 Posted by: Nedtrampz Posted at: 2019-06-13T04:45:11.340Z Reads: 35

```
I feel that running the motor like this its possible the motor still tries to spin the other way whilst im riding it. That wouldnt be good i imagine..
```

---
## \#9 Posted by: Nedtrampz Posted at: 2019-06-13T05:22:00.587Z Reads: 28

```
Could this new resistance reading mean that there is a bad phase connection? It seems high considering the first time round it only measured at 25.
```

---

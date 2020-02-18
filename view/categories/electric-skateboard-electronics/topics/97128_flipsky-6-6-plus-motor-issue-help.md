# Flipsky 6.6 Plus Motor Issue Help

### Replies: 7 Views: 166

## \#1 Posted by: ccgpandora Posted at: 2019-06-22T23:45:45.445Z Reads: 81

```
One of my two motors does not spin with adequate power unless throttle is set to 100%. The other motor is able to change with adjustments of the throttle. The side with the issue is the "master" side of ESC while the slave seems to be functioning normally.

When the master is configured by itself without the slave, it is able to adjust the throttle properly. Once the slave is configured, it adjusts throttle properly, but the master is only 0 throttle or 100% throttle.

Any ideas? I included a video of the issue below.

https://imgur.com/a/EgjyCMC
```

---
## \#2 Posted by: wafflejock Posted at: 2019-06-22T23:50:03.594Z Reads: 77

```
Only run single drive but wondering if you have traction control enabled and its just causing the behavior on the bench.
```

---
## \#3 Posted by: ccgpandora Posted at: 2019-06-23T05:11:42.092Z Reads: 69

```
On VESCTool it says traction control is disabled for both. I have also tried resetting both.
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2019-06-23T06:03:27.951Z Reads: 66

```
enable traction control
```

---
## \#5 Posted by: JoelMatousek Posted at: 2019-06-23T13:26:59.603Z Reads: 48

```
Random question, but what remote do you have?
```

---
## \#6 Posted by: ccgpandora Posted at: 2019-06-23T16:59:57.247Z Reads: 38

```
Firefly Nano. It’s a DIY remote that a fork off of the original firefly remote.
```

---
## \#7 Posted by: banjaxxed Posted at: 2019-06-23T17:27:18.853Z Reads: 37

```
Switch phases from good motor to bad and eliminate problem with motor or phase connections
```

---

# Flux linkage detection failed

### Replies: 9 Views: 445

## \#1 Posted by: Allofyoush Posted at: 2019-06-27T21:41:35.550Z Reads: 84

```
Hey guys, I was setting up my VESC, and I connected everything and started running motor setup. But when I tried to run detection, I got a warning saying "flux linkage detection failed". what does this mean and how do I fix it? I looked in this thread
https://www.electric-skateboard.builders/t/motor-detection-fails-measure-flux-linkage-conclusion-phase-wire-shorrted/79003
but it didn't solve my issue.
```

---
## \#2 Posted by: tomiboi Posted at: 2019-06-29T04:54:52.285Z Reads: 67

```
I've had this problem... but I forget how I solved it. I believe it was with basic trouble shooting.
Start by restarting the tool and your device. Make sure that all connections are tight. Run detection again. If the problem is still there. Switch up two of the three motor wires and give it another shot. Make sure to start from scratch with the Wizard. Don't load the settings that are on your vesc. An old setting could be interfering with a new setting.
```

---
## \#3 Posted by: Allofyoush Posted at: 2019-07-01T23:19:42.536Z Reads: 51

```
I did all of that already. At first I thought it was a problem with the hall sensor, but t happened even when unplugged. And no matter how many times I swapped the 3 motor wires it still happened. I hope it's not a problem inside the motor or the VESC itself, because them's expensive.
```

---
## \#4 Posted by: tomiboi Posted at: 2019-07-02T01:17:01.015Z Reads: 48

```
I think the hall needs to plugged in for the linkage. If you test it without the hall make sure to set up the ESC as "sensorless". Have you ever damaged your motor wires?
```

---
## \#5 Posted by: tomiboi Posted at: 2019-07-02T01:19:03.782Z Reads: 48

```
Is this a new build. Have you checked to make sure your halls wires are wired correctly?
```

---
## \#6 Posted by: Allofyoush Posted at: 2019-07-02T01:35:56.147Z Reads: 43

```
I've set it up as sensorless but it does the same thing. It starts clicking, then spins slowly, but as it picks up speed it stops and just vibrates. Then it gives me the error prompt.

It is a new build. The hall sensor needs soldering, but it's not connected so it doesn't matter yet.
```

---
## \#7 Posted by: Fiori Posted at: 2019-07-02T01:45:27.543Z Reads: 41

```
![its-probably-the-flux-capacitor|379x364](upload://odb8BtzPc4fdPdSZVR4jgCkI4DQ.jpeg)
```

---
## \#8 Posted by: Allofyoush Posted at: 2019-07-02T02:32:55.966Z Reads: 39

```
well. I think I busted it by sending too much current through. Now it flashes pink. Not a good sign at all.
```

---
## \#9 Posted by: tomiboi Posted at: 2019-07-05T02:27:55.636Z Reads: 29

```
What ESC are you using? Could you post some screen shots of your settings and possibly the error message?
```

---

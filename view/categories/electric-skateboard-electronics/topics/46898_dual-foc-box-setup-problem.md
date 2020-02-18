# Dual foc box setup problem

### Replies: 21 Views: 1158

## \#1 Posted by: Brianr058 Posted at: 2018-02-20T00:59:47.879Z Reads: 164

```
I'm lost and hope the community can help.
I'm running a "Y" cable from the boxes to the receiver. Independently the motors run perfect, together one motor stumbles and stops unless it's full throttle. Both vesc's have been setup with the latest firmware and motor detection has been done. Any ideas?? Forgot to mention there's no fault codes
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-20T01:02:03.299Z Reads: 163

```
you set both up right? not just motor detection.
```

---
## \#3 Posted by: Namasaki Posted at: 2018-02-20T01:06:19.470Z Reads: 150

```
Also what controller are you using.
```

---
## \#4 Posted by: b264 Posted at: 2018-02-20T01:10:28.752Z Reads: 142

```
If you swap the motors, is it the same side that stumbles?  Or the same motor?  Or random?
```

---
## \#5 Posted by: Brianr058 Posted at: 2018-02-20T01:17:12.387Z Reads: 139

```
I'm using the gt2b 
And I should add that I had 5 days of perfect monster performance before the problem
```

---
## \#6 Posted by: Brianr058 Posted at: 2018-02-20T01:18:33.181Z Reads: 133

```
The same vesc. I thought it was the motor and replaced it to no avail!
```

---
## \#7 Posted by: Brianr058 Posted at: 2018-02-20T01:19:05.855Z Reads: 125

```
Definitely set up right
```

---
## \#8 Posted by: b264 Posted at: 2018-02-20T01:20:21.332Z Reads: 120

```
Is one of the +5V lines cut going to the receiver?  Are both ESCs connected to the same power source?
```

---
## \#9 Posted by: Brianr058 Posted at: 2018-02-20T01:51:53.053Z Reads: 120

```
After setup I disconnected the power from one
```

---
## \#10 Posted by: Deckoz Posted at: 2018-02-20T01:52:41.483Z Reads: 121

```
Power as in power from the XT60 or power on the 3 pin servo cable...
```

---
## \#11 Posted by: Brianr058 Posted at: 2018-02-20T02:05:47.117Z Reads: 118

```
The 3 pin servo cable
```

---
## \#12 Posted by: E1Allen Posted at: 2018-02-20T02:48:35.076Z Reads: 108

```
So if both work fine separate but when you connect the y cable it doesn't. I would check the y cable connections.  I soldered my y connection for the split.  Maybe a faulty connection somewhere within the pins or wire itself.
```

---
## \#13 Posted by: b264 Posted at: 2018-02-20T02:52:16.763Z Reads: 102

```
Swap which side of the Y connection goes to each ESC and see if it switches which one malfunctions
```

---
## \#14 Posted by: Brianr058 Posted at: 2018-02-20T03:02:33.892Z Reads: 103

```
Great suggestion guys. I will pick up a new cable tomorrow and report back.
```

---
## \#15 Posted by: Brianr058 Posted at: 2018-02-21T00:42:31.835Z Reads: 92

```
New "Y" connector, no change. I'm out of ideas other than to send them to someone to inspect them
```

---
## \#16 Posted by: stimm Posted at: 2018-02-21T01:58:05.591Z Reads: 88

```
Can you post a picture of your setup?
```

---
## \#17 Posted by: Brianr058 Posted at: 2018-02-21T02:19:33.190Z Reads: 85

```
![15191794752231870738985|374x500](upload://6q3TKsTiyNOnX9SULxm0Sy1v8Fr.jpg)![15191795160301511239930|374x500](upload://axc5iD2hu2biNtq3ioHcgGvnueW.jpg)
```

---
## \#18 Posted by: stimm Posted at: 2018-02-21T03:29:02.008Z Reads: 77

```
No Cam bus wire?
```

---
## \#19 Posted by: Brianr058 Posted at: 2018-02-21T03:32:24.062Z Reads: 76

```
not running canbus
```

---
## \#20 Posted by: Jammeslu Posted at: 2018-02-21T08:21:00.728Z Reads: 72

```
Have you opened it up to cheack for shorts etc?
```

---
## \#21 Posted by: Brianr058 Posted at: 2018-02-21T13:27:08.010Z Reads: 52

```
Nothing visual
```

---

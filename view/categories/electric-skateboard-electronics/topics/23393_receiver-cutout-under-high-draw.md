# Receiver cutout under high draw

### Replies: 17 Views: 634

## \#1 Posted by: Jinra Posted at: 2017-05-18T18:17:05.800Z Reads: 97

```
So I've encountered my first (or perhaps not) issue with my Benchwheel remote. The remote itself is perfectly fine, but the receiver's been acting up.

Context: I was riding home yesterday and along the 4 mile ride back, I face insane headwind and hills. This obviously causes high amp draw, and about a mile from home (almost the same place everyday) my board will cut out. I couldn't diagnose on the spot so I'd restart my board and everything would be dandy. However yesterday, I decided to kick it all the way home against high winds and hills so I could see if there were any faults in my VESC. **There were no faults**. Instead, I found that my receiver had a static light (meaning not connected to remote). Cycling the remote power didn't do anything, but unplugging and replugging the receiver fixed the issue.

I'm assuming high draw is what's causing my receiver to spazz out and refuse to connect until power cycled. Today I amped the motor max to 80A (from 60A) and now the receiver cuts out even on the way to work with a **tailwind**. It cut out under hard acceleration which backs my high draw == disconnected receiver theory. 

I'm just wondering if anyone has any insight on why this might be. My board is running dual 6355's with 2 VESCs with split PPM signal (only 1x 5v pin plugged in).

**TL;DR My board's Benchwheel receiver disconnects until power cycled while under high load/current**
```

---
## \#2 Posted by: fraannk Posted at: 2017-05-18T19:45:49.371Z Reads: 84

```
I have this issue with almost all my remotes when the receiver itself is too close to the VESC... The only ones that haven't done it yet is the Benchwheel (which i just got) and the Nano-X.
```

---
## \#3 Posted by: Jinra Posted at: 2017-05-18T19:53:49.245Z Reads: 81

```
is "too close" actually touching the VESC? I did have the PPM signal completely freak out when the antenna was touching the metal heat sink on my VESC. Right now the antenna is in between the two VESCS, not much room in there.

Also is your issue exactly the same where the receiver refuses to connect until power cycling?
```

---
## \#4 Posted by: fraannk Posted at: 2017-05-18T20:03:20.520Z Reads: 76

```
I had the problem when I velcro'd the reciever on top of the VESC. I didn't have to power cycle, I just got random brakes and accelerations. Really scary... I believe the power cycle part is the nature of the Benchwheel remote :)
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-18T20:11:07.577Z Reads: 73

```
The nature how though, not sure what triggers it. I understand the interference issue, which im pretty sure this isn't it.
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2017-05-19T03:50:09.232Z Reads: 66

```
Same issue need to get the receiver away from the esc ... weird stuff happens sometimes... doesn't seems to happen right away
```

---
## \#7 Posted by: Jinra Posted at: 2017-05-19T05:19:24.126Z Reads: 59

```
Is your issue intermittent signal, or complete drop until power cycle? Unfortunately my board is cramped for room and can only work with the receiver sandwiched between my VESCs
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2017-05-19T06:46:59.047Z Reads: 53

```
Intermittent 

I'm glad it doesn't happen all the time 

i made it worse by moving the actual antenna near the phase wires
```

---
## \#9 Posted by: Jinra Posted at: 2017-05-19T07:09:51.377Z Reads: 51

```
Haha yea, been there done that. When that hotdog shaped thing on my PCB antenna touched the aluminum heatsink from chaka's VESC, my PPM signal went full throttle non-stop regardless of whether the controller was on/off.

I suspect my problem has less to do with interference and more to do with high current draw doing shady things on my receiver. Notably, this never happened on my dual 5065 build.
```

---
## \#10 Posted by: Mark Posted at: 2017-05-19T07:12:48.512Z Reads: 52

```
It seems to be common and could also kill the receiver.
```

---
## \#11 Posted by: BigBoyToys Posted at: 2017-05-19T09:07:51.349Z Reads: 49

```
Could this be an interference issue? Add a ferrite ring?
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-05-19T09:25:35.099Z Reads: 48

```
That´s what helped me a bit with my ol´lill lady X-Car Beast and remote. Pushing lot´s of amps through it, while the receiver was close by caused some signal dropouts. Wired the PPM cable around a ferrite ring and problems were almost gone :slight_smile:
```

---
## \#13 Posted by: BigBoyToys Posted at: 2017-05-19T09:28:27.013Z Reads: 44

```
Yeah ferrite rings and routing the PPM wiires as far high current wires solved my cutout issue on two different boards. Definitely worth trying IMO
```

---
## \#14 Posted by: Jinra Posted at: 2017-05-19T13:32:18.784Z Reads: 39

```
As i mentioned i really doubt it's interference since it's 100%stable until i have extended high current draw in which it'll completely cut out until I restart the receiver
```

---
## \#15 Posted by: BigBoyToys Posted at: 2017-05-19T17:25:57.506Z Reads: 40

```
Well I can say my cutouts were definitely linked to current draw as well, but I didn't have to to reset my receiver so not sure what's causing that. Do you have a spare receiver/transmitter you can swap as a test?
```

---
## \#16 Posted by: Jinra Posted at: 2017-05-19T17:28:18.995Z Reads: 41

```
Yea, thankfully I do. Just worried it'll cutout on me again. I have had high current interference like you. It's a different issue than this though.
```

---
## \#17 Posted by: BigBoyToys Posted at: 2017-05-19T17:35:15.946Z Reads: 40

```
Yeah best of luck getting that sorted. I had mine cut out while I was testing my high speed tuck position 😐. ='d Faceplant.
```

---

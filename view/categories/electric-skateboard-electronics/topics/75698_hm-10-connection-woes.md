# HM-10 connection woes

### Replies: 13 Views: 333

## \#1 Posted by: Livid Posted at: 2018-11-23T12:26:54.832Z Reads: 110

```
I can't get data from my vesc on ackmaniacs app. Module seems wired properly. tried both master and slave, set to ppm & uart and uart respectively. baudrate set to 9600. I've selectec the device called "HMSoft" the blinking light on the module goes solid red, but it's all 0's in the app, and whenever i tap on anything it just says "ESC not connected". Does anyone know how to make it work?. phone is a galaxy s8+ on android 8.0.0
```

---
## \#2 Posted by: Andy87 Posted at: 2018-11-23T12:43:51.075Z Reads: 104

```
Which vesc you have?
Rx tx in the right order?
```

---
## \#3 Posted by: Livid Posted at: 2018-11-23T12:44:49.362Z Reads: 101

```
vesc 4.12 on 3.40 firmware. I've checked and double checked the wiring, rx and tx are reversed like they should be
```

---
## \#4 Posted by: Jmding Posted at: 2018-11-23T17:39:36.740Z Reads: 85

```
3.40 has issues, downgrade to 3.39 and it should work
```

---
## \#5 Posted by: thisguyhere Posted at: 2018-11-23T18:08:05.081Z Reads: 72

```
What phone u running?

Hm10 clones stopped working on Android oreo

-edit, if its showing up hm10 u should be good, the clones comes up bt05
```

---
## \#7 Posted by: Livid Posted at: 2018-11-23T18:49:27.639Z Reads: 67

```
hmm, changed to 3.39 and it still doesn't work. i'll keep fiddling
```

---
## \#8 Posted by: Livid Posted at: 2018-11-23T19:38:16.424Z Reads: 62

```
it's probably a knockoff module, i'll try when i get my hands on an old phone
```

---
## \#9 Posted by: Jmding Posted at: 2018-11-23T21:13:18.527Z Reads: 59

```
Did you swap TX and rx?
```

---
## \#10 Posted by: Livid Posted at: 2018-11-23T21:31:31.126Z Reads: 56

```
Yes i did, and just in case i tried with them the wrong way round too
```

---
## \#11 Posted by: Jmding Posted at: 2018-11-23T21:38:52.791Z Reads: 54

```
Welp. I'm out of ideas. Except maybe to try ackmaniac's firmware, but that's a bit of a reach
```

---
## \#12 Posted by: Livid Posted at: 2018-11-23T21:39:28.367Z Reads: 53

```
i'm 92.34% sure it's the clone module playing up, my phone refuses to pair to it
```

---
## \#13 Posted by: Jmding Posted at: 2018-11-24T06:43:48.761Z Reads: 45

```
My phone doesn't pair with it either, but the app works. It's because it is a Bluetooth low energy device (BLE). Not sure how it all works.
```

---
## \#14 Posted by: alexnz Posted at: 2018-11-27T03:11:36.436Z Reads: 34

```
I've had troubles along the upgrade path of Ackmaniac's app, and VESC firmware updates. 
Was working fine and then it stopped at some stage after an update. Bluetooth was connecting to the phone but not exchanging any data.
Got it back working again only by using the firmware 3.102 that comes with the Ackmaniac's vesc tool fork. 

That kind of sucks to have these incompatibilities, and to have to revert to this firmware version to restore functionality is bad!
```

---

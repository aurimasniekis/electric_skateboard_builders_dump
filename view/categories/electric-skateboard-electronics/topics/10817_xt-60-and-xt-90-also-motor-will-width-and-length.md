# XT-60 and XT-90 Also, Motor will, width, and length

### Replies: 9 Views: 1310

## \#1 Posted by: NewbieBoardBuilder Posted at: 2016-10-08T14:26:29.279Z Reads: 190

```
I'm pretty new to this field of research and electronics so I was looking at the "no words, just diagrams" posts and almost all of them had XT-60 and XT-90 pieces in them... Can anyone tell me what they do and when to use them. (Sorry I'm new) Also, cook somebody send me a link or explain what motor will, width, and length is.
```

---
## \#2 Posted by: mrjonnyjones Posted at: 2016-10-08T14:47:15.697Z Reads: 185

```
Hi, welcome to the forum.

XT-60 and XT-90 are connectors - they join wires to wires, wires to speed controllers, etc.  XT-90 connectors are larger than XT-60, so if you're using 10AWG (gauge) wire or lower (lower the number the thicker the wire/cable) I'd go with XT-90 (that's what I used on my board).  The metal connection barrels are bigger on the XT-90's, so can accommodate larger wiring.  Below is a video explaining this more...

https://www.youtube.com/watch?v=nVWn5u3WRsQ

Motor width is the diameter, so 50mm or 63mm usually.  Motor length is exactly that:  A 6355 motor will be 63mm in diameter, 55mm in overall length.  Furthermore, motor KV stands for how many rotations a motor will make for every 1 volt that passes through it.  Voltage x KV.  So, a 190kv motor will rotate 6,840 times if you're using a 10S (36v) system - on full throttle.

Hope this helps! :slight_smile:
```

---
## \#3 Posted by: NewbieBoardBuilder Posted at: 2016-10-08T16:50:18.209Z Reads: 155

```
THANKS SO MUCH, just when would you use a xt-90, what would they be used for to connect?
```

---
## \#4 Posted by: Hummie Posted at: 2016-10-08T17:02:50.929Z Reads: 151

```
 the xt90s is desirable because it has an integrated anti-spark resistor in it.  keeps it from sparking and carbonizing as well as protecting the esc I think

kv times voltage gives you the no-load max speed but put a load on it, you  or especially you on a hill, and it will sink lower.  maybe assume 80percent of the no load on a flat
```

---
## \#5 Posted by: mrjonnyjones Posted at: 2016-10-08T20:56:13.489Z Reads: 130

```
Usually these connectors are used to connect batteries, via wires, to the ESC and when making series or parallel harnesses.
```

---
## \#6 Posted by: NewbieBoardBuilder Posted at: 2016-10-08T21:15:31.416Z Reads: 124

```
Would you ever use one when doing a dual motor and dual vesc (with CANBUS) and an Enertion SPACE cell?
```

---
## \#7 Posted by: NewbieBoardBuilder Posted at: 2016-10-09T20:08:14.659Z Reads: 115

```
Would you ever use one when doing a dual motor and dual vesc (with CANBUS) and an Enertion SPACE cell?
```

---
## \#8 Posted by: Hummie Posted at: 2016-10-09T22:24:54.702Z Reads: 105

```
U have space cell so I don't know don't think so. They're to plug batteries to esc most often.
```

---
## \#9 Posted by: mrjonnyjones Posted at: 2016-10-24T07:21:25.182Z Reads: 89

```
I believe the Space Cell comes with one of these connectors (either XT60 or XT90) ready to plug into an Enertion VESC.
```

---

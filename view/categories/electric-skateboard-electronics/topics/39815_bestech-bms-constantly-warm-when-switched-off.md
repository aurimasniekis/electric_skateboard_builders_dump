# Bestech BMS constantly warm when switched off

### Replies: 8 Views: 1082

## \#1 Posted by: Funktapus Posted at: 2017-11-30T22:42:53.453Z Reads: 124

```
Hi Everyone,
I have a Bestech BMS (d223v1) and noticed that when wired for discharge/charge and switched off, a section of the BMS is constantly warm to touch. See pic below. Has anyone noticed this at all? I noticed it when I was assembling the board. Just before a test ride. Had not even gone for a ride. 

<img src="/uploads/db1493/original/3X/5/b/5bcaed53d1d8b3544a200d52318edb02db4ad488.png" width="429" height="314">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-01T02:04:28.281Z Reads: 112

```
Never noticed anything like that with them.
Can you give details about your wiring? Especially the balance wiring.
```

---
## \#3 Posted by: Funktapus Posted at: 2017-12-01T21:56:42.547Z Reads: 93

```
Here's my diagram. The numbers on the battery correspond with the balance numbers on the BMS.

<img src="/uploads/db1493/original/3X/4/5/452f73fafde1e75aab717ef4b74e96afe3ae2d7f.jpg" width="690" height="419">
```

---
## \#4 Posted by: darkkevind Posted at: 2017-12-01T22:02:40.467Z Reads: 90

```
Sounds like you may have one or more of your balance leads wired to the wrong cell group. Sounds like it's dealing with a short... :/
```

---
## \#5 Posted by: Funktapus Posted at: 2017-12-01T22:06:43.577Z Reads: 89

```
I can definitely confirm that the balance leads a correct. I say this because I did initially have one wired incorrectly and the corresponding pins on the BMS went real hot. Too hot to touch.
```

---
## \#6 Posted by: SilentException Posted at: 2017-12-01T22:07:46.946Z Reads: 91

```
Are you sure your parallel groups are in good shape? Might be a bad cell in one group and the BMS is constantly trying to passively balance the pack.
```

---
## \#7 Posted by: Funktapus Posted at: 2017-12-01T22:08:16.497Z Reads: 89

```
I think I've found a clue from another post. It could be that the BMS is still balancing the cells even when the charger isn't plugged in.

[quote="egzplicit, post:4, topic:39879, full:true"]
It's worth noting that (at least) a Bestech BMS will start balancing as soon as a group hits 4.2v and once a charger goes green, even if you unplug it right after that, the BMS will still balance the pack. I had a chat with the Bestech guys and they confirmed balancing happens even when the charger is unplugged.
[/quote]
```

---
## \#8 Posted by: Namasaki Posted at: 2017-12-02T01:59:00.987Z Reads: 81

```
That sounds logical since it has to dissipate the energy that it is trimming.
```

---

# Would a Wowgo V3 ESC be compatible with my Meepo V2?

### Replies: 13 Views: 235

## \#1 Posted by: dav3d75 Posted at: 2019-10-05T13:22:38.601Z Reads: 36

```
Hello,

I'd like to change my Meepo V2P ESC to a better one, and found someone selling a wowgo V3  ESC for cheap
Do you guys think it would be compatible with my setup? (battery, hubs, remote)

Cheers,
David
```

---
## \#2 Posted by: thebeardedboy Posted at: 2019-10-05T13:29:12.682Z Reads: 36

```
you would need to buy esc,remote and hubs from wowgo for it to be compatible
```

---
## \#3 Posted by: dav3d75 Posted at: 2019-10-05T13:35:15.836Z Reads: 35

```
Mmmh too bad, thanks
```

---
## \#4 Posted by: Ben.Nexus Posted at: 2019-10-05T13:40:56.246Z Reads: 35

```
That isn't true, you can use your existing hubs with the hobbywing hub esc, most come with a remote too. Ownboard sells a complete one for $80 and so does meepo iirc. But you may need to change the connectors on the motors, and perhaps even the hall order
```

---
## \#5 Posted by: xsynatic Posted at: 2019-10-05T14:14:26.942Z Reads: 32

```
Like ben said. It depends. If he sells only the ESC without remote you might need a new one, depending on what ESC your Meepo uses (they like to swap between hobbywing and LingYi, but its a v2p so i assume LingYi)

Hall sensors + phase wires might need adapters too. Wowgo uses a MR30/MR60 Connector.
Another thing to consider is if your Motors and battery are able to pull the Amps that the hobbywing esc needs. If i remember correctly its a 30A (15A per Motor) ESC. Older Motors are usually 12A per Motor.
```

---
## \#6 Posted by: dav3d75 Posted at: 2019-10-05T14:33:42.497Z Reads: 25

```
Thanks for the comprehensive answer.
My Meepo motors are the Koowheel 97mm motors 
No Idea if they are 15 or 12A though
```

---
## \#7 Posted by: Ben.Nexus Posted at: 2019-10-05T15:39:17.970Z Reads: 24

```
They actually take up to 35~40, you should be fine. Just be ready to do some soldering and make sure to buy extra connectors.
```

---
## \#8 Posted by: xsynatic Posted at: 2019-10-05T15:46:01.716Z Reads: 24

```
30-40 are you sure? That could also the reason why they get so hot if thats still the case.
```

---
## \#9 Posted by: Tinp123 Posted at: 2019-10-05T16:09:54.617Z Reads: 24

```
Motors will take as much current as esc will give to them. They *could* take 30-40 amps, but only on low speed with hard acceleration. It depends on esc setup and that is impossible to know. All those chinese hub motors will work with any chinese esc, only question is if connectors fit. And that is easy to fix.

There were people on this forum who were using chinese hubs with vesc - and they were pushing more than 30-40 amps and it was okay. With higher current, motors will heat more. Its not like they will stop working immediately if current is too big.
```

---
## \#10 Posted by: dav3d75 Posted at: 2019-10-05T16:16:33.762Z Reads: 22

```
Thank you so much guys!
```

---
## \#11 Posted by: dav3d75 Posted at: 2019-10-19T11:04:57.123Z Reads: 11

```
Sooo, I've contacted Ownboard to ask them if their ESC (hobbywing too) would work with my koowheel 350w hubs.
They answered "No you'll need to buy our motors with it" 
As some of you told me it would be ok, I'm quite baffled.
What d'you guys think? It's not a big investment ($72.00 with remote!) but still

Cheers,
D.
```

---
## \#12 Posted by: BillGordon Posted at: 2019-10-19T11:08:07.259Z Reads: 12

```
I call sales B.S. The kv should be in the same range so should work fine.
```

---
## \#13 Posted by: dav3d75 Posted at: 2019-10-19T11:17:20.949Z Reads: 12

```
That's what I suspect, but still...
Well I suppose I'l take the plunge
```

---

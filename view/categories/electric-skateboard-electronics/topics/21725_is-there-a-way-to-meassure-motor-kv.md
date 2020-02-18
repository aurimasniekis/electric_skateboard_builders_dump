# Is there a way to meassure motor KV?

### Replies: 4 Views: 456

## \#1 Posted by: Eboosted Posted at: 2017-04-25T02:59:46.737Z Reads: 78

```
According to the Electric Skateboard Calculator the final speed on my Vanguard build on @Torqueboards 190KV motors is spot on, extremely precise, but on my Reaper with 190KV motors from Polar my speed is off by 5km/hr.

I wonder if there is a way to meassure KV directly on the motors to see if Polar motors are in fact 170KV or 190KV as I thought from the begining.

**Loaded Vanguard**
<img src="/uploads/db1493/original/3X/0/1/01304ba8b348bb14d4830b99105f674d49d7ee25.png" width="383" height="500">
<img src="/uploads/db1493/original/3X/a/7/a7668eca75afffc979a06b4c2e31ad3740cc063f.png" width="281" height="500">

**Never Summer Reaper**
<img src="/uploads/db1493/original/3X/8/b/8b47f2ac2172163d13c0f0ab01b4c9e828577d9e.png" width="396" height="500">
<img src="/uploads/db1493/original/3X/c/e/ce6f76c33be681e0f5e7e698f1a696962d1217cb.png" width="281" height="500">

If I change the motor to 170KV the speed matches the skateboard calculator perfectly.
<img src="/uploads/db1493/original/3X/5/e/5e8e1b27165adb0ca80b224bc9f99ca03031acd2.png" width="377" height="500">
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-04-25T03:16:30.424Z Reads: 66

```
The motor constant (Kv) is measured without a load. There are expected losses in power.
```

---
## \#3 Posted by: Eboosted Posted at: 2017-04-25T03:26:35.990Z Reads: 64

```
Both speeds were meassured on the bench, so both e-boards are subjected to the same loses, however the Vanguard matched the speed and the Reaper not.
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-25T03:36:16.983Z Reads: 63

```
In the bldc tool, after you have ran the motor, go in the terminal and type "kv"

You will get the kv in erpm, divide that number by 7
```

---

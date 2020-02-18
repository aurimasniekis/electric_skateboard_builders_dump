# I need help with the set up

### Replies: 10 Views: 360

## \#1 Posted by: Bryantmorris101101 Posted at: 2017-06-13T03:17:46.593Z Reads: 68

```
Tacon 245kv motor with a vesc and 4×5500mah 4s.I dont know if i need to run 8s or a 12s would be better also I weigh 135 in poundsand live in a hilly area
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-13T13:49:45.009Z Reads: 44

```
You need to run 8s2p because that makes the best use of your batteries and 12s would go over the erpm limit of your Vesc. 245kv won't get you up very many hills though, of you wanted to do that it would've been better to buy a 10s battery + VESC + 190kv motor

Edit: 135 pounds is very light so you might be fine on 8s actually
```

---
## \#3 Posted by: Hummie Posted at: 2017-06-13T13:55:13.349Z Reads: 41

```
U have four of those lipo? U could do 12s and limit the max erpm on the Vesc. I'd do that for sure
That would be only using three of the batteries though.  Getting the fourth on would be doable in parallel but likely a bad idea and mixing capacities in series
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-06-13T13:59:20.277Z Reads: 34

```
8s on 245 kv will be good and will bring you up nearly every hill ;)
```

---
## \#5 Posted by: Hummie Posted at: 2017-06-13T14:04:56.655Z Reads: 30

```
im curious how you will do on 8s.  I'd try the 8s with all batteries and if hit the over temp shutdown do 12s
```

---
## \#6 Posted by: ninja Posted at: 2017-06-13T14:07:16.139Z Reads: 30

```
yeah, that is right! 

I have 8s4p with 245kv motor and I'm not light, I'm 90kg+ clothes and backpack. I have no problems with hills, single drive, motor never was hot, just warm. So yeah, 8s with 245kv is totally fine :wink:
```

---
## \#7 Posted by: Bryantmorris101101 Posted at: 2017-06-13T14:18:12.475Z Reads: 26

```
Thank you all so much
```

---
## \#8 Posted by: Hummie Posted at: 2017-06-13T14:41:50.289Z Reads: 25

```
it wouldn't be the motor that would get hotter but the esc
```

---
## \#9 Posted by: ninja Posted at: 2017-06-26T21:24:54.730Z Reads: 17

```
Yeah, you're right! :wink:
With @Ackmaniac App I can clearly see what is hapening in my e-board! My vesc is getting 60-70c from harder accelerations, and highest temp was 81c. Now vesc is in closed CF enclosure with heavy duty heat shrink and foam under it.
I'll upgrade vesc with ollin board heat sink and then will see what is going on. Hope it will solve the problem.
```

---
## \#10 Posted by: Alanhunt123 Posted at: 2017-06-26T21:55:01.001Z Reads: 14

```
I once had a single sk3 6364 245kv motor using a VESC and an 8S2P LiPo battery (4x 5200mAh 4S), and I struggled with heat issues on the VESC. It handled flats just fine, but once I hit a hill, it would just cut out on me.

So, I custom made a CNC aluminum case for it that directly sunk heat from the MOSFETs, and that completely solved the issue! I was able to tackle any hill!

However, this solution was a bit overkill, and you could probably get the same results by sticking some cheap heatsinks on the MOSFETs. The ones from Ollinboards will probably work fine.

Good luck!
```

---

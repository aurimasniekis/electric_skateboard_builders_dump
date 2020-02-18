# 10S4P vs 8S5P , &hellip;both 40 cells?

### Replies: 5 Views: 1175

## \#1 Posted by: Randyc1 Posted at: 2016-02-14T22:16:32.859Z Reads: 127

```
Building my first Single motor E board with a 6364-245kv & VESC. 
  I will achieve intended speed with around 8S , but according to Vedder theory on how to choose , 10S would be better ??

So either 10S4P or 8S5P ?
Your thoughts ?
```

---
## \#2 Posted by: onloop Posted at: 2016-02-14T22:43:50.790Z Reads: 130

```
higher voltage is better because you will have lower average amp draw and achieve the same power output. Depending on your desired top speed 245kv might be a bit high at 10S

either way, the Watt Hours is still the same, so range and charge times remain the same. 

so the benefits are
1. lower amp draw
2. less heat
3. slightly more efficient
```

---
## \#3 Posted by: cmatson Posted at: 2016-02-15T01:48:46.507Z Reads: 121

```
I'd go 8s5p. 245kv on 10s even with serious gearing will be VERY fast. 

I have a 6364 turnigy 245kv running on 6s: With 15/36 gearing I'm hitting around 25mph.

You could run something like 12/40 gearing on 10s, but you'd have a small amount of contact teeth on the motor pulley; less contact teeth means more belt slipping. Even running 12/36 can have a significantly worse effect on breaking than just 3 teeth more at 15/36. 

if you had a slightly lower KV motor, 10s would be the winner for sure- but with the higher speeds and gearing changes you'd have to do (unless hitting 45-50mph is all cool with you :wink:) I think the lower voltage will be better.
```

---
## \#4 Posted by: Randyc1 Posted at: 2016-02-15T15:51:20.478Z Reads: 106

```
I was thinking of making a diy Belt deflector(tensioner) to get more teeth in mesh with  a 12T motor gear ,....that would give me a 1: 3 gear ratio and 6 teeth in mesh ?
```

---
## \#5 Posted by: cmatson Posted at: 2016-02-15T15:52:44.826Z Reads: 104

```
ya, that'd work for sure! 

looking forward to seeing how it turns out
```

---

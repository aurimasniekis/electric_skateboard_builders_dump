# More amps or more volts

### Replies: 12 Views: 1190

## \#1 Posted by: crisonix01 Posted at: 2017-06-02T12:11:52.542Z Reads: 139

```
 need some help here. im building a e-mountainboard but still dont know wich esc to buy im thinking about the Hobbywing Max6 because of the amps for my understanding more amps more torque or a vesc would be better? the vesc is limited to 50 amps and when it comes to a mountainboard you need a lot of torque.
And I also have read that the vesc gets hot. Please help. Im going to be using sk3 6374 149kv by the way.
```

---
## \#2 Posted by: DeathCookies Posted at: 2017-06-02T12:18:16.848Z Reads: 138

```
I run my 149kv on 12S with a VESC. I never had a Temperature cutoff and it has plenty of torque. Great combo!
```

---
## \#3 Posted by: TarzanHBK Posted at: 2017-06-02T12:24:42.906Z Reads: 137

```
check out @Nowind 8s hobbywing max6 setup. Vesc is too weak for him. The max6 does have more punch.
It just depends on what you want :slight_smile:
```

---
## \#4 Posted by: crisonix01 Posted at: 2017-06-02T12:32:15.110Z Reads: 130

```
That is exactly what I want that torque to go up hills with no problem. I think im going with the max6 its just like 50 more dollars anyways and the amperage difference its a lot . thanks for the help
```

---
## \#5 Posted by: chaka Posted at: 2017-06-02T12:48:21.129Z Reads: 124

```
If you purchase a modified vesc with direct FETs you can add more thermal mass to increase the constant current rating.  Plenty of punch on our stock Ollin v1.1 esc (based on the vesc v4.12) I imagine enertions direct FET design has plenty of power also.
```

---
## \#6 Posted by: crisonix01 Posted at: 2017-06-02T12:52:08.564Z Reads: 119

```
im new to this so i dont know what FETS are can you help me with that?
and how much more current we talking about?
```

---
## \#7 Posted by: chaka Posted at: 2017-06-02T13:10:08.801Z Reads: 117

```
FETs, short for MOSFETs. 
You can see the difference in this photo. Direct FETs have a metal case and transfer heat much more efficiently.
<img src="/uploads/db1493/original/3X/c/3/c3fc4725b6b858b384c608b9067fccd8feb78f71.jpg" width="690" height="388">
```

---
## \#8 Posted by: crisonix01 Posted at: 2017-06-02T13:13:00.941Z Reads: 110

```
ok i see.but how much more current would that be able to handle?
```

---
## \#9 Posted by: chaka Posted at: 2017-06-02T13:15:25.359Z Reads: 109

```
With our stock heat sink we have doubled the constant current over the original VESC.
```

---
## \#10 Posted by: crisonix01 Posted at: 2017-06-02T13:16:49.850Z Reads: 108

```
so thats 100a at 44.4v right?
```

---
## \#11 Posted by: chaka Posted at: 2017-06-02T13:30:31.581Z Reads: 105

```
Yes and no. Real world use, you will never use a 100amps constant on a dual motor drive at 12s, that would equate to over 8000 watts of power.  Basically the vesc with direct FETs and heat sinks is no longer a weak link in a mtboard build.
```

---
## \#12 Posted by: nw-esk8 Posted at: 2017-08-24T03:06:31.022Z Reads: 53

```
How about 75-80a continuous :imp:?  Would that be doable w/ the new version?

I'm considering/planning a 12s 165kv-185kv 80mm eMTB 5:1 build (I'm ~140kg (plus a heavy board and a big ass battery and potentially a backpack :disappointed_relieved:)) and have some extended hills on my commute and it's not all paved....sooo, I think I'm a legitimate edge case :slight_smile:. 

Not sure what I'll pull, but I wouldn't be surprised if there are extended lengths where I could be pulling that much power... but either way, I am looking to have a well balanced system and want to err on the side of 'over built' and as bulletproof as possible.  I want to figure out what my controller options are and anything below 75a continuous would result in a bottleneck.

Thanks.
```

---

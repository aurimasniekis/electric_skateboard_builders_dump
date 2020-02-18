# Wiring setup for dual motor

### Replies: 9 Views: 1097

## \#1 Posted by: moe_lester Posted at: 2017-03-14T11:50:33.859Z Reads: 134

```
Hey guys do u mind telling me if my wiring diagram makes sense. I haven't put the bms balance Wiring on the diagram yet ill put it later. 

But does it make sense? 

<img src="/uploads/db1493/original/3X/d/2/d2082a3762c9ae070c0962d695a536822250b34c.jpg" width="374" height="500">
```

---
## \#2 Posted by: jga Posted at: 2017-03-14T12:21:13.203Z Reads: 121

```
Why is the loop key on one + cable only. Should not it be placed on the + cable before the split of the XT90 on the battery side?
```

---
## \#3 Posted by: moe_lester Posted at: 2017-03-14T12:40:51.473Z Reads: 110

```
Yh I'm not sure thats why I'm asking. 

Ive looked at some other people on here and they put the loop key after the battery xt90. 

And I thought that the loop key was only meant to be on the + cable anyway
```

---
## \#4 Posted by: Stefan Posted at: 2017-03-14T13:44:57.856Z Reads: 102

```
Should be placed before the split
```

---
## \#5 Posted by: Namasaki Posted at: 2017-03-14T15:06:35.642Z Reads: 102

```
Yes, before the split. Otherwise you are leaving one Vesc on continuously.
Place your key between the charge port and voltage meter. Then you will be able to charge with the key out and Vescs off. 
Also I see that you will be discharging through your BMS. Are you sure that your BMS can handle the amperage?
```

---
## \#6 Posted by: moe_lester Posted at: 2017-03-14T21:30:55.245Z Reads: 91

```
Ok thanks for advice, is it correct now? 

<img src="/uploads/db1493/original/3X/e/0/e06076c74b94c520dfb710ebdcbac07a3695793e.jpg" width="374" height="500">
```

---
## \#7 Posted by: cricrithezar Posted at: 2017-03-14T23:05:33.974Z Reads: 78

```
Your drawing is kind of a mess after the XT-90 but assuming you're just doing (+) -> (+) and (-) -> (-) then your diagram looks correct. Also make sure your BMS can handle the discharge current (otherwise you can bypass the BMS for discharge since the ESC has a low-voltage cutoff, you just won't get the short protection on your battery). 
Otherwise everything looks good to me.
```

---
## \#8 Posted by: Namasaki Posted at: 2017-03-15T01:23:24.707Z Reads: 66

```
The location of your loop key looks good now. 
What about your BMS ?
What BMS are going to use?
```

---
## \#9 Posted by: moe_lester Posted at: 2017-03-15T08:32:29.335Z Reads: 56

```
Im using this bms 

http://www.batterysupports.com/28v-29v-30v-60a-8x-36v-8s-lithium-ion-lipo-battery-bms-pcm-pcb-p-264.html
```

---

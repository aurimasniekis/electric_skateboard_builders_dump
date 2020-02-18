# VESC 6.0 with high kv (800kv) motor

### Replies: 7 Views: 569

## \#1 Posted by: arsh Posted at: 2018-03-26T03:11:56.094Z Reads: 113

```
Hello everyone, 

I ordered two VESC 6.0 from here last night. 

http://www.trampaboards.com/2x-vesc-6-in-cnc-t6-silicone-sealed-aluminum-box-with-genuine-xt90-connectors--vedder-electronic-speed-controller-trampa-special-p-24334.html

I have had a recent bad experience with MayTech 4.12 VESC (maybe it was partially my mistake too). 

Well, I would like to know that if the VESC I ordered, would they work for high kv motors in the range of 750 kv to 1100 kv? These are basically small copters motors and I would really like to use them for a project. Its not related to skateboards, RC or helicopters. I like the current sensing and other features of VESC thats why I am determined to use that. 

I noticed that in Vedder's video (link below), he said something about shunt in the start. Can anyone clear it to me if I would have to change the shunt if I want to use the 800 kV motor? 

https://www.youtube.com/watch?v=ugD6T4MPXUw

Thank you
```

---
## \#2 Posted by: MysticalDork Posted at: 2018-03-26T03:18:09.617Z Reads: 109

```
What battery voltage are you planning to use? That's an important factor.
```

---
## \#3 Posted by: arsh Posted at: 2018-03-26T03:22:38.443Z Reads: 107

```
I have a power supply with 5 A, variable voltage (upto 30V) output. 

http://ds-parts.co.kr/goods_detail.php?goodsIdx=11914

I also have a 6s LiPo but I would like to use supply.
```

---
## \#4 Posted by: MysticalDork Posted at: 2018-03-26T03:25:39.047Z Reads: 100

```
The vesc6 has been tested up to 150K erpm. With a 1000kv motor, that means you can use up to 15v without worries. I don't know what the absolute maximum possible ERPM is, or how to improve upon it.
```

---
## \#5 Posted by: arsh Posted at: 2018-03-26T03:30:07.077Z Reads: 96

```
Thank you MysticalDork

So I should not worry about changing shunt ? 

For my application, I will eventually apply load on the motor, are there any features that calculates torque also in VESC? I mean for simple DC motor ,  I would simply multiply current value with torque constant. Does it still hold for outrunner?
```

---
## \#6 Posted by: MysticalDork Posted at: 2018-03-26T03:32:10.965Z Reads: 88

```
I don't know enough to give useful advice about that, unfortunately.
```

---
## \#7 Posted by: arsh Posted at: 2018-03-26T03:37:23.241Z Reads: 81

```
Okay. 

Thanks
```

---

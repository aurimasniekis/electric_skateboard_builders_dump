# Higher cell count for more distance?

### Replies: 6 Views: 379

## \#1 Posted by: chewydinosaurs Posted at: 2017-05-30T05:18:22.003Z Reads: 71

```
Im currently running a 280kv motor on a 6s and dont get great range. Would increasing to an 8s increase my range at all or would it only increase my speed? I have fairly small batteries, 4000mah in series, with a wheel diameter of 83mm and a gear ration of 2.25:1. Thanks.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-05-30T05:30:08.120Z Reads: 72

```
Range is increased by increasing watt hours.
voltage x amp hours = watt hours
So yes, increasing voltage or capacity will increase range.
```

---
## \#3 Posted by: saul Posted at: 2017-05-30T05:31:09.374Z Reads: 71

```
if your esc can support the higher voltage, then yes. you'd get about 1/3 more range.

calculators are helpful.
[http://calc.esk8.today/](http://calc.esk8.today/)
```

---
## \#4 Posted by: Namasaki Posted at: 2017-05-30T05:35:01.768Z Reads: 66

```
@saul brought up a very important point.

So what ESC are you running?
If it's a vesc, you will need limit the erpm so that you don't fry the drv chip.
It sounds like your planing to replace your 2 3s lipos with 2 4s lipos.
If your just wanting more range and not speed, a better option would be to get 2 6s lipos and put them in parallel.
That would double you range and reduce voltage sag.
6s Lipos are very common and you can get good deals on them.
```

---
## \#5 Posted by: chewydinosaurs Posted at: 2017-05-30T06:02:05.909Z Reads: 51

```
Yeah it's a vesc, what would I want to limit the erpm down to?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-05-30T06:18:58.131Z Reads: 49

```
max erpm 60000
min erpm -60000
```

---

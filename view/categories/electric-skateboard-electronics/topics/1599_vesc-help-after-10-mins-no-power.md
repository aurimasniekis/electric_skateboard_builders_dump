# VESC HELP - After 10 mins no power

### Replies: 6 Views: 1090

## \#1 Posted by: NerijusM Posted at: 2016-02-29T16:17:14.408Z Reads: 86

```
Hello,

I build a mountainboard:
<img src="/uploads/db1493/original/2X/9/9de94dfd8ea058267939bd494d4955af6bebf61d.jpg" width="666" height="500">
Setup:
6374 192KV SK3 motor
VESC
6 or 12s Lipo setup
9" wheels
4.8:1 gear ratio

Tried 6s and 12s setups - no big diference in performance and distance. Tried FOC - works, but also lack of performance. I can forget about climbing 5-10% hills.

My VESC last setup screens:
<img src="/uploads/db1493/original/2X/5/5d8b259e81f34411aef336392c63dad158281c40.png" width="690" height="334">

<img src="/uploads/db1493/original/2X/6/697a39d9baaa78aee7363c40113367a6ebf8ff48.png" width="690" height="298">

<img src="/uploads/db1493/original/2X/e/e26d754767eb9c177e9ab5f3b2de90d0d62750fe.png" width="690" height="244">

I got basicly 8 km from half 12s 5000mah battery. 

Problems:
All power only for 5 minutes and then max speed about 10-15km/h. When I wait for 5 mins and I get power back for 3-5 mins and then 15km/h top speed. Totaly no hill climb power. My weight about 60kg (130 pounds).

Can somebody tell me where to dig for solving this problems? 
Maybe gear ratio? Or my VESC gots too hot? Current limit too low? Temperature limits too low?

Thank you!
```

---
## \#2 Posted by: treenutter Posted at: 2016-02-29T16:50:04.205Z Reads: 82

```
@NerijusM it sounds like one of the VESC's low-voltage thresholds is being surpassed. That would explain the temporarily reduced power. Are you sure your batteries are delivering the voltage consistent with your settings above? More info about your battery config would probably help the folks here on the forum that are likely to have a complete answer. Good luck!
```

---
## \#3 Posted by: NerijusM Posted at: 2016-02-29T16:52:07.481Z Reads: 82

```
Thanks.
Battery made from http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idproduct=35810 series or parallel, depends on 6 or 12s. Screens are for 12s setup i ride today.
```

---
## \#4 Posted by: NerijusM Posted at: 2016-03-01T12:13:40.905Z Reads: 63

```
Sorry for bump, but I realy need some advice.
Ordered 12T pulley, will try.
For now changed startup boost to 0.15 and current limit to 50A. Better, but no so.
```

---
## \#5 Posted by: RogerD Posted at: 2016-03-01T12:30:17.055Z Reads: 60

```
It's either low voltage cut off, or the FETs on teh board are overheating.
```

---
## \#6 Posted by: NerijusM Posted at: 2016-03-02T21:14:39.076Z Reads: 48

```
It was FET overheating.
Changed pulley to 12T, so now 1:6 gearing and board like new - flies!

Thank you.
Good luck.
Take care.
```

---

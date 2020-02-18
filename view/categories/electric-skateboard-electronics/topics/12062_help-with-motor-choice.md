# Help with motor choice

### Replies: 9 Views: 1073

## \#1 Posted by: AreaKruzer Posted at: 2016-10-28T07:56:58.191Z Reads: 118

```
Hi all,

I am building a new board for my friend but I am presented with just 2 options. He is going with a 8s setup, he weighs 235 to 240lbs.

His relative have gotten some motors wrongly for him. Below are the listed motors
1) 2 x 6354 motors with 270kV
1) 1 x 6374 motor 190kv

I am wondering which set of motors will be better for him. We stay in an area with pretty flat ground and inclines at 15% to 20% at maximum for a short stretch. But we will be using it more for flat ground,

Can someone with experience shed some light into this matter? If need be, he can even get his relative to get another 6374 motor 190kv but the mounting had to be a diagonal mount.
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-10-28T08:19:12.495Z Reads: 112

```
With a VESC, the 270kv on 8s is too high - better go with the 190kv and use the esk8 Calculator to get a gearing with your desired speed.

Depending on how much he weight a single 6374 will be enough
```

---
## \#3 Posted by: AreaKruzer Posted at: 2016-10-28T08:47:00.318Z Reads: 105

```
He weighs about 230 to 240lbs. (105 to 110kg)
```

---
## \#4 Posted by: Photorph Posted at: 2016-10-28T09:05:58.638Z Reads: 98

```
dual diag 6374 190 kv would be my pick because of his weight, 10s would be better also.
```

---
## \#5 Posted by: benwong Posted at: 2016-10-29T14:47:38.469Z Reads: 68

```
jus wondering y 270kv on 8s is too high. not really understand.. haha
appreciate can explain abit..
```

---
## \#6 Posted by: SteveS Posted at: 2016-10-29T15:23:32.834Z Reads: 62

```
270kv x 8s x 4.2v x 7 pole pairs = 63,594 erpm, which exceeds the recommended VESC limit of 60,000 erpm.
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-10-29T17:31:02.417Z Reads: 56

```
here you go:

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#8 Posted by: AreaKruzer Posted at: 2016-10-31T02:02:21.948Z Reads: 47

```
What if the 2 motors are actually 6354 200kv? will that be good for dual??
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-10-31T08:20:53.906Z Reads: 38

```
6354 is the standard size for dual
200kv at 8s-10s is recommended
```

---

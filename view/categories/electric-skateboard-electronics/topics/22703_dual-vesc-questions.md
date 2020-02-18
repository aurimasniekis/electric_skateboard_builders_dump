# Dual vesc questions

### Replies: 6 Views: 596

## \#1 Posted by: L3chef Posted at: 2017-05-09T06:09:40.276Z Reads: 76

```
So my current setup is Vesc 4.1 (50v cap) with a 6364 brushless motor.
I would like to upgrade to dual drive. And the second vesc is V.4.12 with 63v cap. Will there be an issue mixing different hw versions?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-09T06:15:29.511Z Reads: 75

```
If you want to be safe, you could run split servo instead of CAN bus communication.
```

---
## \#3 Posted by: L3chef Posted at: 2017-05-09T06:19:51.935Z Reads: 73

```
Thanks. This is all new to me so I have to check out what "split servo" means :)
```

---
## \#4 Posted by: Jinra Posted at: 2017-05-09T06:28:43.829Z Reads: 69

```
You basically want one of these (male to male split servo)

https://a.pololu-files.com/picture/0J3405.1200.jpg?686e82b3787b69952b99027ad77f2fc5

one end goes to your receiver, the other two ends go to each VESC. Make sure you remove the middle cable from one of the servo headers that go into the VESCs.

If you're using the benchwheel remote, the receiver supports 2 servo cables for which you don't need to remove the middle pin, makes it very easy to hook up, no split cable needed :)
```

---
## \#5 Posted by: L3chef Posted at: 2017-05-09T07:05:11.700Z Reads: 57

```
I see. I've got the alienpowersystem remote. So does it make a difference witch middle cable you cut? I meen the one that goes to master or slave vesc?
```

---
## \#6 Posted by: Jinra Posted at: 2017-05-09T07:07:08.585Z Reads: 57

```
Nope, it's the power pin, only 1 vesc needs to supply power
```

---

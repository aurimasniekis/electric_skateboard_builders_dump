# SOLVED* Motor Detection Failed

### Replies: 16 Views: 897

## \#1 Posted by: Challlsss Posted at: 2017-05-09T00:12:29.609Z Reads: 94

```
Hi guys I am configuring my brand new enertion VESC-X witha a turnigy SK3 6354 260 kv motor. I have a 6s setup and am trying to do motor detection. When I click start detection, my motor spins really fast then it stops really fast and then it spins slow. Then I get "Bad Detection Result Recieved" Here are my settings:

<img src="/uploads/db1493/original/3X/6/9/69703a244b748489839b94f556bb95dad1493fcc.png" width="690" height="355">

<img src="/uploads/db1493/original/3X/e/c/eca6398523de5b4ec08d4f13829467dc5ec534cc.png" width="690" height="354">

Any thoughts?
```

---
## \#2 Posted by: Jinra Posted at: 2017-05-09T00:13:22.097Z Reads: 81

```
lower your low voltage cutoff, that's definitely an issue
```

---
## \#3 Posted by: Challlsss Posted at: 2017-05-09T00:14:22.480Z Reads: 81

```
Just noticed that
Doesn't fix problem
I put it to 21 and 20.4
```

---
## \#5 Posted by: Jinra Posted at: 2017-05-09T00:18:43.843Z Reads: 78

```
Try a different phase wire combo, make sure they are not shorting as well
```

---
## \#6 Posted by: Challlsss Posted at: 2017-05-09T00:20:12.703Z Reads: 80

```
ok
That did not work either...
```

---
## \#7 Posted by: Blasto Posted at: 2017-05-09T00:34:03.298Z Reads: 76

```
Did you hit "write" when you did your changes?
```

---
## \#8 Posted by: psychotiller Posted at: 2017-05-09T02:53:14.137Z Reads: 71

```
Try doing motor detection with a lower voltage. Try 4s if possible.
```

---
## \#9 Posted by: Challlsss Posted at: 2017-05-09T13:06:49.069Z Reads: 60

```
Ok I will give that a whack
```

---
## \#10 Posted by: Philippe1 Posted at: 2017-05-09T13:09:08.405Z Reads: 61

```
Is your remote connected to the vesc?
```

---
## \#11 Posted by: Challlsss Posted at: 2017-05-09T13:09:42.438Z Reads: 60

```
No I did not have it plugged in
```

---
## \#12 Posted by: Challlsss Posted at: 2017-05-09T13:09:51.321Z Reads: 59

```
Just to the computer
```

---
## \#13 Posted by: Philippe1 Posted at: 2017-05-09T13:10:21.345Z Reads: 61

```
Could you take a picture of your setup pls?
```

---
## \#14 Posted by: Challlsss Posted at: 2017-05-09T13:20:48.135Z Reads: 62

```
I'm at work right now. I can continue to update this thread with photos... etc once I am off work.
```

---
## \#15 Posted by: Challlsss Posted at: 2017-05-09T13:21:37.156Z Reads: 61

```
I was also thinking about doing a full charge on my batteries before running the motor check.. would that help?
```

---
## \#16 Posted by: Challlsss Posted at: 2017-05-10T13:34:30.000Z Reads: 56

```
I fully charged batteries and then made sure to write configuration before doing motor detection. This fixed my problem
```

---
## \#17 Posted by: Challlsss Posted at: 2017-05-10T13:35:07.246Z Reads: 56

```
that is what I didn't do haha
```

---

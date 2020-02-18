# Constantly cutt-off when riding while using wining remote

### Replies: 12 Views: 1358

## \#1 Posted by: sandrewvdv Posted at: 2016-07-31T14:25:10.272Z Reads: 153

```
Even when riding slowly and acceleration slowly, the signal cuts off. It isnt braking, just losing throttle.
This happens for 1 second only. After this 1 sec period, (when I already released the trigger), The sginal comes back on and accelerates me the same amount of time I was pressing the button after the cutt off. I hope I make a little bit of sense ... The same goes while Im braking (sometimes). 
Is it:
- The amount off amps im drawing ( doesnt make sense, because I throttle very little and when Im going all the this doesnt occur more then when riding slowly)
-A temperature cutt-off? ( Also weird, sinse it happens even when just starting riding) + temps dont decrease in a 1 sec time period.
- A vesc related issue?
-An issue with the remote and receiver? ( no cables are coming loose + distince between remote and receiver is less than 1 meter) (+ tested range of remote and receiver is more than 5 meters)

Maybe anyone else that has had this problem? 

Thanks in advance
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-07-31T15:04:41.621Z Reads: 144

```
What is you remote ?
```

---
## \#3 Posted by: psychotiller Posted at: 2016-07-31T15:11:55.748Z Reads: 138

```
He said in his post it is a winning remote. 

It could be a couple of things, 
You could be pulling too many amps and if you are using the vesc it will shut you down for a second, then come back live. If so, you could adjust your voltage cut-off.

Could also maybe be a faulty receiver/transmitter. Borrow one from some else or hook up another if you've got it to rule TX/RX out.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-07-31T15:23:20.027Z Reads: 129

```
Sorry :sweat_smile: I think I might need a second coffee.
```

---
## \#5 Posted by: Jinra Posted at: 2016-07-31T15:30:45.645Z Reads: 128

```
is your receiver close to your phase wires or other electronics? try moving it away from them and trying it out.
```

---
## \#6 Posted by: sandrewvdv Posted at: 2016-07-31T16:26:37.180Z Reads: 118

```
Another thing I experience. It isnt 'just' a cutt-off. It almost feels like 'lag'. Because when I break, the breaking sometimes happens 1sec later, but he Time of breaking corresponds with the Time I held the break down. 

interference of the phase wires should really not be a problem, they are on the oppiste side of My box.

I unfortunately have no one close by to test with an other controller

also, of it was an voltage cut off setting in the vec, it should
.  cut of immedeatly
.  Happen al the Time and not once in a while


i must add that My box is made of a material of aluminium and a sturdy plastic. Maybe a farraday cage, but that doesnt really explain the 'lag' ?

(aome typo's may be present, on phone and autocorrect in Dutch)
```

---
## \#7 Posted by: Jinra Posted at: 2016-07-31T16:41:41.363Z Reads: 110

```
try insulating the receiver from your aluminum enclosure or other metals by having it sit in rubber (heatshrink). When my receiver touched my aluminum heatsink of my VESC, it freaked out and wouldn't accept my input and sent my motors to full blast.
```

---
## \#8 Posted by: sandrewvdv Posted at: 2016-07-31T16:57:44.636Z Reads: 104

```
It's an aluminium case fully enwrapped in a plastic enclosure (we Call it 'dibond') so there is no 'naked' aluminium. Therefore no need to insulate My wires ( although I taped each wire seperately.).
```

---
## \#9 Posted by: sandrewvdv Posted at: 2016-07-31T22:09:58.611Z Reads: 91

```
Thank You very much for your responses, the problem to My solution seemed to be:  Remove the receiver out of the box.

so an aluminium case isnt the best solution ( altough being very sturdy ;) )
```

---
## \#10 Posted by: stuxtruth Posted at: 2016-07-31T22:43:09.523Z Reads: 88

```
I'm having the same issue with my winning remote.
```

---
## \#11 Posted by: stuxtruth Posted at: 2016-07-31T22:44:46.816Z Reads: 88

```
http://www.electric-skateboard.builders/t/motor-braking-at-high-speed/6824

Keep in mind it was a different issue with the video I posted. I may see if I can get a vid of my board doing it.
```

---
## \#12 Posted by: sandrewvdv Posted at: 2016-07-31T22:58:48.224Z Reads: 82

```
Im almost certain the issue is solved. I think the box was the problem. Ill keep this post updateted if this wasnt the problem. The responses on This thread were very helpful, it made Me look at the problem differently. 
thank You very much
```

---

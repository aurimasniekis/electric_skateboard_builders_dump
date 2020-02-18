# How to connect a Yuneec E-GO Cruiser to my source VESC on my DIY Electric Longboard

### Replies: 26 Views: 275

## \#1 Posted by: TdeBeer Posted at: 2019-02-10T08:37:06.798Z Reads: 33

```
Hello there guys,

I am having trouble as the remote to my electric longboard has gone missing and the only other controller I have is the Yuneec E-GO Cruiser controller. Is there a way to connect this to my DIY board with a source VESC??

Any help would be appreciated, 
Thanks.
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-02-10T08:53:37.337Z Reads: 29

```
Does the yuneec remote have a separate receiver, or is it built into the yuneec board? If there's a separate receiver, then you should be able to connect its output to the vesc. If it's integrated, you're SOL and you have to get another remote.
```

---
## \#3 Posted by: TdeBeer Posted at: 2019-02-10T08:55:19.975Z Reads: 25

```
What do you mean?

I have a reciever connected to My own VESC inside my board.
```

---
## \#4 Posted by: TdeBeer Posted at: 2019-02-10T08:56:32.150Z Reads: 25

```
Would it be easier if I sent a picture of my setup and the remote?
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-02-10T08:56:53.022Z Reads: 25

```
Pictures help, yes.
```

---
## \#6 Posted by: TdeBeer Posted at: 2019-02-10T08:57:05.356Z Reads: 24

```
Ok, one second
```

---
## \#7 Posted by: TdeBeer Posted at: 2019-02-10T09:00:13.347Z Reads: 24

```
![IMG_0555|375x500](upload://1G8WtCKRHBUUzlSHFO9RV4HR3ba.jpeg) ![IMG_0554|375x500](upload://dXtfqnIQHK5i4oBaazXCnuQV7ms.jpeg) ![IMG_0553|375x500](upload://fUIYx2uILzziDBXJg6jlS2Rkzf0.jpeg) ![IMG_0555|375x500](upload://1G8WtCKRHBUUzlSHFO9RV4HR3ba.jpeg) ![IMG_0554|375x500](upload://dXtfqnIQHK5i4oBaazXCnuQV7ms.jpeg) ![IMG_0553|375x500](upload://fUIYx2uILzziDBXJg6jlS2Rkzf0.jpeg)
```

---
## \#8 Posted by: MysticalDork Posted at: 2019-02-10T09:01:21.983Z Reads: 23

```
So, that little module hanging off the vesc is the yuneec e-go receiver?
```

---
## \#9 Posted by: TdeBeer Posted at: 2019-02-10T09:02:00.499Z Reads: 22

```
No, that is from the controller the controller that has been lost.
```

---
## \#10 Posted by: MysticalDork Posted at: 2019-02-10T09:02:13.676Z Reads: 22

```
And what kind of controller was that?
```

---
## \#11 Posted by: TdeBeer Posted at: 2019-02-10T09:02:31.424Z Reads: 23

```
it was a Maytech controller from Electric Board Solutions
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-02-10T09:03:56.793Z Reads: 23

```
There's your problem. I don't think the yuneec controller will talk to a maytech receiver.
```

---
## \#13 Posted by: b264 Posted at: 2019-02-10T09:04:36.548Z Reads: 22

```
Send a photo of the E-GO internals if possible
```

---
## \#14 Posted by: TdeBeer Posted at: 2019-02-10T09:04:39.279Z Reads: 23

```
ok. So I could fix this by getting a 2.4GHz remote with a reciever?
```

---
## \#15 Posted by: b264 Posted at: 2019-02-10T09:05:04.545Z Reads: 23

```
Yes, a Mini Remote as we call them is the best option
```

---
## \#16 Posted by: TdeBeer Posted at: 2019-02-10T09:05:12.335Z Reads: 23

```
and if so, does it have to be a electric longboard controller specific or can it be any 2.4GHz controller with a reciever?
```

---
## \#17 Posted by: MysticalDork Posted at: 2019-02-10T09:06:35.189Z Reads: 24

```
As long as you have a remote and a receiver that talk to each other, and the receiver has a signal that the vesc can interpret, the possibilities are endless. RC car remotes, wii nunchucks, the list goes on.

2.4GHz is preferred because it's a robust communication protocol, but others have been used.

Like Brian said, a Mini remote is a great choice.
```

---
## \#18 Posted by: TdeBeer Posted at: 2019-02-10T09:07:19.990Z Reads: 24

```
Ok, awesome. Thanks for the help
```

---
## \#19 Posted by: b264 Posted at: 2019-02-10T09:08:14.359Z Reads: 22

```
https://buildkitboards.com/products/mini-remote
```

---
## \#20 Posted by: TdeBeer Posted at: 2019-02-10T09:08:30.838Z Reads: 22

```
So I could basically buy a cheap remote car, steal the remote and the reciever and connect it to my board?
```

---
## \#21 Posted by: MysticalDork Posted at: 2019-02-10T09:09:11.092Z Reads: 20

```
Yes, but.

Most "cheap" RC cars don't have a receiver you can remove, it's built right into the control board.
```

---
## \#22 Posted by: TdeBeer Posted at: 2019-02-10T09:09:42.444Z Reads: 19

```
Oh, I'm currently in South Africa and trying to find one near me
```

---
## \#23 Posted by: b264 Posted at: 2019-02-10T09:10:03.869Z Reads: 20

```
Yes but reliability is a big deal.  You don't want it to fail or cut-out on you while you're going fast.  I would highly recommend that one I linked if you're in the USA and don't know which one to get.  Make sure you put a lanyard on it, because dropping the remote is an extremely hazardous thing to happen.
```

---
## \#24 Posted by: MysticalDork Posted at: 2019-02-10T09:10:39.136Z Reads: 20

```
If there's a hobby shop near you, you can get a RC car remote and a compatible receiver. As long as they both use the same protocol (spektrum, etc) you're good.
```

---
## \#25 Posted by: TdeBeer Posted at: 2019-02-10T09:10:40.514Z Reads: 21

```
Ok, I'll see what I can find
```

---
## \#27 Posted by: b264 Posted at: 2019-02-10T09:12:30.696Z Reads: 21

```
https://www.ebay.com/itm/2-4Gb-radio-remote-controller-for-electric-longboard-skateboard/323106671799

Plus 2 x AA batteries and [a lanyard](https://www.ebay.com/itm/Strap-Hand-Wrist-Lanyard-for-Cellphone-Wii-Camera-Phone-Mp4-Mp3/362545667135)
```

---

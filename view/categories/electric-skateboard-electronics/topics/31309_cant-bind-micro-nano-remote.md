# Can&rsquo;t bind Micro (Nano?) remote

### Replies: 5 Views: 593

## \#1 Posted by: karosass1 Posted at: 2017-08-23T12:50:39.939Z Reads: 77

```
I have this 'Micro' remote http://www.hellray.de/shop/#!/eSk8-de-Micro-Remote-2-4GHz/p/68315132/category=15842017
But i think it's nano?
I try to bind it by plugging in bind cable in bind channel, then power from vesc, receiver starts flashing.
Hold bind button on controller and power it on, receiver led turns off, controller start blinking fast. 
After few seconds there is bright led on both of them and it says to disconnect binding cable from receiver, that's what I do, but then LED turns off on receiver (Still solid red on the controller) and pressing throttle doesnt do anything. turning controller off and on again doesnt do anything.

The Vesc (focbox) is at the moment connected to pc bldc tool if that changes anything
```

---
## \#2 Posted by: karosass1 Posted at: 2017-08-23T13:02:50.051Z Reads: 72

```
I think, I fixed it, the problem now is that motor automatically spins, unless I put remote on full brake

http://i.imgur.com/OdwPkc3.png
http://i.imgur.com/NrAppnJ.png
http://i.imgur.com/doCozuH.png
http://i.imgur.com/SHDbG2B.png
```

---
## \#3 Posted by: JLabs Posted at: 2017-08-23T13:35:21.647Z Reads: 57

```
You have to set the min and max pulse width values in the PPM tab. 

 You can do this by checking the display box and then giving full throttle and in putting that value in the max box. Then give full break and input that value in the min box.
```

---
## \#4 Posted by: karosass1 Posted at: 2017-08-23T14:05:11.650Z Reads: 51

```
Yeah, I posted this too soon, without doing enough research :smiley:
```

---
## \#5 Posted by: trancejunkiexxl Posted at: 2017-08-23T14:53:44.472Z Reads: 46

```
i freaked out and did the same thing, then bothered jinra a bunch haha. it happens XD
```

---

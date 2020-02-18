# Motors Spin up when transmitter is disconnected

### Replies: 8 Views: 246

## \#1 Posted by: Kuchi Posted at: 2018-07-05T01:45:01.447Z Reads: 75

```
So I have almost everything figured out now with my build except if I turn off my remote while the motors are powered it ramps up to full throttle. How do I fix this and make it just go into free spin mode and if it disconnected for more than 10 seconds it slowly applies full brake.
```

---
## \#2 Posted by: lrdesigns Posted at: 2018-07-05T05:15:51.964Z Reads: 58

```
More information? Which remote are you using?

Most likely you need to set the "failsafe" so the board goes to neutral with the remote off.
```

---
## \#3 Posted by: Kuchi Posted at: 2018-07-05T05:30:32.024Z Reads: 57

```
I am technically using a gt2b but have it in a thumb style case, I don't know much more info I can give you, where can I find this "failsafe", I have been reading and watching diyelectric tutorials to help me learn VESC tool.
```

---
## \#4 Posted by: lrdesigns Posted at: 2018-07-05T05:36:23.242Z Reads: 56

```
Just google gt2b fail safe setup. 

But from memory the steps are, 
1. turn on remote (leave throttle in neutral position)
2. Turn on board, while holding the the button on the receiver for few seconds. 
3. turn everything off and on again. Always turn on remote first.

This should set the fail safe on the receiver to go to neutral when the remote is disconnected. 

One issue with thumb remotes / gt2b is if your natural position in vesc tool is not 1500 then turning your board on first before the remote will result in the board going to throttle on after a minute if the remote remains off. So always turn on the remote first as this will set the fail safe on the receiver.
```

---
## \#5 Posted by: Kuchi Posted at: 2018-07-05T05:53:21.001Z Reads: 44

```
Ok I will try that tomorrow
```

---
## \#6 Posted by: lrdesigns Posted at: 2018-07-05T06:15:08.650Z Reads: 44

```
[GT2B Instructions.](https://hobbyking.com/media/file/737141785X1139128X5.pdf) 

In chinglish 
![image|683x500](upload://zbzKmFBxbNq2AkFjf6vZrxnFTQc.jpg)
```

---
## \#7 Posted by: Kuchi Posted at: 2018-07-05T22:58:30.479Z Reads: 27

```
Wow thank you that was stupidly easy, I thought it was through the VESC tool.
```

---
## \#8 Posted by: lrdesigns Posted at: 2018-07-05T23:02:30.845Z Reads: 25

```
Vesc can have its own fail safe settings too but it’s not needed if set on receiver.
```

---

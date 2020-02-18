# Should the voltage drop after going trough the bms?

### Replies: 4 Views: 834

## \#1 Posted by: DennisBlad Posted at: 2017-07-18T14:55:43.919Z Reads: 66

```
Hey! 
My first post in this amazing forum. I have been lurking for month and am now in the middle of building my first E-skate!
I am almost done with my battery(10s4p LGHG2) and found one, to me, strange thing. When i measure the voltage from plus to minus over the whole battery it says 35.4 volts, but once going trough the bms it says 31.4. Is this normal?

I wouldn't dare to connect the balance wires before checking with the pros here on the forum. But on the other hand maybe its because of not connecting the balance wires i am getting this problem? 
Anyways thanks in advance!
<img src="/uploads/db1493/original/3X/d/8/d845077ced0762fd2e593971b1f72e50a7f12916.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/2/4/24e19f9f2ae5aed49eacad059726c203eab33fc4.JPG" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2017-07-18T15:08:48.650Z Reads: 60

```
Yea.. it should read the same from both ends, but as you said, it may because the balance leads aren't plugged in. Theres a wide variance on how a BMS will behave, and unfortunately, no standard for it all. 

As long as you make absolutely sure the balance leads are in the right place and at the right voltage, just go ahead and plug it in and find out. Worst case scenario your BMS fries or a balance lead fries, but your pack should be safe.

Also, I'm not sure how an XT-90S works, but there is a built in resistor which may be affecting the readout of the voltage. Try measuring from the battery positive directly and the battery negative after the bms, but before the xt90s
```

---
## \#3 Posted by: DennisBlad Posted at: 2017-07-18T15:36:36.269Z Reads: 57

```
I plugged the balance wires into the bms and hoped for the best.. But no smoke so far! 
Now the XT90 shows 35.4 also, so i guess it had something to do with the wires not being connected.
Thanks for the help Jinra!
```

---
## \#4 Posted by: Martinsp Posted at: 2017-07-18T17:19:37.013Z Reads: 44

```
Yes that is caused by the balance not connected. The BMS is pretty simple because all it does is monitor the voltages of the cells and discharges the cells that are not balanced through the big resistors you can see under the heatshrink.

So if it does not see any voltage on one or more cells it disconnects the load with the big transistors. If you put in on your board like this and tried to ride it would go for a second, limit the current to the load, work for a second and so on...
```

---

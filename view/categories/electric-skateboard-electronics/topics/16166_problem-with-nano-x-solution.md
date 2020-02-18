# Problem with Nano-x \[Solution\]

### Replies: 17 Views: 1914

## \#1 Posted by: captainskippy Posted at: 2017-01-16T02:22:43.152Z Reads: 196

```
Finally got my nano-x controller and mounted it up.  It would not connect to the handheld unit, just sat and blinked.  Then I jiggled the wires and it connected.  Figured it was a bad wire harness so I made a new one.  Same issue.  I just had to pull on the harness at the receiver and it would connect.  Took the receiver apart (it has two little screws) and pulled out the board.  There was white two sided tape right under the harness connectors.  Not really sure, but I am guessing the two sided tape was conductive enough to be messing with my voltages.  I peeled the tape from the housing and moved it over away from where the harness leads come out of the back of the board and problem solved!  I have verified this on two Nano-X receivers so I am pretty sure this was the issue.  System connects perfectly every time now.  Hope this helps this great online community.
```

---
## \#2 Posted by: Blasto Posted at: 2017-01-16T02:52:02.939Z Reads: 193

```
Great find!

Was wondering why some users had problems and others don't.

Will do some test to verify if this is the root cause
```

---
## \#3 Posted by: captainskippy Posted at: 2017-01-16T02:52:38.208Z Reads: 186

```
glad to help
```

---
## \#4 Posted by: Blasto Posted at: 2017-01-16T03:00:08.394Z Reads: 184

```
updated my video with your thread as reference!

https://www.youtube.com/watch?v=nUrmKLpR70E
```

---
## \#5 Posted by: onloop Posted at: 2017-01-16T04:07:59.118Z Reads: 175

```
Interesting find. 

We will share this info with others if they report binding issues.
```

---
## \#7 Posted by: onloop Posted at: 2017-01-16T06:48:44.073Z Reads: 156

```
My personal test units work fine. Also there were no complaints of issues reported by independent users during the beta test program. Manufacturer also does a test bind check before shipping. 

Seems as though most issues are isolated to a small number of units. At least 250 units shipped and 95% have had no issues/ reported issues also vary. 

it seems only a small percentage reporting similar problem and we will investigate this further and do more specific checks.

We will also remove the autobind as it seems to be a point of confusion with some users due to booting inconsistencies.

A manual button press and bind key process may be a simple solution.  

My advice for now is follow the process in the instructions. If your unit is faulty let us know and we help you troubleshoot and if necessary replace it for free.

Apart from the very few binding issues we are getting lots of positive feedback about this product.
```

---
## \#8 Posted by: Schulerbible Posted at: 2017-01-16T09:08:56.141Z Reads: 141

```
Did you measure the resistance? I get a reading through my body but none through the tape ... not so sure if this is the origin of this issue??? I got the issue but the cause was a partially loose signal cable. The receiver was powered up but the auto binding did not work. And I did not have any issues when connecting the harness to the GT2B receiver ... 

> I just had to pull on the harness at the receiver and it would connect

Same issue. I removed the board from the enclosure (and tape) and still did not work.
```

---
## \#9 Posted by: Lsalt Posted at: 2017-01-30T01:21:53.085Z Reads: 119

```
I have an esc with bec. When I have the bec power connected only, it will bind. But if I have both the esc connected in ch1 and bec power connected it will not bind. I have to connect the bec to bind and then connect the esc to ch1. So basically this has to be done every time I power up the board. I would like a new one please cuz this one obviously has issues.
```

---
## \#10 Posted by: Deakbannok Posted at: 2017-02-07T08:32:07.145Z Reads: 115

```
I just received a Nano -X last week. I preordered them on sum since the November 2016 with everything, Battery, VescX, motor and wheels.

The remote and receiver came with instruction. BUT NO harness wire with them.
Follow the instructions on manual.

- Tried with binding cable
- Switching CH slot
- removed the 2 side tape in the RX.

I get TX and Rx to bind with these methods a few times.
But once I power them off. They will not stay binding.

What do you guys think?
```

---
## \#11 Posted by: Deakbannok Posted at: 2017-02-08T11:58:06.457Z Reads: 103

```
The only way to you get your Nano-X remote (TX) to bind with receiver (RX).
You must disconnect the signal line between your RX and VESC-X.
Then your TX and RX will bind together right away.

I am not sure it is the RX or VESC-X is doing that.
Is any options on BLD tool to check that?
```

---
## \#12 Posted by: Schulerbible Posted at: 2017-02-08T12:33:54.868Z Reads: 101

```
The signal line must be rock solid. I have experienced this in my setup where the signal cable was partially loose but still connected to the RX. The GT2E had no problem at all.
```

---
## \#13 Posted by: Lsalt Posted at: 2017-02-09T03:20:22.840Z Reads: 96

```
No your signal line being rock solid has nothing to do with it. Its not your vesc. I have torqueboards 12s esc and power the reciever with bec. Will bind only if signal wire for esc is not connected. Then you can plug it in after bind but then must repeat after power down. Sending my reciever back to enertion. They have figured out the issue and will repair it and pay shipping. They said they would ship out a new rx but don't have any. Repair is the only option.
```

---
## \#14 Posted by: Deakbannok Posted at: 2017-02-09T08:21:09.730Z Reads: 92

```
So out of nowhere. I got the TX and RX to work now
I was using the same wire connection and play around with the connection between RX and VESC.

The RX started to bind randomly when I moved the wire and connection around. Then I would retry to rebind them again.

 Some it couldn't bind, but sometime it could for a few time.

Also I did was, disconnect and reconnect the signal wire repeatedly between RX and VESC until I can get TX to bind with RX.

Use it for a few seconds and then turn off power and repeat to rebind them again. *For  nearly hour*

I am still curious about it. And how....
```

---
## \#15 Posted by: Deakbannok Posted at: 2017-02-09T08:42:34.147Z Reads: 87

```
@Lsalt Did they inform you what is wrong with it?
Is it the connection or component problem or the chip itself in RX?

My Nano-X controller came in the mail last month with a broken plastic power switch.
But I didn't get home from mission until last Friday.
So I sent email and photo to Enertion customer support. They have informed to mail me a new controller once the product is in the warehouse.

The controller is working fine. Need to use a small plastic pin to turn the switch every time. Little difficult but I am happy with Enertion products.

I am new to Electric skateboard here. But I have been longboard for years. Grewup in Bellingham and MT Baker hwy is the path.
```

---
## \#16 Posted by: Schulerbible Posted at: 2017-02-09T11:29:55.653Z Reads: 84

```
Yes it does! Of course you don't need a signal line for binding but if this one is attached it could lead to bjnding issues which was exactly the case in my setup!
```

---
## \#17 Posted by: Lsalt Posted at: 2017-02-09T17:38:56.063Z Reads: 82

```
Of course it's important to have a strong signal line, but even if you do have one, the reciever has a binding issue. So therefore it must be repaired by them. They asked for the reciever, not my signal wire lol. They know what's wrong with it but didn't say exactly what. They did say some users were having this binding issue. I have used the mini and other nano from torqueboards with zero binding issues with the same setup. Granted they have other reasons why I don't like them but no issues binding. If you remove the signal wire 
on the nano x receiver, it's the disconnect that let's it bind in my case. So I dont see what having a poor connection has to do with it not binding since it will bind with zero connection. Granted there may be more than one issue with the receiver but this is the logic in my case in particular. :smile:
```

---
## \#18 Posted by: Deakbannok Posted at: 2017-02-09T18:49:43.139Z Reads: 76

```
That's weird. I wish they can give us some explanation here.

Now I have my Nano-X controller and receiver working normal.
Everything is connected. Power on and push.

But I will try to disconnect and test them again. To see if it will stay bind.

Off topic
Is anyone here know what type of power switch on its controller and where can I buy them. I need to replace this broken plastic switch.
<img src="/uploads/db1493/original/3X/0/f/0f4a72937afeb13ae55228aa748ea31e210b04a7.jpg" width="690" height="388">
```

---

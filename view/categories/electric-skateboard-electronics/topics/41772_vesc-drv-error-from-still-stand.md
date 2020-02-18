# VESC DRV error from still stand

### Replies: 13 Views: 1731

## \#1 Posted by: lansselot Posted at: 2017-12-23T16:48:34.604Z Reads: 178

```
Hello people, great forum you have hear. 
I have been busy for the past few months building my first esk8 board. After a lot of designing, planing , googling, 3d printing and customising parts to let it fit I could make my first rite. And it was great. 

This has been about a month ago, I made a few improvements, changes and have made a few kilometres. But I run Into a little hickup with my VESC. I'm struggling with a start-up problem. When I power the board and I use my remote to accelerate it won't start turning from a standstill and blinks 3 times red. When I gif it a hard spin bij hand and then apply thrust it starts turning on his own. And after it spint for a while it will start from a standstill. 
Also, when I apply to mutch break power it stops breaking blinks 3 times and breaks again and starts over with this cycle. 

When the board has been in a cold car it is even worse. Than I have to gif it quite a few spins before it will start turning on his own.
This is in use and also on the work bench. 
I tried to read the error code, but when I send the command to get the last error code it says there are non. And in life info feat on the computer it says DRV but I can't see more info. 

My setup:
10s2p
4.12 VESC
Turnigy Aerodrive SK3 - 6374-192KV
FOC mode

Someone who can help me?
Thanks,
```

---
## \#2 Posted by: Eboosted Posted at: 2017-12-24T04:08:26.324Z Reads: 142

```
Switch to BLDC mode before you fry your VESC.
```

---
## \#3 Posted by: bimmer Posted at: 2017-12-24T05:03:00.047Z Reads: 133

```
What did you use to setup your vesc? Vesc tool or the old bldc one? When I switched Foc stopped killing my vesc's.
```

---
## \#4 Posted by: lansselot Posted at: 2017-12-24T12:35:38.924Z Reads: 123

```
I used BLDC tool from http://www.electric-skateboard.builders/t/extended-bldc-tool-with-watt-control-mode-ppm-cruise-control-individual-throttle-curve-and-android-app/12286

I will try BLDC mode, and have a look if that fix the problem. 
Bud I have read a lot of topics about BLDC VS FOC and if FOC blows up your VESC.  I understood that there are a lot of people who use FOC mode without any problem and is was mostly configuration folds. 
But this isn't true?

Thanks for you're help and have a nice Christmas.
```

---
## \#5 Posted by: telnoi Posted at: 2017-12-24T12:52:22.115Z Reads: 112

```
What controller do you have? Not all Vesc can run foc without going into self-destruct mode.
```

---
## \#6 Posted by: lansselot Posted at: 2017-12-24T13:31:20.675Z Reads: 104

```
I have this controller: http://e-greenmotion.com/index.php?route=product/product&product_id=282&search=4.12VESC+BLDC+Electric+Skateboard+ESC+
But can that explain the strange behaviour when the board is "cold"?
```

---
## \#7 Posted by: telnoi Posted at: 2017-12-24T13:47:53.310Z Reads: 101

```
They are as far as known here rebranded Maytech VESC and should only be operated in bldc. 

Temperature dependent deviations might be due to poor solder connections.

Also read this thread:
http://www.electric-skateboard.builders/t/has-anyone-used-these-vescs-green-motion/31256/12

You'll find allot of troubleshooting advice for maytech VESCs, including upgrading buggy firmware.
```

---
## \#8 Posted by: rich Posted at: 2017-12-24T14:20:12.172Z Reads: 92

```
Switch to BLDC mode and all your troubles fade away...
Your controller is not made for FOC. But switch to new firmware and VESC-Tool. The firmware on maytech/greenmotion is buggy! You must upload bootloader in VESC-Tool first but that's easy. And your motor is without sensor so usually you have to push once before hitting the throttle.
```

---
## \#9 Posted by: lansselot Posted at: 2017-12-24T16:08:04.714Z Reads: 86

```
So the "extended BLDC tool" is outdated?
I will check Al my connection and try the board in BLDC when the board is done charging.
```

---
## \#10 Posted by: rich Posted at: 2017-12-24T16:23:12.336Z Reads: 89

```
There is new software and firmware available. But the main problem is the buggy firmware 2.18 on maytech/greenmotion, or is there different firmware now? BTW BLDC Tool is the software, VESC Tool is the new version of it (in combination with new firmware). Which FW do you use?
```

---
## \#11 Posted by: piepolitb Posted at: 2018-05-21T15:35:50.145Z Reads: 67

```
Hi @lansselot and everyone else, I pick up this post from the dead: did you solve the issue?
I'm in the exact same situation with a VESC from torqueboards running BLDC.
I found out later the weird behavior, at first I thought I was just getting the 3 LED blinking, the I tried the jump start

here is my post http://www.electric-skateboard.builders/t/vesc-fault-drv-not-spinning-the-motor-anymore/55936/8
```

---
## \#12 Posted by: lansselot Posted at: 2018-05-22T06:39:23.976Z Reads: 57

```
I didn't wend on with fixing my board. With Christmas and renovating and moving to a new house + my last year of school so I had to make a lot of reports resolved in my board laying there on the bench. :sweat_smile:
I also demolish my battery case and motor support.. 

But with the incoming summer and the weather that comes with it I :sunglasses:, last week, ordered some polyester to make a new case. And I coincidental took my drive train to school today to fix my motor mount.
I haven’t had my VESC on my computer since so I still don’t know my FM version. But I am going to get busy with fixing my board.
I will watch you’re post to maybe find an answer to my original problem.

hopfuly you wil find you're problem.
```

---
## \#13 Posted by: lansselot Posted at: 2018-10-26T20:41:31.455Z Reads: 30

```
Sorry people, long time no see.
My problem fix was putting my vesc back to bldc mode. Never had a problem since. 

It's a pity I can't use foc bud it doesn't matter that mutch. 

I did a big upgrade of my board and I will post a update soon, for the people who are interested.
```

---

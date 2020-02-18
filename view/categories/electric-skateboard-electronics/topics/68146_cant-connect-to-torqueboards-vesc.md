# Cant connect to torqueboards vesc

### Replies: 18 Views: 352

## \#1 Posted by: 3dman Posted at: 2018-09-15T21:18:44.739Z Reads: 98

```
Hi
So I bought this Vesc from diy electricskateboard (4.12 Hardware, software version is unknown) late November 2017 but have not had time to do the actually build until recently.
I connected the vesc to my laptop for the very first time today and started up the latest Vesc Tool. After locating the correct COM port and pushing "connect" I get the following error pop up message:

_The firmware on the connected VESC is too old. Please update it using a programmer._

Is it possible to use and older version of the VESC tool/BLDC tool to update the firmware on my vesc?
If so, could someone please point me in a direction of which version I should be trying. Because I am afraid of "frying" my vesc by using wrong version.

Thanks.
```

---
## \#2 Posted by: J0ker3366 Posted at: 2018-09-15T21:21:43.099Z Reads: 92

```
https://www.electric-skateboard.builders/search
```

---
## \#3 Posted by: dareno Posted at: 2018-09-15T21:49:40.318Z Reads: 87

```
Try chucking a pm at @torqueboards 
I've only updated firmware using the tab in vesc tool on HK versions and that was fine but you'd better check first.
```

---
## \#4 Posted by: trancejunkiexxl Posted at: 2018-09-15T22:05:05.681Z Reads: 77

```
They have a chat feature and are pretty quick
```

---
## \#5 Posted by: Bor.inc Posted at: 2018-09-15T23:07:40.389Z Reads: 69

```
hahahahahah @J0ker3366 wp
```

---
## \#6 Posted by: threebysix Posted at: 2018-09-16T00:00:06.426Z Reads: 64

```
Maybe shoot a dm to @Ackmaniac as well. See if you could flash it with his latest firmware.
```

---
## \#7 Posted by: torqueboards Posted at: 2018-09-16T02:33:23.615Z Reads: 62

```
@3dman Make sure you download the latest VESC Tool. Sometimes you see that error if you're using an older tool and that VESC may have a more updated firmware. You'll definitely need to update the firmware to the latest.
```

---
## \#8 Posted by: 3dman Posted at: 2018-09-16T12:43:18.979Z Reads: 56

```
thanks for the respond, folks!

Yes, I have tried diyelectricskateboard builders chat, but they could not help me. I was asked to send them a mail.

@torqueboards. I am running the latest VESC tool downloaded yesterday from VESC project. Please help me, how do I upgrade the firmware without the VESC tool? I read something online about ST2 link, is this the way to go?
```

---
## \#9 Posted by: trancejunkiexxl Posted at: 2018-09-16T13:31:51.939Z Reads: 48

```
if you can still connect and receive the fw too old message then you do not need STlink
```

---
## \#10 Posted by: torqueboards Posted at: 2018-09-16T21:37:32.679Z Reads: 45

```
@3dman - Yeah, Stlink would work for sure. Email us and we can do it for you also. Just pay shipping.
```

---
## \#11 Posted by: 3dman Posted at: 2018-09-17T04:44:07.647Z Reads: 38

```
@trancejunkiexxl, when I try to connect to VESC tool I get the mentioned message "fw to old". So how do I connect to update firmware without ST link cable and no connection with VESC?

@torqueboards, I appreciate the offer, I will probably get a ST link cable for the shipping price I would have to pay from Norway.
```

---
## \#12 Posted by: trancejunkiexxl Posted at: 2018-09-17T05:05:16.199Z Reads: 31

```
If your using the latest ackmaniac software it was only a matter of hitting update for me.  In the event of missing bootloader I couldn't even get the devices to be seen period.. took more effort
```

---
## \#13 Posted by: 3dman Posted at: 2018-09-17T05:18:48.106Z Reads: 32

```
I beleve the torqueboards vesc is shipped with bootloader as standard (@torqueboards ?). I did try the ackmaniac software as well (VESC Tool mod). But same error message.

trancejunkiexxl, can you confirm if you also got the same error message that I am facing?
```

---
## \#14 Posted by: PredatorBoards Posted at: 2018-09-17T05:24:15.150Z Reads: 31

```
You should invest in an STLink anyways, just in case something gets bricked in the future.
```

---
## \#15 Posted by: trancejunkiexxl Posted at: 2018-09-17T17:54:34.515Z Reads: 24

```
@JohnnyMeduse might be able to help u better. If ur short on cash and need programmer  u can borrow my stlink I'll ship it.
```

---
## \#16 Posted by: 3dman Posted at: 2018-09-17T18:08:54.482Z Reads: 26

```
@trancejunkiexxl, I appreciate the offer:-) I am located in Norway, so it might be a bit far? I just order one from the far east, but that is sent with snail-Mail..

So if it is possible to solve this without the ST link cable that would be the best!
```

---
## \#17 Posted by: Hansg Posted at: 2019-04-10T16:22:24.029Z Reads: 12

```
Hello @3dman,

Can you fix this error? I have the same error I cant upgrade my firmware, could you help me please?
```

---
## \#18 Posted by: 3dman Posted at: 2019-04-10T19:20:05.304Z Reads: 7

```
Hi Hansg.
I ordered the stlink as suggested above, but I have not found time to finish the project or try the update. Please jet me know if you manage to fix it!
```

---

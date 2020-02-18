# TORQUEBOARDS 2.4GHZ Nano controller trigger NOT WORKING when paired and in correct channel

### Replies: 9 Views: 511

## \#1 Posted by: Fraserrazor Posted at: 2018-05-02T19:49:32.216Z Reads: 84

```
Dear Esk8ing community,

I have recently started a new electric longboard build with dual belt driven motors. Upon downloading the BLDC tool, I have noticed that my controller (although paired and in correct channel) does not output anything to the single motor I am currently testing i.e the motor is not spinning. This cannot be a motor issue because I can spin the motor direct through the BLDC.

Anyone any ideas on how to fix as I have been playing around with the BLDC and have watched countless videos on existing threads in trying to fix this problem?

My controller is the torqueboards 2.4GHZ nano controller.
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2018-05-02T20:20:20.658Z Reads: 69

```
check to see if your servo cable is orientated correctly might have it upsidedown
```

---
## \#3 Posted by: BigBrit Posted at: 2018-05-02T22:54:50.309Z Reads: 58

```
This exact same thing happened to me a few days ago when I was programming my new DIY.  Swap the vesc cable that plugs into receiver round 180 degrees.  Seems the middle pin is the one that gives you the connection so you get your symptoms if its plugged the wrong way round.
```

---
## \#4 Posted by: mmaner Posted at: 2018-05-03T01:50:07.655Z Reads: 49

```
The ground wire (black) should be to the outside if the RX.
```

---
## \#5 Posted by: Fraserrazor Posted at: 2018-05-03T11:17:45.846Z Reads: 45

```
I have tried re-orientating my servo cable a number of times but with no effect. I am going to try again later tonight in case I was just unlucky. I will post if anything changes or doesn't.

Thanks anyway
```

---
## \#6 Posted by: trancejunkiexxl Posted at: 2018-05-03T13:39:36.482Z Reads: 39

```
shouldnt be to hard to replace the controller, id keep an extra one jic something like this happens again. u can get a cheaper one if price is an issue.. [controller](https://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-w-Receiver-Binding-Plug-for-Electric-Skateboard/263592631161?hash=item3d5f585b79:g:FzwAAOSwdoNayJWW)
```

---
## \#7 Posted by: Fraserrazor Posted at: 2018-05-03T13:54:53.140Z Reads: 39

```
If it doesn't work i'll contact torqueboards but thanks for the link.
```

---
## \#8 Posted by: banjaxxed Posted at: 2018-05-03T15:51:47.784Z Reads: 33

```
Screen of your app settings? ensure the correct option for controller is chosen
```

---
## \#9 Posted by: Fraserrazor Posted at: 2018-05-03T18:08:00.976Z Reads: 25

```
Thanks everyone for your help. I played around the BLDC tool in app configuration and then repaired the remote to the transmitter after constantly reconnecting my servo connector and now the connection works. The motors are spinning and I can now use the Torqueboard remote. Anyone who has this problem should download the BLDC tool from enertion http://www.enertionboards.com/new-focbox-speed-controller/focbox-bldc-tool-win/ and should also keep attaching and removing your servo connector to what this tutorial suggests https://www.youtube.com/watch?v=SOjPTMa0Bew&t=23s . 

Cheers
```

---

# Can I connect my nano x to my gt2b receiver?

### Replies: 6 Views: 1082

## \#1 Posted by: Kaden56 Posted at: 2017-01-25T23:37:45.415Z Reads: 116

```
**Why on earth would I care to do this?** Two reasons.

1.) My nano x receiver is faulty and I was told to send it to enertions place in canada and they'll fix it or replace it. 

2.) I tried powering a usb powered led strip for underglow on my board with the 2nd channel on the nano x and it would turn on but it was only half the brightness that they normally are and the led strip wouldn't respond to remote that the led strip came with to change colors and things. However if I hook up my gt2b receiver I can plug the led strip into the s+- row (i'm assuming it's for servos?) and it powers up to full brightness and responds to the led remote great. 

**What would be ideal?** 

I would like to use my nano x obviously (the remote is freaking awesome) and be able to turn the led strip on and off with the 2nd channel button and also use the color changing remote if I ever want to. Because I couldn't get it to power on fully or consistently with the nano x receiver I would like to use the gt2b receiver. 

**What I need to know:**

1.) How would I pair the nano x to the gt2b receiver (or if it's possible at all)

2.) How would the channels work out beings that the trigger on my gt2b is controlled by the second channel on it's receiver? Would I be able to pair it to the nano x with the trigger being on the first channel of the gt2b receiver so the second channel is the button on the nano x controller? 

Pictures:
<img src="/uploads/db1493/original/3X/7/1/71df09dcd59c5cecefca5a60833407c1e3eb8ba2.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/6/5/65f0b7a9c9b00159c7195a41be19683bd96d8eef.JPG" width="375" height="500"><img src="/uploads/db1493/original/3X/9/e/9e93ec869dff35cc1bcea0dc738f7b29f6d71812.JPG" width="375" height="500">

Thank you for any responses!
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-01-25T23:53:47.825Z Reads: 102

```
First.... No I won't work... 

Second... for the nano x receiver and even with the gt2b receiver I suggest to use a external power source to power up your led... mostly around 12v and use your remote as a switch... (a bit like the vedder switch works) It should prevent your receiver from blowing up since your asking for more power that it can produce

Third... for the channel 2 operate on the nanox you need to push the button for around 10sec
```

---
## \#3 Posted by: Kaden56 Posted at: 2017-01-25T23:58:32.927Z Reads: 98

```
Can you explain why it won't work? I'm just trying to learn. Are all 2.4ghz receiver different and will only work with specific remotes? 

The led strip requires only 5v and I think it pulls like 1 amp. Is that more than the gt2b receiver can handle?

The channel 2 on my nano x turns on and off within about 3 to 4 seconds of holding the button.
```

---
## \#4 Posted by: Schulerbible Posted at: 2017-01-26T00:28:26.237Z Reads: 91

```
I am not sure why it won't work but I found some info in an RC forum:

> The general rule is that on 2.4 GHz, the brands of the transmitter and 
> receiver have to be the same. There are exceptions though. Here are a 
> few that I can think of:

> * A JR 2.4 Ghz radio will work with a Spektrum receiver as long as both say "DSM2."For some module-based radios, there are 2.4 GHz modules that adapt the radios to other systems. For example, you can buy a module for a Futaba radio that will make it compatible with Spektrum receivers.

> * Hobby King sells something they call the Orange Receiver that works with Spektrum and JR 2.4 Ghz radios

> * Hobby King also sells the Corona system that can adapt many different radio brands to use their own 2.4 GHz system. 

> That's just a start. I'm sure there are more examples, and there will probably be even more in the future.
		
Source: [https://www.rcgroups.com/forums/showthread.php?1344552-Different-Brand-Receiver-Interchangeability](https://www.rcgroups.com/forums/showthread.php?1344552-Different-Brand-Receiver-Interchangeability)

Btw. my GT2E receiver is also not compatible with the Nano-X.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-01-26T05:37:19.710Z Reads: 74

```
Sorry for the late answer...

<img src="/uploads/db1493/original/3X/1/3/13e7de98ee2cdf04b9776f596e00345823358462.JPG" width="374" height="500">

As you can see in the picture the two receiver, even if they work with the same frequency, have two completely different systeme of operation. The one on the top (nanox), use a custom made ic, also with probably a custom firmware from the manufaturer. And the bottom one (Gt2b) use a differnt chip (witch is a serial eeprom, from what i can find)... so on this one the data is probably decode by the tranceiver.

Also, the current is not determined by the receiver, but the vesc witch is limited to 1.5Amp (if I'm not mistaken), but why I suggest to use a external power source is because the 5v is straight from the DRV, so even if you're still in operating range, if something short your led strip or draw more current, guess wich part will suffer first.
```

---
## \#6 Posted by: Kaden56 Posted at: 2017-01-26T17:54:56.162Z Reads: 60

```
Thank you so much for that! So informative! Good to know about the 5v sorce coming from the DRV too. I'll have to start figuring out how I want to go about hooking everything up. Thanks again!
```

---

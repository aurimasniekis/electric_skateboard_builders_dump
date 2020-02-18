# Flipsky mini vesc4.20 solid blue light and not connecting to laptop

### Replies: 14 Views: 250

## \#1 Posted by: FirstTimeBuilder Posted at: 2019-05-26T20:09:16.933Z Reads: 60

```
Hey all, 

Ive got a new mini vesc4.20 and for some reason my laptop doesnt recognise its connected and all i get is a solid blue light on the vesc. Its not the port as ive connected my dual flipsky vesc with no issues. Anyone had this before and have any idea whats going on?

This is the link to the vesc incase needed 
https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike

Thanks in advance
```

---
## \#2 Posted by: JakeSkate Posted at: 2019-05-26T20:21:25.503Z Reads: 59

```
What OS are you running the program on? And is the cable you are using just a charging cable with two wires or is it the same one you used with your other controller?

Another thing I would check is that your vesc is showing up under devices and or on the correct com port.

Maybe try to power it off the battery pack that your used for your other controller.
```

---
## \#3 Posted by: FirstTimeBuilder Posted at: 2019-05-26T22:32:32.040Z Reads: 53

```
Hey, 

Using windows 10 and the Vesc tool software. Ive tried a number of different cables including the one that works with the other vesc. 

I havnt tried the other batteries though so will give that a go and report back

Cheers
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-05-27T00:36:37.469Z Reads: 48

```
the new firmware is rather buggy still it seems. i had to revert back to the older release to "unbrick" a vesc i had thought was cooked. it was just firmware issues with the newest vesc tool. im running .95 now with no issues.
```

---
## \#5 Posted by: Gamer43 Posted at: 2019-05-27T00:42:39.254Z Reads: 46

```
Sounds like a firmware issue, the STM32 is either blank or bricked somehow, as there should also be a green light.

You will need an st-link to reprogram it, I'd recommend getting a $10 nucleo-64 board of Arrow.com and using its embedded st-link.
```

---
## \#6 Posted by: eparks11 Posted at: 2019-06-14T17:12:54.678Z Reads: 31

```
Were you able to get your mini vesc connected to your PC? I'm having the exact same issue. I've tried everything I can think of to connect mine, but no luck. I've downloaded drivers from here: https://www.st.com/en/development-tools/stsw-stm32102.html

That did't help. Tried both USB 2 & 3 ports, tried multiple cables. Powered the board on and off multiple times. Restarted my computer multiple times....all nothing. My PC simply won't recognize the Flipsky VESC, and I'm at a bit of a loss as to what to try next.
```

---
## \#7 Posted by: FirstTimeBuilder Posted at: 2019-06-14T19:02:02.700Z Reads: 28

```
Hi, 

Nope. Still nothing, im having so much trouble with the st link as well. Ive found someone who will flash it for me but will cost 35euro each. Im struggling to find the HEX file as well so even if i did manage to connect it i cant really do much anyway
```

---
## \#8 Posted by: eparks11 Posted at: 2019-06-14T21:20:04.279Z Reads: 24

```
Well that stinks. My next course of action is to borrow a friends laptop and see if it will connect to that one, but I'm not expecting that to work either.
```

---
## \#9 Posted by: eparks11 Posted at: 2019-07-06T13:14:56.916Z Reads: 20

```
Still no luck on my end as far as getting my mini VESC to connect. I’ve tried 3 different computers, all three shut down the USB due to excessive power draw. I bought a Bluetooth module in hopes that would work, but that won’t connect either. 

I’ve given up at this point and have asked Flipsky for a refund, but they don’t seem very open to that. They instead want to sell me a different VESC at a slightly discounted rate. which I find insulting to be honest, it seems like the least they could do is sell me a replacement at cost. 

I’m just going to buy from a different vendor since I no longer feel I can trust them. It sucks, I ordered $270 worth of parts from them, and they’re forcing me to fight them on returning just one of the items. My next course of action will be a credit card dispute in hopes I’ll get my money back that way.
```

---
## \#10 Posted by: FirstTimeBuilder Posted at: 2019-07-06T16:00:22.639Z Reads: 18

```
Hi, that sucks! 

Ive sent mine to a guy called Martin over in Slavakia to fix for me. Email him on customerservicesprusi@gmail.com. 35euro is better than buying new. Plus it includes him sending them back to you. 

I told them about my issue and got a similar response. They said they have a sale coming up and buy a new one!! They make great products but their customer service when something goes wrong sucks! 

Did you pay through paypal?
```

---
## \#11 Posted by: eparks11 Posted at: 2019-07-16T08:11:02.785Z Reads: 15

```
Thanks for the reply, I decided just to buy a Flipsky 4.12 VESC off of Amazon so I could return it if it didn’t work. Board is done now and working great (see attached photo).

I did indeed buy through PayPal, so I’m attempting to get my money back that way. Flipsky hasn’t responded via PayPal, they instead sent me another Facebook message saying they were surprised I went that route since they “offered me a discounted replacement”. Keep in mind that discounted replacement was no cheaper than I could have bought it on eBay for, so I found their token gesture pretty insulting. 

They also once again said they don’t do refunds because it’s against their policy...I guess they have no control over their own policy?

Anyway, I’ll figure out something to do with the mini vesc. It’s currently just collecting dust in a drawer. Unfortunately I live in the US, so I’m not sure if it makes any sense for me to pay for shipping over to Europe for repair. May just list it on here for sale: $5 or best offer :slight_smile: 

![image|666x500](upload://1sruJfwnW91BkF2vZ1f58We70xV.jpeg)
```

---
## \#12 Posted by: FirstTimeBuilder Posted at: 2019-07-16T08:35:46.670Z Reads: 13

```
Hey, 

The board looks awesome!

WOW Flipsky really suck at their customer service! 

Might be worth asking the question to the US people on here to see if anyone fixes them. Get more money for it afterwards, plus people on here are always looking for stuff.

Where abouts in the US are you, were heading upto Michigan in September to visit friends.

I'm converting mine into another project. Dual motor scooter with golf buggy wheels, design idea attached.

![66154048_763844767351276_9042039982201503744_n|690x390](upload://4stTPHVmddzCSMMx1WmBhNa9Xs4.jpeg)
```

---
## \#13 Posted by: eparks11 Posted at: 2019-07-16T08:51:28.503Z Reads: 13

```
Ha! That’s crazy. I live in Charlotte, NC. 

Post a pic of the scooter when you’re done. I’m currently looking for ideas for something I can ride on rainy days, so I’ve started researching diy scooters and ebikes to go along with my skateboard.
```

---
## \#14 Posted by: FirstTimeBuilder Posted at: 2019-07-16T09:48:42.308Z Reads: 11

```
Yea its going to be amazing! These are the tyres lol ![IMG-20190709-WA0000|281x500](upload://psDY17uI2jsT1lC9leFwg8iWxIm.jpeg)
```

---

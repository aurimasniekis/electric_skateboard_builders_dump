# Wireless Playchuck &#124; Not a Nyko &#124; Kinda working, not really though

### Replies: 8 Views: 721

## \#1 Posted by: patrickgoeler Posted at: 2017-07-24T09:03:07.734Z Reads: 73

```
Hey, so I almost finished my build and as a remote I wanted a nunchuck. Since I did not get my hands on a Nyko I ordered a similar one. (https://www.amazon.de/gp/product/B001WYAB5W/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1). I soldered all the connections on to the PCB and the other ends on to the VESC. (3,3V, GND, Data and Clock). In the BLDC I chose Nunchuck in the App Configuration and if I display the input amount in the Nunchuck-Tab it shows something.

Now here is the problem: 
If I give it full throttle it takes something like 3-6 seconds for the input to go from 50% to 100%, same for any other changes I make to the throttle.
As far as I know changes to the throttle should be displayed immediately..

I did not have the chance yet to test it on the motor, but any idea how to make the input consistent?

Thanks so much!
```

---
## \#2 Posted by: Maxid Posted at: 2017-07-24T10:16:49.242Z Reads: 66

```
The VESC only works with Nyko Kamas.
Any other Nunchuck will not work.
If by any chance you find one let us know - we have all been searching for ages to find an alternative to the Nyko.
```

---
## \#3 Posted by: patrickgoeler Posted at: 2017-07-24T10:43:39.578Z Reads: 58

```
I knew that I was making a bet, but I really wanted to try it out. Since I can move the input bar from 0% to 100% it should work with the motor as well right? It would suck though, if the motor took 6 seconds before reacting to my breaking signal..
```

---
## \#4 Posted by: rpn314 Posted at: 2017-07-24T14:02:00.068Z Reads: 45

```
Another nunchuck option I'd recommend is the modded nunchuck that vedder designed (replace the internal board in a regular nunchuck).

https://www.electric-skateboard.builders/t/vesc-nunchuk-rf/588?u=rpn314

Edited: to reflect @Maxid's comment below
```

---
## \#5 Posted by: Maxid Posted at: 2017-07-24T14:08:07.923Z Reads: 40

```
I put the data lines of my Nyko through a ferrite and never had a single issue.
```

---
## \#6 Posted by: rpn314 Posted at: 2017-07-24T14:09:20.808Z Reads: 38

```
Really? I hadn't heard that ferrite rings fix the nyko issues; that's fantastic! Too bad Kamas seem pretty difficult to find now-a-days :frowning:
```

---
## \#7 Posted by: Maxid Posted at: 2017-07-24T14:12:42.117Z Reads: 38

```
http://www.electric-skateboard.builders/t/vesc-faq-connect-the-nyko-kama-wireless-wii-nunchuck/139/59
```

---
## \#8 Posted by: lowGuido Posted at: 2017-07-24T16:08:12.811Z Reads: 28

```
the toroid helps but soldering is king!
people who try to plug the dongle in directly are going to street their face.
```

---

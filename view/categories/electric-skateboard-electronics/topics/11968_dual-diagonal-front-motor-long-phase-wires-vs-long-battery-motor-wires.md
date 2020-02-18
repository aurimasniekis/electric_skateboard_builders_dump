# Dual diagonal front motor. Long phase wires VS long battery &gt; motor wires?

### Replies: 9 Views: 1214

## \#1 Posted by: michaelcpg Posted at: 2016-10-26T21:46:23.620Z Reads: 220

```
I'm in the process of redesigning my board with a new deck and will be sticking with a dual diagonal setup (largely because I'm using Ollin motors on Calibers). 

Just trying to work out whether I should mount one of my VESCs at the front of my board so that the phase wires for the front motor are short but the wires between the front VESC and battery are longer or would it be better to have both VESCs at the back of the board so that the wires between the VESCs and batteries are short but the front motor's phase wires are longer? 

Is there actually any significant difference either way?

Cheers
```

---
## \#2 Posted by: lox897 Posted at: 2016-10-26T21:48:39.843Z Reads: 219

```
Have the battery in the middle and VESCs on either side. Motor wires should be short and it's ok if the battery wires are under 20cm
```

---
## \#3 Posted by: Jinra Posted at: 2016-10-26T21:49:27.061Z Reads: 217

```
I use long phase wires as I prefer to have a short connection from battery to ESC. Also if you have 2 VESCs far away you'll need a loooong servo split/CAN cable.

http://www.electric-skateboard.builders/t/honey-driver-honey-velocity-v3-deck-caliber-iis-83mm-evolve-gt-wheels-dual-om5065-200kv-space-cell-pro4-diy-pulleys-enertion-pulley-bones-super-reds-enertion-mounts-winning-remote-chaka-vescs-build-complete/5760
```

---
## \#4 Posted by: michaelcpg Posted at: 2016-10-26T21:54:01.667Z Reads: 194

```
I'm doing a split battery Vanguard build so can't have the battery in the middle unfortunately.

My current build uses long phase wires which I've had no issues with but having long battery wires instead would be kind of nice as it'd mean I'd need one less large wire running down the deck
```

---
## \#5 Posted by: Jinra Posted at: 2016-10-26T22:10:20.458Z Reads: 182

```
Keep in mind long wires causes problems with FOC.
```

---
## \#6 Posted by: michaelcpg Posted at: 2016-10-26T22:21:09.351Z Reads: 179

```
Yea that's one thing I've been thinking about, even though I don't really have any plans to use FOC at the moment. 
Any idea whether the problems with FOC and long wires are dependent on which wires are longer?
```

---
## \#7 Posted by: Jinra Posted at: 2016-10-26T22:24:26.834Z Reads: 186

```
I don't think it matters, but at the same time I have no idea why it causes problems in the first place. My other point remains, even if you have 2 wires for the battery to extend to the front VESC, you need a long servo/can cable too to reach the other VESC.
```

---
## \#8 Posted by: Hummie Posted at: 2018-03-08T20:52:31.584Z Reads: 88

```
how long is too long for motor wires for bldc or foc?  getting test failures and wondering if its the long wires
```

---
## \#9 Posted by: michaelcpg Posted at: 2018-03-08T21:08:38.712Z Reads: 87

```
From what I've read, long motor wires seem to be better than long battery wires, unless you have an extra large capacitor bank by your ESCs. My first board had motor wires roughly 2ft long to the front motor and I never had any issues if that helps.
```

---

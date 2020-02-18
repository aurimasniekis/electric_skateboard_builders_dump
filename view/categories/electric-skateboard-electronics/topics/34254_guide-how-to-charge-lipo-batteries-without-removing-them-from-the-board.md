# \[GUIDE\] How to charge LiPo batteries without removing them from the board

### Replies: 9 Views: 1576

## \#1 Posted by: danieloath Posted at: 2017-09-29T07:41:48.551Z Reads: 194

```
For those of us that choose to use LiPo batteries, whether it be for the financial savings or the (generally) higher discharge rates, we can find ourselves restricted to the types of enclosures we can make or choose from due to the fact that the battery charge leads and balance leads need to be easily and readily accessible when it comes time to charge them, and short of using tupperware containers for enclosures, or gluing our XT60/90 connectors into our enclosures and having them exposed to puddles due to lack of weatherproof shielding or appropriate panel mounting hardware, we don't have too many options.

I've drawn up a wiring schematic showing how I plan to circumnavigate this issue, allowing me to make use of a standard DC panel mount with waterproof cap, and a cheap means of disconnecting the ESC during charging. An SPDT switch would also work, and would be preferable to many, but the basic principal still stands, whatever your method of disconnect happens to be.

I hope that people find this somewhat useful if they're planning a first build with LiPo's.

<img src="/uploads/db1493/original/3X/4/0/4042f795aa2478d73e093c8a23476955aff609cd.jpg" width="690" height="487">

EDIT: This method allows the user to replace the battery without resoldering or rewiring any components.
```

---
## \#2 Posted by: Okami Posted at: 2017-09-29T08:32:57.442Z Reads: 187

```
I would advice to put [schematic] or [guide] in the title or tags, otherwise it looked like u are seeking answers when in fact you offer a solution.

Otherwise a very nice and clean drawing. Congrats / appreciation for that

I still dont know why some people just dont make parallel plugs in the first place, it might be that they just dont think about it in the first place and realize this only later when they need to charge the board.

What i also find very useful is balance wire extender, usually these balance wires are quite short for lipo batteries
```

---
## \#3 Posted by: Grozniy Posted at: 2017-09-29T10:47:10.704Z Reads: 178

```
hey. Could you link this peace please?<img src="/uploads/db1493/original/3X/9/0/90b7ad26dd21b0d1307ea2ea575d432d2cd551ca.jpg" width="690" height="487">
```

---
## \#4 Posted by: scrapheap Posted at: 2017-09-29T13:02:28.354Z Reads: 156

```
[https://hobbyking.com/en_us/2-1mm-dc-power-plug-with-screw-terminal-block-5pcs.html](https://hobbyking.com/en_us/2-1mm-dc-power-plug-with-screw-terminal-block-5pcs.html)

[http://www.ebay.com/itm/10pcs-Waterproof-5-5-x2-1mm-DC-Socket-Power-Jack-Plug-Female-Mount-Connector-TB-/202036303768?hash=item2f0a4d5798:g:akcAAOSwdj9XT412](http://www.ebay.com/itm/10pcs-Waterproof-5-5-x2-1mm-DC-Socket-Power-Jack-Plug-Female-Mount-Connector-TB-/202036303768?hash=item2f0a4d5798:g:akcAAOSwdj9XT412)

Plenty to choose from if you just look, these are just examples.
```

---
## \#5 Posted by: danieloath Posted at: 2017-09-29T13:11:57.639Z Reads: 151

```
@scrapheap has given a couple of links to some options for you. I personally obtained these parts from my local electrical supply shop. :slight_smile:
```

---
## \#6 Posted by: Crossfire Posted at: 2017-09-29T13:45:41.962Z Reads: 145

```
I’d be more interested in a parallel charge/serial discharge option without removing them serial cable for 2 or more lipos :slight_smile: 
The one posted is OK for max 5S-6S setups. 8, 10 and 12 S is where the fun part begins...riding and charging :)
```

---
## \#7 Posted by: danieloath Posted at: 2017-09-29T13:54:35.612Z Reads: 139

```
Now that would be something. Definitely need a SPDT switch for that setup.

You're correct in saying that this setup is only good for simple battery arrays. I, personally, am running a 6S1P. ;)

Thanks for your input!
```

---
## \#8 Posted by: Crossfire Posted at: 2017-09-29T14:05:57.982Z Reads: 134

```
I use my hobby charger for 2x 5S4P Lion 30Q cells. When riding I connect them together in series 10S, when charging they're in parallel safely at 12A. Charging time for 12Ah battery around 2h. Using BMS? At least like 5 or 6h. 

I just need to unplug the serial cable and connect the batteries with power and balance cables. 30 seconds job. :)
```

---
## \#9 Posted by: eranmo Posted at: 2019-08-14T21:47:03.539Z Reads: 28

```
SPDT or DPDT does not work in high current applications, they are all good for 50A max, the one that are rated at 200A will do fine but not to portable setups that relay on the lipo power, not even the most expansive Relays/SSRs.
They simply bring too much resistance and heat that damage the solder/connectors (also reduce run time) and may blow up your ESC.
```

---

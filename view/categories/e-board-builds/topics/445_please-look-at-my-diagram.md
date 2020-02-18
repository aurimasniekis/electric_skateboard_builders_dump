# Please look at my diagram

### Replies: 16 Views: 3074

## \#1 Posted by: sgaana Posted at: 2015-11-11T08:15:11.900Z Reads: 131

```
I have few questions:
What type of wires to use to connect two VESCs? The connector is called JST-PH2MM ?
What is CanBus? Is it a protocol or an actual component? 

<img src="/uploads/db1493/original/1X/df5b9811c0277ec7edc7424eae1bf6bc977b051c.png" width="647" height="500">
```

---
## \#2 Posted by: trbt555 Posted at: 2015-11-11T08:32:24.042Z Reads: 123

```
Canbus is a widely used protocol in industry. It is also widely used in automotive applications. [CANbus][1]
Here's a source for the connector: [JST PH 2mm 4-pin][2]
You'll also find 6-pin connectors.


  [1]: https://en.m.wikipedia.org/wiki/CAN_bus
  [2]: http://www.benl.ebay.be/itm/JST-2-0mm-PH-4-Pin-Connector-with-Wire-x-10-Sets-/181441351403?hash=item2a3ebf4eeb:g:Lk0AAMXQDK1Rx6Of
```

---
## \#3 Posted by: sgaana Posted at: 2015-11-11T17:25:16.604Z Reads: 116

```
@trbt555 thanks. 
What type of wires are those in blue and green?
http://www.electric-skateboard.builders/uploads/db1493/optimized/1X/fd512974e0f361a1edf6f33b492f868b9f2f18fa_1_669x499.jpg
```

---
## \#4 Posted by: trbt555 Posted at: 2015-11-11T18:11:05.007Z Reads: 118

```
Not sure I understand your question.
Just plain ordinary wires which come with the JST connectors are fine.
```

---
## \#5 Posted by: kai Posted at: 2015-11-11T22:01:26.581Z Reads: 118

```
If you are going to crimp your own jst ph female connectors the wire size depends on which connector contacts you get. I think they are 26 to 32 gauge wires. http://www.digikey.com/catalog/en/partgroup/ph-series/8871
But i haven't done it before so dont take my word for it. I was just looking into it myself so i could be wrong.
 It would be easier to get the jst connector with the wires on it already and solder the wires together then to crimp every wire and jamming it in the connector.
On a side note... do you have all your parts already? We are building the exact same build. Would you document your progress in a thread so i can see how yours goes?
```

---
## \#6 Posted by: onloop Posted at: 2015-11-11T23:45:16.034Z Reads: 113

```
use any wire and just solder onto the pins on the other side of pcb. maybe put some hot glue on that solder joint and also around the wire to ensure it doesnt get snapped off.
```

---
## \#7 Posted by: sgaana Posted at: 2015-11-12T00:01:28.654Z Reads: 113

```
@kai Most of the components have arrived except Space Cell.  But I still have to pick them up in my mailbox across the US border. I am anticipating to start my build in mid December. 
Once I have all the electronics, I will look for a deck. Both Rayne and Landyachtz are located in my home town Vancouver. I'm sure I can find a light and flat deck. 
For sure will post a thread with lots of pictures. I have been reading yours as well. Good luck!
```

---
## \#8 Posted by: sgaana Posted at: 2015-11-12T00:03:51.151Z Reads: 111

```
@onloop thanks. Just waiting for Space cell to start my build.
```

---
## \#9 Posted by: onloop Posted at: 2015-11-12T00:39:52.845Z Reads: 102

```
whats the order number? ill check its status
```

---
## \#10 Posted by: sgaana Posted at: 2015-11-12T03:48:11.452Z Reads: 102

```
@onloop my mailbox company just received a package sent from Shenzhen (7x18x6 in, 2.68kg). It must be SPACE cell. 
So, I am just waiting for VESC order #1104. I just tracked it, and is in Los Angeles on its way to Washington State. All is good. Cheers.
```

---
## \#11 Posted by: kai Posted at: 2015-11-12T05:02:12.400Z Reads: 100

```
i wont be getting my vesc till mid november batch and jerry from carvon said i would get my hub motors mid nov, but i have everything else. my space battery came yesterday but i started pressing a new deck cause i think my first one was to flexible. going 8 ply canadian maple 2 sheets of fiberglass this time.
why wait till mid december to start building when it sounds like u will have all your components soon? i would be to excited to not start haha
```

---
## \#12 Posted by: sgaana Posted at: 2015-11-12T05:39:55.393Z Reads: 103

```
@kai you are right. Now with VESC coming soon I will be heading down to pick up all components at once either next week or the following. 
I'm not that handy to press my own deck but your first one was already impressive. I am thinking of getting a similar shape: http://www.rayne.com/product/rival-2014/
<img src="/uploads/db1493/original/1X/716f67108768402d778919f40621821819ffa5e8.png" width="500" height="500">
```

---
## \#13 Posted by: kai Posted at: 2015-11-12T06:18:36.479Z Reads: 96

```
that looks pretty tight. i love boards with graphics on the top. a cool trick you cant do is put a layer of clear polyurethane varnish on the top and sprinkle tread tex out of a salt shaker on it while wet to the desired roughness. then a few more layers of varnish. cool trick that works ... and leaves a pretty clear finish. cheap too.
```

---
## \#14 Posted by: sgaana Posted at: 2015-12-02T05:38:27.428Z Reads: 87

```
Hi guys,
I went to my local electronic store and asked for JST-PH 2MM 4 pin and 6 pin connectors and that's what they gave to me and told me to crimp them. Am I on the right track?  
<img src="/uploads/db1493/original/2X/8/8e8ffe3e2fcff336705703b4365e78b1ddb43bb6.JPG" width="666" height="500">
```

---
## \#15 Posted by: trbt555 Posted at: 2015-12-02T06:00:36.326Z Reads: 84

```
That should work though you could have bought pre-wired ones on ebay for almost nothing and saved yourself the hassle.
```

---
## \#16 Posted by: kai Posted at: 2015-12-02T12:30:24.914Z Reads: 81

```
Looks like you have male connectors as well that you dont need. You only need the female ones because the male is on the vesc. I cant tell if those contacts are correct from the pic but it looks like. So basically you need 2 female 4 pins for canbus. You need one 6 or 7 pin for nunchuck. I probably wont use the connectors. I will crimp the contact and plug them into the vesc without the connector to test. Then i am just going to solder the contacts right to the vesc and put shrink wrap around each wire. Hmmm maybe i could get away with no solder. Sometimes the contacts dont slide in and lock to the plug. So basically, if you want to use the connectors... you need one more female 4 pin connector
```

---

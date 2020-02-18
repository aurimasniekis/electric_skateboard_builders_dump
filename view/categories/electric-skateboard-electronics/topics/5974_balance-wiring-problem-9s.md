# Balance Wiring problem (9S)

### Replies: 3 Views: 2097

## \#1 Posted by: AugustM Posted at: 2016-07-12T11:00:17.986Z Reads: 116

```
Hi guys,

I have a small problem.
I'm using a 3*3S 4.5AH LIPO pack
and a 10S 60A BMS from battery supports.

The 10S BMS is of course compatible with a 9S pack!
I contacted BS myself and they responded:
"Yes, this BMS works the same for 9S battery pack, just leave the 10th balance wire with no connection, makes the 9th wire be the final positive output then it will work, as this is a balance board and independently charge each serial connection, it has no problem for 9S pack."

So here is my wiring diagram:
<img src="/uploads/db1493/original/2X/a/ac293750d02b3a9a1389d8b54b1fe4fdd135bd02.png" width="690" height="431">

Now the problem is how to merge the 3*3S balancing wires into a 10S connector for the BMS (with one cable w/o a connection of course since it is 9S).

I'm not that into soldering, so maybe someone has an easier solution?

Thanks!!
```

---
## \#2 Posted by: AugustM Posted at: 2016-07-12T11:02:46.399Z Reads: 106

```
Oh i forgot to add the bms interface!

<img src="/uploads/db1493/original/2X/4/432260339c72d317c0a5ccfab20f31b619b1c2e3.jpg" width="690" height="363">

http://www.ebay.com/itm/36V-37V-42V-10S-60A-Lithium-ion-Li-ion-Li-Po-LiPo-Polymer-Battery-BMS-PCB-System-/221769582503?hash=item33a27f47a7#shpCntId
```

---
## \#3 Posted by: rubz Posted at: 2016-07-12T12:09:30.866Z Reads: 97

```
I made up this diagram really quick, it's not the best, but should be clear, battery negative should go to battery negative as in your BMS interface and battery positive should go straight to ESC, charger etc...
As for no soldering, you could look into screw terminals for balance wires, but they're not the safest and take up some space (but should still be okay for those small balance wires) - please do think about soldering them, they're pretty easy to solder.

<img src="/uploads/db1493/original/2X/d/d33e1431817f77051efe044b13a4a66faaffce56.jpg" width="279" height="500">
```

---

# Electric longboard Connection Diagram (review please)

### Replies: 4 Views: 737

## \#1 Posted by: voltimere Posted at: 2018-04-08T16:32:14.469Z Reads: 85

```
Hello all, 
I am pretty new to this so please understand me.

First, I want to give out my current diagram and ask for recommendation according to what i wanted to build.
Bear with my questions. I marked the picture with number that corresponds to my questions on this.

------------------------------------------------------------------------------------------------------------------------------------------
**Main items used in my project**
1) [Motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5055-280kv-brushless-outrunner-motor.html)
2)  [ESC](https://hobbyking.com/en_us/hobbywing-ezrun-max8-v3-150a-brushless-esc.html)
3) [2 x Zippy 5000 mAH battery](https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html)
4) [19 mm 12 V Latching Switch](https://www.ebay.com/itm/19mm-12V-Latching-Push-Button-Power-Switch-Stainless-Steel-Blue-LED-Waterproof/132286739133?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649)
5) [Bullet to XT60](https://www.ebay.com/itm/HXT-4mm-Bullet-to-XT60-Female-Battery-Connector-Adapter-Lipo-2PCS-Ships-from-USA/302685497504?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2060353.m2749.l2649)
6) [Lipo Charger](https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html)

------------------------------------------------------------------------------------------------------------------------------------------

![Longboard Diagram|690x291](upload://muGYM5C0U7xN3Fbh1Ho6PyNrL8N.png)



Here are the questions:

**1)** Should I re-build the T connectors into XT90 port to connect to the other modules easily? 

OR If I were to keep it and make an extra T-Connector to XT90 converter to "less damage" the item, how should I make it according this connection of the ESC?

**2)** Battery Capacity Indicator: I am thinking this is placed in the right position. Should indicate when #3 switch is turned on.

**3)** BIGGEST concern.
I plan to have two switches: One right after battery (Main ignition) and One on ESC (second ignition). First, Do I need anti-spark switch? I looked up a lot of anti-spark switches(vedder's, etc), some parts were hard to find.  

If then, what kind (value) of fuse, MOSFET, or other resistor/capacitor value do i need to use to secure this connection. I couldn't find any math calculation you can use to find these factors according to  my two 5000 mAh (in series) battery build. 

**4)** Open circuit Port created right after battery connection for easy connection to the charger. Is this okay to connect to straight like that or do I need "charging switch" to secure the port? (please consider safety and all) 
 
**EXTRA question 5)** I heard that 6S requires XT90. Using listed two 3S1P 5000mAH battery, do I need to use XT90 or can i use XT60?  

Please do correct me if I am wrong.
Please let me know guys.
Help would be greatly appreciated!
Thank you very much.
Cheers!
```

---
## \#2 Posted by: E1Allen Posted at: 2018-04-08T16:56:17.364Z Reads: 63

```
1. I would change the battery connectors to xt90.  Then make the small Y-series adapter in xt90.  So you would have one xt90 lead coming from the batteries.  
2. So long as it's after your switch it will come on and off with the board.
3. 6s voltage only makes a little pop.  All my 6s RC stuff I ran with no anti Sparks.
4. Your open circuit Port of left open will not complete the circuit.  You need it closed with a loop key.  Which could also be your anti spark connector if you choose.  Also you need take your 3s balance leads and turn it into a 6s balance lead.  Do some research on that or you will have to charge each pack individually.  
5. You can use whatever size connector you want.  However the larger connector the more amps it is rated for.  Those wires are probably much larger than xt60, I would just use xt90.

http://www.electric-skateboard.builders/t/turnigy-b6-compact-charger-not-charging-up-2x-series-lipo-3s-5800mah-batteries/38098/7?u=e1allen

![IMG_4748|281x500](upload://xgB6GvzplokVDLpovxpWWWrNZZM.PNG)
```

---
## \#3 Posted by: E1Allen Posted at: 2018-04-08T17:23:35.154Z Reads: 46

```
Also, please take the time to read as much on this forum as you can. Especially the build logs.  The search function works really well also.
```

---
## \#4 Posted by: voltimere Posted at: 2018-04-08T17:50:22.491Z Reads: 42

```
Thanks a lot!

I tried! But all the different builds confused me a lot. I wanted to make sure. 

That cleared up a lot.

Thank you!
```

---

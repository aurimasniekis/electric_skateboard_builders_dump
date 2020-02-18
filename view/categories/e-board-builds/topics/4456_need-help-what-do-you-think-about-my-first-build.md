# Need help, what do you think about my first build?

### Replies: 4 Views: 958

## \#1 Posted by: tueboard Posted at: 2016-06-09T01:46:17.063Z Reads: 99

```
hi,

i'm doing a checklist of my first eboard and i've some questions.

specs

R-SPEC Motor + Mount + wheels + torque + trucks
http://www.enertionboards.com/diy-electric-skateboard-kits/enertion-single-motor-mount-pro-kit/

deck
http://www.ebay.es/itm/pro-tec-Skate-Longboard-104x23cm-DROP-THROUGH-Tabla-Completa-Calavera-/351728659499

2x batteries
RC Turnigy 5000mAh 3S 20C Lipo Pack
http://www.ebay.es/itm/RC-Turnigy-5000mAh-3S-20C-Lipo-Pack-/231812428502?hash=item35f918f2d6:g:OTcAAOSwT~9WlfsK

controller + receptor
SODIAL Flysky FS-GT2B 2.4G 3CH
https://www.amazon.es/SODIAL-FS-GT2B-transmisor-sistema-receptor/dp/B00N71ZP1S/

balance charger
IMAX B6
http://www.ebay.es/itm/Cargador-Balanceador-IMAX-B6-de-Baterias-Li-Ion-Lipo-NiMh-Transformador-4091b-/251928655160?hash=item3aa81e3538:g:FdEAAOSwwE5WagD0

vesc
http://www.enertionboards.com/electric-skateboard-parts/vesc-standard/


can you give me some advice...

1- i find out that the batteries can have different charges plugs like JST-XH, XT90...
which is better for my specs? any of these is better to prevent sparks?

2- i read thats better to connect the batteries in series, if i get a battery with JST-XH charge plug this cable is compatible?
http://www.ebay.es/itm/262230784059?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT

3- which is the best switch on-off compatible with my vesc under $50 ? or i can avoid this part and plug in-out the batteries?

4- which cable i need to connect the motor with the vesc?

5- do you recommend this battery indicator for my specs?
http://www.ebay.es/itm/12V-Lead-acid-Lithium-LiPo-Battery-Power-Capacity-LCD-Indicator-Tester-Voltmeter-/311498010755

thank you!
```

---
## \#2 Posted by: ArmandR Posted at: 2016-06-09T01:53:42.835Z Reads: 83

```
I recommend getting just the deck, I believe you bought the complete.
```

---
## \#3 Posted by: JLabs Posted at: 2016-06-09T02:20:20.187Z Reads: 84

```
You can use an xt90s loop key as an on/off switch, they are about $10 + soldering
```

---
## \#4 Posted by: Jinra Posted at: 2016-06-09T02:40:10.983Z Reads: 82

```
>1- i find out that the batteries can have different charges plugs like JST-XH, XT90...
>which is better for my specs? any of these is better to prevent sparks?

It's going to spark no matter what header you use. You can use these for your anti spark loop. http://www.hobbyking.com/hobbyking/store/__61690__XT90_S_Anti_Spark_Connector_2pairs_bag_.html

>2- i read thats better to connect the batteries in series, if i get a battery with JST-XH charge >plug this cable is compatible?

That's a bullet connector, not JST-XH. JST-XH is normally what is used for balance charging (comes with the battery packs you listed). Your packs come with a bullet connector header so it should work. You'll want to make sure your VESC has bullet connectors as well.

>3- which is the best switch on-off compatible with my vesc under $50 ? or i can avoid this >part and plug in-out the batteries?

Building an anti-spark loop as mentioned above. See more here: http://www.electric-skateboard.builders/t/how-to-anti-spark-xt-90-loop-key/204 Otherwise you can solder on an on/off anti-spark switch.

>4- which cable i need to connect the motor with the vesc?

Just make sure the motor has the same leads as the VESC (5.5mm bullet connector)

>5- do you recommend this battery indicator for my specs?

That wont work since max voltage is 12v and you'll be running 22.2v (2 x 3s = 6s). Try this one http://www.ebay.com/itm/172143986261?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
```

---

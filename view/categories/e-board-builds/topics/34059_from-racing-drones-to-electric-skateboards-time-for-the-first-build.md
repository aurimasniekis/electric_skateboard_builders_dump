# From racing drones to electric skateboards, time for the first build

### Replies: 9 Views: 1299

## \#1 Posted by: Discogoose Posted at: 2017-09-27T07:07:16.024Z Reads: 154

```
Hey Guys,

It's time to build a esk8!  I bought a Meepo for my little brother (not here yet) and then realized I need a board too if we're going to jam around together.

I'm no stranger to building things.  I'm an electrical engineer, drone builder, equipment designer, and lover of tinkering so, I don't think I should have a huge issue with building one of these monsters.  But with all the information, good parts, bad parts, drama, and ideas out there I think it would be best for me to run my simple build past you guys!

So I want to build a portable, single motor, pulley driven esk8.  Please look over my list and let me know what you think.  Nothing is set in stone, and if you have better options then what I have below please let me know.  I am located in San Diego, CA, USA so I would like to source as many parts in the US as possible.  I want to do this right!

**Mechanical**
Board - TBD, would prefer the smallest form factor that can fit the equipment below.
Trucks -  [Caliber II](https://www.amazon.com/gp/product/B072J845HD/ref=ox_sc_act_title_2?smid=AQ5JN7IFU4T3S&psc=1)
Wheels - [Orangatan Kegels](https://www.amazon.com/gp/product/B074XGYP4S/ref=ox_sc_act_title_1?smid=A2YR3NFJ41VU11&psc=1)
Motor Mount - [Mount!](http://www.electric-skateboard.builders/t/boardnamics-cnc-motor-mount-w-idler-tensioner/31015)
Pulley Kit - [15mm, 36T, 15T](http://www.electric-skateboard.builders/t/15mm-wide-pulley-kits-and-individual-parts-wheel-pulley-motor-pulley-belts-and-hardware/27184)

**Electrical**
VESC - FOCBox
Motor - [6354 208kv Motor](https://buildkitboards.com/collections/motors/products/6354-208kv-motor)
Battery - [Namasaki Battery](http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014) 5x 2S 60C LiPo, still figuring this out
BMS - [BesTech BMS](http://bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html), need to find a source for this. Really don't want to have to buy 2 from the vendor
Controller - TBD, not sure what to get.  I really want to make sure it's safe.
Misc. - switches and whatnot depending on the components I pick

So what do you guys think?  Are there better options I should be looking at?

Thanks for the help!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-27T11:37:17.464Z Reads: 119

```
The pulley kit you listed as far as I know will only fit flywheel style wheels.
There are other options for kegels 

- you need to get these printed 
http://www.electric-skateboard.builders/t/oranatang-kegel-32-34-36-38-40-42-44-tooth-pulleys-stls-for-9mm-12mm-15mm-belts/7227

-  www.unikboards.com also sells kegel pulleys. They are 32t. He ships fast from Paris.

- another good choice for pulley and also a mini remote.

https://buildkitboards.com/collections/remotes
https://buildkitboards.com/collections/parts/products/36t-orangatang-kegel-pulley?variant=32845454597

- This might help with the BMS.
http://www.electric-skateboard.builders/t/group-buy-bestech-bms/34028

- You can also try the new maytech remote
https://psychotiller.com/products/shop/remote-controller
 
Good luck.
```

---
## \#3 Posted by: i2oadsweepei2 Posted at: 2017-09-27T12:35:10.259Z Reads: 96

```
Also if you don't have your focbox yet. These were just restocked in Cali.

http://www.electric-skateboard.builders/t/new-focbox-for-sale-us-free-shipping-price-reduction/19089
```

---
## \#4 Posted by: NickTheDude Posted at: 2017-09-27T12:44:43.422Z Reads: 87

```
Other than the stuff mentioned above it looks good! For your remote you might want to look at the nano v2. Make sure its the second version since the first had issues with dropouts.

Another great option is a GT2-B with a case mod. I've got a mastercho mod and it's fantastic.
```

---
## \#5 Posted by: i2oadsweepei2 Posted at: 2017-09-27T13:32:38.548Z Reads: 77

```
I can also vouch for the gt2b and the mastercho mod. It's been perfect for over a year.
```

---
## \#6 Posted by: JdogAwesome Posted at: 2017-09-27T16:29:42.981Z Reads: 67

```
Also if your planning on running 10S1P you can get BMS a lot cheaper on AliExpress and just bypass the over current protection. Also 60C LiPos are not necessary for this use case I think 25C is fine and it's what I use in my board. Also how are you planning on turning your board on and off? XT90 loop key or a MOSFET switch?
```

---
## \#7 Posted by: Discogoose Posted at: 2017-09-27T19:51:44.122Z Reads: 60

```
@i2oadsweepei2 , thanks for all the good information and links! I will check that out today and hopefully start ordering some parts!

 @JdogAwesome , I was initially looking that the BMS's you are talking about but the BesTech just seems like higher quality and it has the e-switch built in so that I won't need an antispark switch. At least that's what I've read. Please correct me if I'm wrong. 

Now to start checking out cool board designs. Any recommendations would be great!

Thanks again for all the help!
```

---
## \#8 Posted by: John_Doe Posted at: 2017-09-28T20:58:43.348Z Reads: 38

```
If your buying the BMS I want to buy one as well, though i need a 12S, maybe we can get them to shift the MOQ over to 2 different models if your willing to buy one with me?
```

---
## \#9 Posted by: Discogoose Posted at: 2017-10-02T17:43:01.747Z Reads: 22

```
Hey guys,

The parts are slowly trickling in. The only part I haven't purchased and was hoping for some feedback on was the battery/BMS/enclosure. Initially I was thinking about 5x 2s 5000mah lipos with a BesTech BMS. 

After searching around I bit I saw this: http://www.diyeboard.com/10s5p-11ah-lg-battery-power-kit-with-bmschargerenclosure-p-572.html

Any thoughts on this all in one solution? This is battery/BMS/enclosure. It also has room for my FOCBOX and receiver probably (or I can make room). 

I am somewhat unfamiliar with the this battery technology and just want to know if I'm shooting myself in the foot here. 

Any help would be greatly appreciated. 

Thanks,
Cory
```

---

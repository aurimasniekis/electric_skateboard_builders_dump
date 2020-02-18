# JayKay e-truck statement

### Replies: 41 Views: 4198

## \#1 Posted by: JayKay Posted at: 2017-06-19T15:01:36.409Z Reads: 476

```
**Hi guys,**
**we have just read your discussions about our e-truck and that there is maybe a lack of information. Thus we will give you more details about the technic.**
 
We know that the whole truck indicators sounds too crazy, so it is difficult for us to demonstrate the benefits.
We try to explain the whole truck with calculation examples and support it with videos - if our truck is back from an exhibition in Berlin.
 
 
**First about the batteries:**
Fundamentally the energy and the power of a cell goes opposite.
So for range we need energy, and for acceleration we need current. To combine range and acceleration (especially needed at the drive up) in one cell, we develop a serial / parallel switch to have 2S2P for high torque and acceleration at low speed and 4S1P for high speed.
Four batteries are integrated in each hanger of the truck. So we have in two trucks 8 cells in sum. We use the new industrial cell size 2170(0) to get almost the latest and best cells for the truck.
At the beginning we tested our trucks with the LG HG2 (18650, 20A continuous, 3 Ah) and had very good results regarding acceleration and good regarding range. Now we test the Panasonic NCR20700B (2070(0), 15A continuous, 4,25 Ah), cause the focus is to increase the range.
With this cell we generate a conservative calculated capacity of 100 Wh with a moderate cycle life.
At this point we haven't consider the new 2170(0) cells, which will be available very soon.
 
 
**EMC**
The cells are directly mounted on our PCB inside the truck. So we have a very short distance between cells, EMC and Motor and have only one plug between the PCB and the motorphases. So the wire losses are minimal. We use a four layer PCB with 70 µm cooper, so there is for every single motorphase a own PCB layer with lowest resistance. We tested the PCB successful with 30 Amps (temp rise at 20 A is about 7° C). We have at both ends our motormosfets with a low RDSon of 1 mOhm and a QGD of 13,5 nC for highest efficient.
We have never made a compromise between cost and quality, we almost take the best for the best result (OK, no silverwinding ;))
The PCB includes:
- for each motor a mosfet circuit with driver, a back emf measurement, current measurement and capacitor bank
- a balancer circuit for each cell with voltage measurement and total current measurement
- a cell switch 2S2P <-> 4S1P, to have till about half of speed high torque or if the torque is not required a quarter of the cell losses.
example, 10 km/h and 10A for each motor, 20 mOhm cell resistance
4S1P:
(20 A)² x 4 x 20 mOhm = 32 W cell loss
2S2P
2 x (10 A)² x 2 x 20 mOhm = 8 W cell loss
so the controller switches if possible in 2S2P to reduce internal losses.
- an automatic on/off switch with self holding (using the voltage from a rotating motor to switch the circuit on at about 2-3 km/h)
- a DC powerline communication, to communicate and power the PCB in the baseplate with only one power pogopin (mass connection goes through the housing like in a car) so you can mount the hanger in the baseplate without plug a cable.
- a high-performance, low-power 32-bit controller with 50 MHz to manage all the tasks
- and other stuff like voltage regulators and temperature measurement.
All parts are under 1 mm height and so the total PCB height with parts is max. 1,8 mm.
 
 
**Motor**
We use an ironless permanently excited synchronous machine.
This kind of motor has following benefits:
- no cogging and very less eddy currents, cause of the less iron in the stator and the thin lamination.
                We want to use the e-truck like a normal truck, so we don't want to use electric energy for freewheeling. This is the only permanently excited synchronous machine who can do this. Other possible motors for freewheeling are without magnets, like reluctant- or asynchron. But these types are heavier at the same power and have no ideal powercurve for our application.
- best ratio of weight to torque (in hub configuration without gearbox) cause of the less iron which is needed to close the magnetic circuit.
- high efficiency, in our manufacturing process we press the cooper winding with high pressure on the stator and get a coil resistance of 50 mOhm of each phase!
In one motor we generate a torque of 0,06 Nm / A.
The three motorphases would be automatic connected by putting the stator on the truck, so you haven't connect the motor with a cable.
 
In sum we get a very high system efficiency, which generates less heat and more range!
 
 
**PCB Baseplate**
In the baseplate we include a second PCB. This small PCB includes the following features:
- powerline communication with the hanger PCB, cause the hanger PCB is inside a faraday cage and can't send via bluetooth.
- communication via Bluetooth with the second truck, the remote and possible with a smartphone or -watch
- handle the USB PD protocol to unlock the PD charger. We can charge the e-truck with profile 4 and 5, this means 3 A @ 20 V or 5 A @ 20 V (look for further Information at USB Power Delivery)
- Charge inductively the e-truck. We integrated in the cover a primary Qi coil. With this coil the board could be charged inductive. The holder is under development, but other tasks have actual higher priority.
- As gadget you can charge your qi-able phone if the truck is drop through mounted, otherwise you can charge via the type C connector. Both connections are limited with 5 V @ 1 A. We see this connection as a emergency charge station, to take a call.
- NFC chip for fast Smartphone connection and fast Truck profiling
 
 
**Truck housing**
The truck itself is made of a high quality aluminum alloying, which is normally used in automotive axis. Unsuccessful we tried to break it with a 2 t car jack.
The truck is housing and cools the rest of the motor and electronics.
```

---
## \#2 Posted by: anorak234 Posted at: 2017-06-19T17:29:54.669Z Reads: 425

```
Wonderful explanation - although to be perfectly honest I believe both 2s2p and 4s1p even in a 4wd setup is much too weak to impress anyone on this forum (we are used to 6-12s and 3-8p). What I do find impressive (and I'm sure others can agree) is that you have taken the initiative to respond to each and every one of our criticisms in clear detail, and I think that this shows extremely good communication and reliability on the part of your company. Good luck to you, and I wish you the success that you hope for your product to achieve.
```

---
## \#3 Posted by: Maxid Posted at: 2017-06-19T17:56:19.539Z Reads: 417

```
Actually I am fascinated by how much electronics you apparently put into such a tiny footprint. My Antispark alone is apparently larger than your whole electronics setup :confused: 

If it works: Good job!
```

---
## \#4 Posted by: Print3r Posted at: 2017-06-19T18:21:19.060Z Reads: 400

```
Can you explain where I went wrong - 4.25Ah*3.7V*4=62.9Wh no? Secondly 
> We can charge the e-truck with profile 4 and 5, this means 3 A @ 20 V or 5 A @ 20 V

 4*4.2=16.8V   or 2*4.2=8.4V  .... how does the 20V charging work - do you have a step-down voltage divider?

Many thanks for the explanation on the other details - if this works it clearly shows you have succesfully, completely rethought eboarding!
```

---
## \#5 Posted by: Hummie Posted at: 2017-06-19T19:20:14.573Z Reads: 377

```
How do u stop?

Can u do a video of going up a hill and of the inside of the truck.  I'd like to see how you fit 2 of those large cells and the esc inside.
```

---
## \#6 Posted by: JayKay Posted at: 2017-06-19T19:54:20.035Z Reads: 368

```
Hello Print3r,

4,25 Ah x 3,6 V x 4 cells = 61,2 Wh per e-truck. Means 122,4 Wh with both e-trucks as maximum.
In this case we "only" use 80 % of the cell capacity, about 100 Wh, to guarantee the 12 km range and maximize the cycle life of the cells.

When we charge the e-truck via USB, the cells are switched in 4S1P, so the maximum cell voltage is 4,2 V x 4 = 16,8 V. For this we have on the PCB in the hanger a step down converter. 

i will load up a picture of the PCB and explain the components
```

---
## \#7 Posted by: Print3r Posted at: 2017-06-19T19:59:14.098Z Reads: 354

```
Is 20V 5A over usb safe! Thanks for the prompt reply.
```

---
## \#8 Posted by: JayKay Posted at: 2017-06-19T20:31:04.096Z Reads: 353

```
Hello Hummie,

1. you can brake like a non electric board
2. you can recuperate and push energy back to the cells. The energy from the motors go through the charging circuit to regulate it. Limited is this "brake" force by the maximum charge current of the cells and the cell state. If the required "brake" force is higher, we burn the current in the motorcoil till the temperature is too high. This goes very fast (depending on brakeforce) and then there is no more possibility to break. We thought about a brake resistor, which is cast in the aluminum hanger, but this would only put off the problematic to handle the heat.

Fundamentally a "brake" via a recuperate isn't a real break cause it depend on cell voltage and the system temperature.
A brake have a defined brake torque and work in every case, so we do not brake, we decelerate if possible.

So the driver of a electric board without a brake should be able to brake by himself.

We fit four cells with electronic in each truck.

Tomorrow I open for you the accupack to show you who it fits. Cause our board is exposed I send a uphill video as soon as possible.
```

---
## \#9 Posted by: Hummie Posted at: 2017-06-19T20:41:13.728Z Reads: 339

```
i don't understand as you say the motor will start to be powered if it is moved by pushing right?  and then once you're moving it will continue to move until you brake as done with a non-electric board, which I guess means put your foot down and drag it, but I must be missing something as how is the motor to know if it's an uphill resistance or the rider putting their foot down?
```

---
## \#10 Posted by: JayKay Posted at: 2017-06-19T21:05:30.316Z Reads: 347

```
[quote="Print3r, post:7, topic:25698, full:true"]
Is 20V 5A over usb safe! Thanks for the prompt reply.
[/quote]

With the USB Power Delivery it is,
There is a controller in the device and one in the power adapter. The device sends a request what it need for a profile (means voltage and current) and the power adapter send a answer message with his possible profiles. So they handle out and start charge if they match. For profile 5 (meanse 5 A) the active cable must be detected and these cabels are build for 5 Amps. So you can charge a Smartphone, which needs 5 V or a notebook which needs 20 V with the same adapter without destroing one of the devices.
```

---
## \#11 Posted by: JayKay Posted at: 2017-06-19T21:18:05.657Z Reads: 331

```
Sorry, I misunderstood.
You control the board with a remote.
The remote has three basic functions: accelerate, decelerate and freewheel.
You push once the board, then only the electronic circuit switch on. Now you can accelerate with the remote or push further like a non electric board.
If you want to stop you decelerate till you stop or you choose freewheel and brake by foot.
```

---
## \#12 Posted by: Tuomalar Posted at: 2017-06-19T21:34:00.022Z Reads: 329

```
Sooo this board is more like longboard with assistant motors. Not for bashing around streets with raw electric power.
```

---
## \#13 Posted by: JayKay Posted at: 2017-06-20T09:07:04.329Z Reads: 344

```
This drive is comparable with other drives in the 100 Wh class.
You can push the board and assist if you don't want to push at long distances or uphill. Futher you can drive pure electric. It's like a hybrid with foot and electric. For bashing around the streets with raw power, the capacity is to low like other drives in this class. It's perfect for cruising through the city or on the sea promenade.
```

---
## \#14 Posted by: JayKay Posted at: 2017-06-20T09:16:14.992Z Reads: 345

```
<img src="/uploads/db1493/original/3X/7/8/784c010ddcb136037dafac04d0fd43440da4175c.jpg" width="666" height="500">

This is the PCB with the LG cells. The red wire is only for us to debug and load software.
```

---
## \#15 Posted by: TarzanHBK Posted at: 2017-06-20T09:41:59.348Z Reads: 340

```
That´s awesome how much you packed in there :D
```

---
## \#16 Posted by: Pedrodemio Posted at: 2017-06-20T11:46:00.975Z Reads: 333

```
Nice work, as I understand two of the cells goes inside the motor? The larger diameter section of the hanger is where the motor goes? What about heat on these cells? Lithium degrade faster at higher temperatures, and a hub motor will be severely limited if you have to keep the current down to prevent cell overheat, not saying it doesn't work, I just want to hear what was the thinking behind this setup 

Thanks
```

---
## \#17 Posted by: JayKay Posted at: 2017-06-20T20:29:16.184Z Reads: 322

```
Hello Pedrodemio,
yes, the both outer cells are inside the motor. We know from the beginning that we had a challenge to handle the heat, cause our electronic and the motors are directly mounted near the cells. Because we want anyway range and no heat, we spend a lot of time to develop a high efficient setup.
So we designed the PCB circuits so, that the power loss are low as possible.
We use four motors, so there is half of the current compared with a 2WD and so we have a quarter of the losses per motor.
We designed the Motor that we could implement a winding with only 100 mOhm. For this we press under high pressure a litz wire (although to minimize eddy currents) on the stator and use in the rotor  N52 Neodym magnets for a strong magnetic field. At nominal voltage the back inductance of the motor limit the maximal speed at 35 km/h. So you see the magnetic flux can't be higher!
Cause of the less stator iron this motor type have much lower impedance compared with other synchron motors.
Additionally we use between the stator iron and the aluminium hanger an aluminium spacer, to lead the heat to the complete hanger.
So we don't create heat hotspots in the coil like other hub motors.
Cause of the thermal conductance of aluminium the heat spreads, so the temperature between the inner and outer cells are only a few degree Celsius.

The result is, that we have at our last test ride a hanger temperature at about 40° C. It feels only warm.

At the promised uphill test ride, I take pictures for you with a thermal camera.
```

---
## \#18 Posted by: Hummie Posted at: 2017-06-24T03:09:36.579Z Reads: 295

```
Thank you for telling us as before you seemed possibly unbelievable.  how much iron is there and why not use more?
```

---
## \#19 Posted by: JayKay Posted at: 2017-06-24T15:33:49.658Z Reads: 296

```
Hi Hummie,

We use only the iron that there is no saturation of the flux.
Or do you mean why this motor type need a lower quantity of iron?

If we use more iron, there would be a slightly higher flux and a noticeable heavier engine.
Although the motor would slightly increase the torque and degrees the speed.

If you design a motor, there are many parameters to adjust.
If you change a parameter on the one side, there is a change on some other sides.
So we give the parameters priorities regarding the engine requirements.
```

---
## \#20 Posted by: Hummie Posted at: 2017-06-24T17:01:04.992Z Reads: 295

```
I'd think for a hub motor especially you'd want a high magnetic flux that would come from iron at the expense of weight.  Is there any iron in the motor on the stator or rotor side?  I'd think you could do a hallbach array on the rotor and avoid any need for iron but the stator side it seems unavoidable if you have so slow a motor with no gearing to have torque. 
Can u show pics of the motor?  And how it attaches?
```

---
## \#21 Posted by: JayKay Posted at: 2017-06-26T09:33:40.587Z Reads: 296

```
Hi Hummie,
The iron is need to lead the magnetic flux. In our setup there are no stator teeth, so it is less iron to close the magnetic flux.

<img src="/uploads/db1493/original/3X/8/5/85f6c5ef943a34d929d6b8231203faa289e678fa.JPG" width="539" height="500">

Outside pure iron, inside iron lamination.

<img src="/uploads/db1493/original/3X/5/4/54d911291ef00fb3486bf260e13cff0aceba0f3c.JPG" width="690" height="339">

This is the flux density over one magnet, its an average of 0,76 Tesla.
```

---
## \#22 Posted by: JayKay Posted at: 2017-07-11T07:44:36.907Z Reads: 282

```
<img src="/uploads/db1493/original/3X/a/0/a02504333cbdb0c0c4b876792ce9006f111734ec.jpg" width="666" height="500">

This is the thermal view of the truck at max. penetrating and ambient temp of 26° C
Drive tests will follow on our social media channels with our new model which is in build.
```

---
## \#23 Posted by: anorak234 Posted at: 2017-07-11T14:19:05.820Z Reads: 278

```
The maximum safe recommended charging temperature for lithium cells is 45 Celsius, and I would charge closer to 25 to maximise cell life. You may want to find a way to drop that a few degrees or warn customers to wait for the unit to cool down after use. Also it may not look the coolest, but you could probably integrate a slight heatsink into the metal of the trucks if you tried

http://batteryuniversity.com/learn/article/charging_at_high_and_low_temperatures
```

---
## \#24 Posted by: JayKay Posted at: 2017-07-12T06:26:08.759Z Reads: 266

```
Hello anorak234,
this temperature is in the discharge range from -20° C to 60° C. The charge temperature range is like you said from 0° C to 45° C. At all time the temperature is measured by the controller, and the controller throttles the current if the temp go's to the limit. So if you charge the truck with the temp above, the system waits till the temp is in a non critical range. To degree the heat (the whole hanger is an aluminium heatsink) we could increase the surface of the hanger. 
Overall, for max. penetrating (this is quite not the normal case) it's a very acceptable value.
```

---
## \#25 Posted by: FredSaberhagen Posted at: 2017-07-13T15:20:56.841Z Reads: 252

```
That's the outside of the truck meaning the inside is way hotter
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-07-13T16:10:19.381Z Reads: 249

```
Florida heat is also very unfriendly to motors which is one reason i use large well ventilated ones that aren't sealed. 

@JayKay Wow. Just... wow. This is very impressive.  

When can i get a drive system to test?
```

---
## \#28 Posted by: Achmed20 Posted at: 2017-07-13T18:10:57.872Z Reads: 253

```
ok i just backed it!
if anyone here has some serious interest in these you should probably do this as well because they just have 13hours left and are still missing 46% ;)
```

---
## \#29 Posted by: JayKay Posted at: 2017-07-19T07:45:35.482Z Reads: 238

```
We are searching for distributors in dfferent countries who offers test rides. 

But you can also buy one, test it and if you are not happy with it you can send it back within 2 weeks. Of cause without big traces of usage. 

Very likely available from December 2017.
```

---
## \#31 Posted by: FilipBastien Posted at: 2017-09-21T23:36:52.964Z Reads: 207

```
Do you use thermal paste to help cool the components like in a computer? and do you think its possible to integrate small batteries inside a deck and keep it flexy?

BTW im loving this project, very impressive feat of engineering and well thought through from what I see :+1:
```

---
## \#32 Posted by: Idle Posted at: 2017-11-30T19:12:28.540Z Reads: 195

```
@JayKay can you post some video of this wizardry?
```

---
## \#33 Posted by: evoheyax Posted at: 2017-11-30T19:28:13.841Z Reads: 194

```
Crazy cool. This will be the most normal looking e-skate ever built. However, it annoys the crap out of me when I hear the words high torque and high speed followed by 2s2p or 4s1p in the same sentence. Only thing it will do is confuse people who don't know anything about e-skate electronics. What is the target weight for these in your mind? Even a lighter guy will struggle to move with such a low voltage. Has to be what, 5 amps at 8.4 volts per motor? That's only 42 watts per motor, for 168 watts total. Almost everything on the market is at least 300 watts, and those are very weak systems already. 1000-2000 watts is standard torque, high torque is 2000-4000 watts. Then theres very high torque at 4000+ watts. So this is very low torque at best.

Not trying to pull you down or anything, it's just misleading to say high torque with 168 watts...
```

---
## \#34 Posted by: Pedrodemio Posted at: 2017-11-30T20:06:28.319Z Reads: 187

```
Since they are using 21700 they could be using the Samsung 30T, 30A without much problem, even more for short bursts, this brings everything to almost 900W with both trucks, even an Panasonic 21700B could provide 15A with a decent capacity
```

---
## \#35 Posted by: pat.speed Posted at: 2017-11-30T20:10:29.199Z Reads: 186

```
[quote="JayKay, post:1, topic:25698"]
Now we test the Panasonic NCR20700B (2070(0), 15A continuous, 4,25 Ah), cause the focus is to increase the range.
[/quote]

I think they are using the NCR20700b
```

---
## \#36 Posted by: evoheyax Posted at: 2017-11-30T20:24:40.572Z Reads: 185

```
regardless, the issue will be heat in the esc. As it is right now, even the vesc 4.12 can only do 25 amp continuous. Those fets are tiny on that esc, no way it can do more than 5 amps con, if even that...
```

---
## \#37 Posted by: Pedrodemio Posted at: 2017-11-30T22:28:00.584Z Reads: 177

```
I really don't know, once you go down on voltage rating on the MOSFET's, the rdson also go lower, so probably they produce less heat for a given current than the 4.12, but i agree that heat has to be managed
```

---
## \#38 Posted by: evoheyax Posted at: 2017-11-30T22:41:30.120Z Reads: 182

```
The other issue is going to be sag. You'll sag down from 4.2 to 3.4 at 15 amps with those cells. That means 6.8 x 15 = 102 watts per motor x 4 = 408 watts total. Range will be like like, 15 city blocks before your sagging below the low voltage cutoff at 15 amps at best, probably more like 5. Again, assuming 15 amps is even possible.

Again, not trying to tear this project apart, just giving my analysis of the concept. I'd still love to see it done. Maybe you can prove me wrong?

Either way, it's clearly misleading to say high torque or high speed. The Carvon EXO uses the koolwheel motors, so it's limited to 700 watts total. At that even the acceleration when I tested it at the SPD2 was very weak for my taste (not trying to hate on carvon, just trying to compare watts with what I've ridden before).
```

---
## \#39 Posted by: Exiledd_Top Posted at: 2017-12-01T03:41:11.006Z Reads: 164

```
Am assuming u meant carvon EXO  not carvon EVO the evo is 5000watts total in dual and EXO is 300 watt per motor carvon doesn't use koowheel motors for Evo just EXO btw it's like koowheel motors but Jerry design on it
```

---
## \#40 Posted by: evoheyax Posted at: 2017-12-01T06:46:44.984Z Reads: 156

```
Yes, my mistake. Thank you. The little he talked to me at SPD2, he told me they are koowheel motors moved out of the hub and on a carvon designed mounting system. Probably redid the can and magnets.
```

---
## \#41 Posted by: JayKay Posted at: 2017-12-01T10:50:12.337Z Reads: 149

```
Hello evoheyax,

Thank you for your comment.
We fundamentaly have to difference between power, meassured in W and tourque, meassured in Nm.
The tourque at the same power depends only on the max. speed! And a low system voltage requires a higher current for the same power, which you can splitt to four motors. In our first statemaent we tried to explain the system, couse you can't look to one parameter and appraise the system.
Over all we see there is much discussion about our e-truck, work or work not... however at the moment we produce our serie and then you have to feel the e-truck.
Driving, not talking :wink:
```

---
## \#42 Posted by: JayKay Posted at: 2017-12-01T10:53:31.455Z Reads: 144

```
There are some new interresting cells on the market which we are testing at the moment.
```

---
## \#43 Posted by: pat.speed Posted at: 2017-12-01T12:05:13.276Z Reads: 134

```
I think the 30t would be ideal for this
```

---

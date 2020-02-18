# Electronic setup help!

### Replies: 9 Views: 708

## \#1 Posted by: DarkJoker Posted at: 2017-09-05T21:42:03.742Z Reads: 64

```
This is my 1st build and i have everything i pretty much want for my build and the parts i have picked are for certain specs but im not really sure how to connect everything together. 
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html
4x Lipo batteries: https://hobbyking.com/en_us/turnigy-battery-nano-tech-3000mah-2s-25-50c-lipo-pack-xt-60.html (in series and parallel)
 Remote: http://alienpowersystem.com/shop/radio-transmitters/alien-power-system-2-4ghz-electric-skateboard-remote-control/
Vesc: http://alienpowersystem.com/shop/esc/ev-esc/vesc/

i know there are more parts that are required to complete the build like the board trucks and wheels but my main concern in how to connect each individual part together in order to get everything to work. 

Diagrams would be helpful
```

---
## \#2 Posted by: Yecrtz Posted at: 2017-09-05T21:51:10.736Z Reads: 62

```
I'm not sure which connectors the VESC you are buying comes with. But you know which connectors the batteries and motors have.

The batteries have XT60 for discharge, so you'll need two [xt60 series cables](https://hobbyking.com/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/1/0/10264.jpg) and one [parallel XT60 cable](https://hobbyking.com/media/catalog/product/cache/1/image/9df78eab33525d08d6e5fb8d27136e95/1/0/10265.jpg) to hook up the batteries. Next is the VESC, you probably need to solder on your own connector, so I suggest you buy some XT60 connectors and put one on the vesc. Tip, put an antispark switch between the XT60 coming from the batteries and the vesc. 

Then, your motor has 4mm bullet connectors, so you'll need to put those onto the 3 wires that are coming from the vesc in order to connect it. Doesn't matter which one goes where, if the motor spins in the wrong direction, switch two of them. The remote receiver simply plugs into the vesc.
```

---
## \#3 Posted by: DarkJoker Posted at: 2017-09-05T21:54:03.632Z Reads: 53

```
I dont think my dorm room would be a fan of me using a solder in my room, do you know of an alternate to bypass any soldering needed?
```

---
## \#4 Posted by: Yecrtz Posted at: 2017-09-05T21:57:11.836Z Reads: 47

```
Nope, it seems  the VESC doesn't come with connectors so you'll have to solder them on.
```

---
## \#5 Posted by: DarkJoker Posted at: 2017-09-05T22:01:25.062Z Reads: 47

```
do you know of a different vesc that comes with connectors so i wouldn't need to solder?
```

---
## \#6 Posted by: Yecrtz Posted at: 2017-09-05T22:07:54.081Z Reads: 42

```
I'm not aware of any VESC that comes with 4mm bullets for the motors. So you'll need to solder them anyway. Maybe you can contact the seller and ask if they can solder them on for you.

Here do you have a diagram, I added an antispark/on-off switch. 
<img src="/uploads/db1493/original/3X/7/3/739c242256cb878c2e4114e2268e9c78e12fefa9.png" width="480" height="500">
```

---
## \#7 Posted by: DarkJoker Posted at: 2017-09-05T22:14:41.191Z Reads: 36

```
would you know if this [VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/) would work? and i found batteries that have xt90 connectors so i know that the VESC I said in this reply would be able to connect to the batteries. With this diagram the batteries would look like 12000 mah 8s4p right?
```

---
## \#8 Posted by: Yecrtz Posted at: 2017-09-05T22:20:52.467Z Reads: 35

```
That vesc is fine. But DIY's comes with 5.5mm bullet connectors.. Doesn't match the 4mm from your motor. Also with your original 4 batteries in series and parallel, you'll have a 4s2p and only 6000mah.

If you take four 5s 5000mah batteries and configure them in the same way you'll have a 10s2p with 10ah. I would not go with less than 8s. Google series and parallel explained and you'll find some usefull info regarding the different kind of options.
```

---
## \#9 Posted by: DarkJoker Posted at: 2017-09-06T00:22:12.667Z Reads: 33

```
<img src="/uploads/db1493/original/3X/5/f/5f59744eede808cbab10448ef8536c3f230c4b4b.png" width="524" height="500">

Would this work? as 10s2p at 8000mah parallel?
the[ battery](https://hobbyking.com/en_us/zippy-compact-4000mah-10s-25c-lipo-pack.html)
[connectors](https://hobbyking.com/en_us/hxt-4mm-bullet-to-xt90-battery-adapter-2pcs.html) 4mm to xt90
[parallel](https://hobbyking.com/en_us/xt90-battery-harness-10awg-for-2-packs-in-parallel.html) cord
[anti spark](https://hobbyking.com/en_us/xt90-s-anti-spark-connector-2pairs-bag.html?countrycode=US&gclid=CjwKCAjwlrnNBRBMEiwApKU4PAMdYmzXvcojdTVzqI33ycKX_Y6ZbiTnPSQuoHdD2dPpmykYa16YyxoCsmUQAvD_BwE&gclsrc=aw.ds)
```

---

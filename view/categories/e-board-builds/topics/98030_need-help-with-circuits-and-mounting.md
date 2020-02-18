# Need help with Circuits and Mounting

### Replies: 5 Views: 109

## \#1 Posted by: Peteymy Posted at: 2019-07-07T23:43:05.660Z Reads: 32

```
Alright, this is going to be a long post. Thanks for reading and helping!

Background: So, I've ordered all my parts and received most of them and have run into some complications to exactly how I'm going to deal with everything that goes under the board. All will be discussed later in this post.

Battery: https://www.banggood.com/ZOP-Power-22_2V-8000MAH-30C-6S-Lipo-Battery-XT60-Plug-For-RC-Quadcopter-FPV-p-990752.html?cur_warehouse=CN

Charger - https://www.aliexpress.com/item/32966624241.html?spm=a2g0o.cart.cb0001.1.703d3c00NfQHb4&scm=1007.13440.95620.0&pvid=cc068508-8089-4fb9-a3eb-6ad46cdb3604&tpp=1

ESC- https://www.ebay.com/itm/single-motor-electric-longboard-skateboard-controller-ESC-Substitute/302546263597?_trkparms=aid%3D111001%26algo%3DREC.SEED%26ao%3D1%26asc%3D20160908105057%26meid%3Dc93d1f95bfd342d8bc7d2a7709d407bc%26pid%3D100675%26rk%3D3%26rkt%3D15%26mehot%3Dpp%26sd%3D291966653914%26itm%3D302546263597&_trksid=p2481888.c100675.m4236&_trkparms=pageci%3A85fc3e2e-a110-11e9-b381-74dbd180c234%7Cparentrq%3Acecee93516b0abc66084f6ffffe1f8d9%7Ciid%3A1

Circuit - 
So what I originally thought I wanted to do was to make a hinge on the "top" of my mount so it would be easy to reach my battery to unplug it and charge it when needed, possibly 5 or so days a week. I decided that having two pieces to the enclosure would not be the best idea, and it would just look cooler to have it one piece as well as the enclosure being stronger. 
My new idea is to try to include a DPDT (if that is the wrong type to do what I want, please correct me) switch so I don't have to deal with removing the battery. I was just wondering if this circuit would work for my purpose, essentially wanting to be able to easily switch between the battery connection from the ESC to the charger port. 
![image|690x388](upload://aLKZrQxkEibghelvQuudxhzkNUO.png) 

Battery Monitor - 
So, I know there is a low to what you should discharge LiPo cells to (3.5 or so if I'm not mistaken). The thing is that the ESC I bought didn't come with a monitor that lists off the voltage of cells, but one that has a 4-level monitor as seen in the "background" section. I'm just wondering if this is a direct monitor or if it would be tuned so it hits "zero" each cell would be around 3.5 volts. I'm not sure how the monitor works, so I don't really have a way to test it other than run the cells down to that voltage, which I'm not sure I wont to do. 

Mounting - 
My next question is how the hell to mount my enclosure to the board. Of course, I'm mounting all my electronics and stuff to the board, but since I'm planning to 3D print (I'm using PLA+ with 4mm walls and a sealant, so I think it should be strong enough) I'm not sure exactly how to mount it to the board. I don't really want to drill all the way through the board since it would look sorta gross having screws pointing through the board at what would appear random points. I was wondering how I would mount the 3D print with something that wouldn't crack the plastic and would be able to hold without going all the way through the board. I searched through different threads but didn't understand them too much.

Thank you in advance for all the help you can provide, this is my first board and I'm excited to see it working!
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-07-08T02:15:37.643Z Reads: 23

```
I'm confused as to why you want to switch between your ESC and charger, and not just have both the charge port and the ESC connected at the same time? A DPDT switch capable of handling the full discharge current will be bulky and expensive.

For monitoring, you can get meters like [This](https://usa.banggood.com/Geekcreit-0_28-Inch-2_5V-30V-Mini-Digital-Volt-Meter-Voltage-Tester-Two-Line-Voltmeter-p-974258.html) and just remember what your minimum safe voltage is, or you can get ones with an actual capacity estimate built in.

As for mounting, the way I did it was to use threaded inserts in the board, with machine screws (M4) screwed into those. With some care and the correct inserts, you should be able to do it without any holes coming through the top side.
```

---
## \#3 Posted by: Peteymy Posted at: 2019-07-08T02:33:28.556Z Reads: 22

```
I was thinking of using a y connector between the ESC and battery. That way I could connect the charger to the extra port, and charge it. The problems I thought this would bring was that while I was charging the battery, wouldn't there be voltage running to the ESC? It seems like it might damage it. Also, it could short if water got to the outside connector, but I could just put a closing clip in it.

About the monitor, I knew I could just get something that would show me the voltage, but that would require extra testing to find the minimal voltage, along with waiting for that part to arrive, so I would prefer to stick with what I have.
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-07-08T03:39:12.484Z Reads: 15

```
You would put a loop key or other switch between the battery and ESC, or if the ESC has switching capability itself it doesn't matter if you charge while it's connected - it'd be seeing battery voltage already, a couple extra volts while charging is nothing.

A water resistant connector is a good idea regardless.

You don't need any testing, just basic math - 3.5v, times the number of cells in your pack, equals the voltage you should stop at.

Plus, you can get those meters from like Amazon with two-day shipping. Totally worth it.
```

---
## \#5 Posted by: Peteymy Posted at: 2019-07-08T04:18:28.377Z Reads: 15

```
So would you advise making just one port outside, which connects to the charger, or put all three connectors outside and just choose which one is active by connecting the loop key to each one when I need to charge/run? 
My ESC does have a button to turn it on and off, so I might just to the Y-connector thing, but would there be a problem caused if I were charging and the ESC got turned on somehow?

Thank you for all the help.
```

---

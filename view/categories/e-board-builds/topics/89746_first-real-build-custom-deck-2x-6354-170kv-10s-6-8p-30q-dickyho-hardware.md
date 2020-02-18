# First Real Build &#124; Custom Deck &#124; 2x 6354 170kV &#124; 10S 6/8P 30Q &#124; Dickyho Hardware

### Replies: 7 Views: 556

## \#1 Posted by: Vykku Posted at: 2019-04-07T22:14:22.415Z Reads: 195

```
I am currently using a 27" Ownboard deck swap for commuting to uni since that's all I could fit under the seat. However now I have a space to store and charge it there, so I decided to build one from scratch suited for my needs and wants.

To keep things short, I have main 3 requirements:

* **Bigger wheels**. The current 90mm are sometimes unforgiving for the London suburb roads.
* **Range**. I was hoping I could get about 25 miles on it. This means that I can cross out the pneumatics, so I decided to go with Dickyho's 145mm solid wheels since I should hopefully get better range on them while still making the ride more comfortable than on 90mm wheels.
* **Larger deck**. I am not constrained anymore in terms for size, and I would need a big deck for the wheels and batteries.


Parts List:

* **Deck**: I was thinking to get the Hummie deck, but I couldn't find any for sale, and I would like having the motor direction flipped so it would be a bit more stealthy (and I wanted to be able to hold it vertically and not have the motor mount hit the ground). I found a local guy who makes custom decks, and he will make me a deck to my specs. It would be 15ply so I will be able to route out a cavity for batteries and ESC, while maintaining it's structural rigidity. Here are some renders of the deck (along with a crude model of the trucks, wheels and motor mounts):

![12%20(2)|690x388](upload://lO9ZCXxTWMEj5pElVXLJop2VQvq.jpeg) 

It would have a logo laser etched in the middle. Undecided between laser cut black griptape just where the feet are, or clear griptape on the whole deck:

![12%20(1)|690x388](upload://aTnzHI7CgjTm2PBghme94L15SGw.jpeg) 

Photo of the cutout on the bottom. I will route it out at the end as I first need to work out the dimensions I would require:

![12|690x388](upload://dWk1bYBYJ7RP6C1785mpHYynx2z.jpeg) 

The direction of the motors:

![37%20(1)|690x345](upload://3knifJ4dIoheXFewQdwv2QGm3ch.jpeg) 

The board will not be uniform, with the front tip being shorter than the rear, to accommodate for the motors.

* **Wheels:** Dickyho's 145mm solid wheels seemed to have pretty good reviews, and they are pretty cheap, so I ordered them. Worst case scenario, if they are not quite what I want, I can always resell them for a reasonable price, and buy something else (probably Trampa 125mm Gummies). 

* **Trucks and Motor Mounts**: I ordered these from dickyho again, since they are the cheapest things on the market, and still seem quite decent quality. All I would need is new bushings and pivot cups since they are not too great, as expected. 

* **ESC:** I've been using the Ownboard ESC for a while and it seemed pretty decent, so I decided to get the Dickyho's ESC, since it was only about £50 including remote and power switch, and even if I don't end up liking it, I could resell it without a big loss, and get VESCs instead.

* **Motors**: I am using 2x sensored 6354 170kV, again from dickyho, since they are cheap and the right kV for my setup. I am using 15/60 gearing, so I would be aiming at about 25 mph max, which is pretty much perfect for me. The roads here are not good enough to be trying to go faster, and I will not go offroad to justify bigger more expensive motors.

* **Battery**: The lipos are quite a bit cheaper than the liions, should handle higher current, and are somewhat more modular, so I decided to go with them. The best value, while having suitable dimensions, turned out to be the Hobbyking 5S 8Ah lipos, and I would be running 2S2P with them with a BMS. They are easier to damage than Li-ions, but I am planning to use individual Lipo fire bags for them, and also would use a fiberglass enclosure in general, so it should be pretty safe. Their height is 39 mm, and I expect the lipo bag and padding to add about 15 mm, but there will still be plenty of clearance due to the large wheels.

* **Enclosure**: It would be a custom deck, so I will need a custom enclosure. I got a CR10 that sits idle most of the time, so I am planning to make the enclosure out of fibreglass while using a PLA negative mold. There was a Youtube video where someone has done fibreglass parts using 3D printed molds and he achieved impressive results, so I would follow his instructions.

I will use this thread as a build log. It will probably take a few months to complete it, but I am in no rush due to being quite busy with university.

Feel free to add any suggestions or comments about it!

**12.05.19:**

I decided against the Lipos as they seem to last less cycles than 18650 cells, and also they are much easier to damage. I ordered a Boss spot welder (was going for the MiniA one, but I do need a new soldering iron as well), and a Bestech 80A BMS.

I will have space for dual stack batteries, so it will either be 10S6P or 10S8P 30Q with PCBs depending on how much space there is on the deck.
```

---
## \#2 Posted by: Grozniy Posted at: 2019-04-08T08:31:42.612Z Reads: 146

```
Looking forward for the build
```

---
## \#3 Posted by: Vykku Posted at: 2019-04-08T12:23:47.119Z Reads: 141

```
I received dickyho's parts, and I am pretty happy with them. First think I noticed is how heavy it turned out to be, the rear truck with wheels, 60T pulleys, motor mounts and motors are 3.9kg, but it does feel pretty high quality. Here are some pics of the rear truck with motors mounted: 

Front view:
![DSC02276|690x460](upload://2uqQO1syYPHF9I2Cc6sUXudGCKL.jpeg) 

I will spraypaint the outer circular aluminium piece that holds the pulley black so it would not be as noticeable.

Top view:
![DSC02277|690x486](upload://f2gq43fVz6jblCsqS6H1hdSFHwz.jpeg) 

Rear view:
![DSC02278|690x460](upload://r5a0lKEVQXNRWtxwVvPkByE1pVL.jpeg) 

I have bought his adjustable crossbar (Ebay number 303033848672), but I found it hard to install, and once installed it is hard to move the motors to adjust the tension. It might be different for you however. SInce my motors are forward mounted, I wanted some cover for them to help against small pebbles and dirt. I designed and printed the following cover which uses the pulley covers and bolts and nuts that come with the trucks:

![image|690x361](upload://d6mB99yw93NZWwL6eW2JGI5mU16.jpeg) 

I printed it out of PLA mainly as a test. When I will start seeing any issues with it, such as delaminating, cracks, etc, I will reprint it out of PETG or ABS.
```

---
## \#4 Posted by: Vykku Posted at: 2019-04-19T12:24:04.052Z Reads: 104

```
New update, the deck mold was done and it is ready to be vacuum pressed. The drop down might be a bit more mellow than originally designed since the deck will use 15 ply and needs a lot of force to bend, but it will still be enough:

![30|666x500](upload://oWZVlAQDBHJVuAbbxbNNyN8fSdj.jpeg)
```

---
## \#5 Posted by: Vykku Posted at: 2019-05-01T17:22:11.387Z Reads: 82

```
The deck is almost done, just needs a few more layers of varnish. It ended up having 12 ply instead of the originally planned 15.

Big thanks to Big Aye Skateboards to building it close to my original design.

![image|281x500](upload://nH7R9KSGVxaJ7LtakSUQoAiQmGD.jpeg)
```

---
## \#6 Posted by: Vykku Posted at: 2019-05-12T20:30:18.190Z Reads: 59

```
Well, it seems that by the time I finish the build, it will be nothing like originally planned. I decided against the Lipos as they seem to last less cycles than 18650 cells, and also they are much easier to damage. I ordered a Boss spot welder (was going for the MiniA one, but I do need a new soldering iron as well), and a Bestech 80A BMS. 

I will have space for dual stack batteries, so it will either be 10S6P or 10S8P 30Q with PCBs depending on how much space there is on the deck. I will find out once I collect the deck, hopefully at some point this week.

So next things on my plan are:

* Work out the required enclosure dimensions (including enough spare space for future upgrade to VESCs), print out a negative mold, and make the enclosure out of fibreglass.
* Build the battery pack
* Do all the finishing bits, install the parts, griptape, connectors, cable management, 

I don't have a lot of time due to uni exams and assignments, so I expect to finish everything somewhere around mid of July.

Then once I want to upgrade, I am planning to get better large wheels (125mm gummies and maybe a set of pneumatics), better trucks, VESCs, larger motors and possibly 12S batteries if I feel the need for higher speeds and more torque.
```

---
## \#7 Posted by: Vykku Posted at: 2019-05-30T23:00:26.703Z Reads: 50

```
Due to recent circumstances, I decided to update this build thread in the future on the  forum: 

https://forum./t/long-range-commuter-custom-deck-2x-6354-170kv-10s-6-8p-30q-dickyho-trucks-wheels-mounts-esc-for-now/1426
```

---

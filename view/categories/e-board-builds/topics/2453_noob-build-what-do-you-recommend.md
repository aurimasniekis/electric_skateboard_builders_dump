# Noob build - What do you recommend?

### Replies: 6 Views: 1160

## \#1 Posted by: tha-mikey Posted at: 2016-04-19T15:03:55.694Z Reads: 106

```
Hi i am Mike,

At first I want to make a reliable e-board because i would like to have one as a daily driver. Secondly I want the board to be easy to maintain (i.e. easy to charge and no swapping out of components) The reason I don't want to buy something like a boosted board is because I feel it will be cheaper to build it myself and I would learn a lot from it.

I am not a very demanding user. There are not a lot of hills in my country (some bridges but thats it) and i usually go somewhere around 20 km/h, but it would be nice to achieve 30 km/h every once in a while. 

The main problem is that I am overwhelmed with information on some fronts but lacking on the others. For example I have no idea which motor to get, but there is so much debate going on about the vesc vs the generic car esc that i have no idea if the vesc is reliable enough to be used.

I hope you will forgive my bad english and my lack of knowledge about electronics. I have read a lot but everything is just really confusing. 

So my main questions are:

1. What formulas are used to calculate the needed specs for an E-board?
2. s a vesc worth it or not stable enough yet? and if so where do i get a stable one?
3. What batteries do you recommend? I read lipos are bad but what is the alternative? I ve read something about using a BMS
4. How much should I expect to pay for al the electric components for an E-board?

Mike
```

---
## \#2 Posted by: mattdig Posted at: 2016-04-19T16:45:32.067Z Reads: 101

```
Start with the board.
You want a deck that gives you at least 16"-20" between the trucks, and decide if you want a tail.

Then you have to make a decision: are you going to get a complete truck/mount/wheel/pulley kit from somewhere like Enertion, or get everything in pieces from various vendors? (I recommend going with the Enertion kit, it will just save you a ton of time and headaches).

Then you need a motor, ESC and battery.

Lipos are great and cheap, just don't puncture or overcharge it. A 6S battery will work better than you expect, but more is better. Make sure the C rating equates to at least 60A max draw, again more is better.

VESC is the best thing around if you plan to run more than 6S. Otherwise just get any RC car ESC that supports 6S and about 100A.

The motor just needs to be somewhere in 190kV - 260kV. Any SK3 6364 from HobbyKing will work.

I'm using a 245kV motor, with a 6S battery (8Ah, 30C), and a 6S/90A RC helicopter ESC. It can do 20km/h easily and 30 if I'm feeling brave, and 10km per charge.

Mix and match as you see fit and as your budget allows.

If I was doing it over, I'd get 2 4S/10Ah LiPos, in series, (for 8s/10Ah) and a VESC. But I'd keep the motor I've got.

Budget at least $800USD. On top the main components you need the battery charger/balancer, battery case, switches, wiring, hardware, and any tools you might be missing.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-04-19T17:22:26.374Z Reads: 85

```
Here's a great deal mate...just bought one last night ...thanks to @Mobutusan

 http://www.electric-skateboard.builders/t/hobby-king-deals-sales/2450?u=michaelinvegas

If you looking for hardware...I can vouch for Enertions / @onloop's stuff and he just put up more things.

DIY skateboard / @torqueboards is another place to check 

If you have time check the threads on this forum ... It's not out of control to search just yet...there are some great setups... Look up @RunPlayBack's ride  http://www.electric-skateboard.builders/t/esk8tube-video-thread/47/194?u=michaelinvegas which is a very popular one in this forum because of its clean design...

But yes...starting with a board in mind is probably the first step as @mattdig mentioned....then work around that..

It's not that complicated once you sort it out in your head...it's just getting the parts....then soldering and bolting things together ... There isn't a manual .... But it's very satisfying when you are done...people will be impressed
```

---
## \#4 Posted by: Mobutusan Posted at: 2016-04-19T17:46:44.082Z Reads: 81

```
Regarding wheelbase, I personally feel longer is generally better, for stability at speed and also not getting dumped on your arse from the torque of these motors. I feel like 23-28" wheelbase is the sweet spot for me at 69" tall and 165lbs. (Sorry for not using metric numbers; stupid imperial system.) I tried a board with an 18" wheelbase and it felt way to narrow and unstable for me. 

Also, check out this calculator to determine speed from motor/battery/gearing combinations.
http://toddy616.blogspot.com/2013/07/electric-skateboard-calculator.html?m=1

Also, stay single drive/motor if you want to keep costs down. And also know that you may have to wait a while if you want a VESC. There seems to be a perpetual shortage from most vendors, except maybe chaka/ollinboards. I think the shortage should be resolved soon when new inventory comes in, but there are a lot of people waiting right now.
```

---
## \#5 Posted by: tha-mikey Posted at: 2016-04-20T09:03:49.158Z Reads: 56

```
Thanks for the reply! I was thinking of mimicking the Boosted board design. I've seen someone use the following combination:
Vanguard flex 3, orangatang kegel wheels, caliber trucks

I can produce a motor mount myself and also have a friend whom can weld it on for me :slight_smile:

As for a charger I would like to have something portable to carry between work and home and from what I have seen from the Lipo chargers is that they are bulky and have a lot of wires to carry. 

Thanks for al the links! Sadly I don't have a lot of time left this month, but the coming months ill have more. That is why I want to start ordering the parts soon. 

I have found some formulas for the needed motor specs so i have that figured out now. Is it possible to expand to 2 motors later on? If the board is not strong enough, or do I need a second Vesc?
```

---
## \#6 Posted by: Michaelinvegas Posted at: 2016-04-22T05:49:13.468Z Reads: 48

```
Well one of the quickest solutions for the battery is Enertions battery pack and not sure who else.....you will need an esc that can handle the voltage...

And why copy boosted? Then just get a boosted....
There are so many other choices in boards...id pick something else...but it's up to you.

Also think about what controller you want...there are a few choices
```

---

# Trying to build a AT EBoard, need help

### Replies: 5 Views: 501

## \#1 Posted by: Eckhartt Posted at: 2017-10-28T18:02:46.261Z Reads: 105

```
I'm still a noob and extremely new to all this and I've been looking to build my (first) own AT EBoard. 

I've got two questions:


1. [This website](http://www.diyeboard.com) looks interesting and has all the parts I think I need. does anyone have experience buying from it? I live In Belgium if that's helpful. Maybe there is an even better website out there?

2. And what to you think about these parts; do they fit, work together? anything you would change?


these are the parts I've been looking at.

- [Wheels](http://www.diyeboard.com/8-20050mm-allterrain-offroad-pneumatic-tire-inflation-wheel-p-574.html)

- [Truck kit](http://www.diyeboard.com/11-422mm-off-road-all-terrian-electric-skateboard-truck-kit-p-582.html)

- [Battery](http://www.diyeboard.com/10s5p-18650-lithium-battery-pack-36v-10ah-360wh-p-460.html)

- [Lithium-ion Battery Pack & ESC  Enclosure](http://www.diyeboard.com/10s5p-lithiumion-battery-pack-esc-2-in-1-enclosure-p-504.html)

- [FOC ESC](http://www.diyeboard.com/upgraded-v21-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-599.html) 

- [Motor](http://www.diyeboard.com/180kv-n6354-outrunner-motor-2000w-for-diy-electric-skateboard-p-540.html) 

- [Belts](http://www.diyeboard.com/4005m-htd5-12mm-width-belt-for-8-pneumatic-tire-p-615.html)

- [Charger](http://www.diyeboard.com/10s-42v-2a-lithium-battery-charger-for-10s-electric-skateboard-p-512.html) - is this the right one?

- [Risers](http://www.diyeboard.com/longboard-shockpad-pu-risers-8mm-thickness-p-473.html) - do I need these?

- [Bolts and crews](http://www.diyeboard.com/8-pcs-deck-hardware-bolts-p-475.html) - do I need more?

- [Cable](http://www.diyeboard.com/xt60-power-cable-wire-connecting-battery-and-esc-p-591.html) - not sure if I need this.

- [Deck](http://www.diyeboard.com/38″-bamboo-deck-for-diy-offroad-all-terrian-electric-skateboard-p-578.html)

Anything I missed?
Like I said, I'm completely new to all this. So sorry for the beginner questions.
```

---
## \#2 Posted by: telnoi Posted at: 2017-10-28T18:57:35.616Z Reads: 80

```
My suggestion. Get a trampa or MBS mountain board, some sensored maytech motors,  2 or 4 5s 5000/8000 mah Lipo packs from Hobbyking, an isdt lipo charger and some good esk8.de or focbox controllers.

There are multiple issues with the components you listed.
Poor truck construction/springs only and no replacement parts available. Typically, you will have to replace bushings every 6 months or so. No replacement parts available at all anywhere. Springs only means it will be very poor at properly dampening unwanted movements, leading to speed wobbles. Then you have a non-standard size for the axis (10mm), meaning you won't be able to reuse things such as the wheel hubs and integrated pulley if you do decide to upgrade the trucks at some point in time and I can assure you...you will quickly outgrown those trucks.

The motor mount has a fixed length and fixed motor mount holes, meaning it will be compatible with only a few motors and you cannot alter the belt tension in a proper way.

The motors you listed are unsensored, meaning you will have issues getting going from a stand still or when standing on a hill.

The li-ion pack you listed uses poor performance LG mf1 cells, which in a 5p configuration delivers 50a. Enough for a single motor drive, but not dual. In addition, braking will be limited to 20a combined, which is not enough for efficient braking. The voltage sag is rather severe on a dual drive and you will notice a significant drop in performance after 8km or so, or after a significant climb.

The esc you listed has limited performance..also capped at 50a. Suitable for paved roads.

I owned most of the parts you listed and am in the process of replacing them all one by one.
```

---
## \#3 Posted by: diyeboard Posted at: 2017-10-28T19:17:29.222Z Reads: 63

```
you are really not a kind person bashing us without reason, you even never bought from us, and you bought a kit from somewhere we don't know, and you keep bashing us everywhere, be kind, as i said it is quite different quality level because you buy the cheap one from other place.
really feel sorry for you, not a kind a people at least.
```

---
## \#4 Posted by: telnoi Posted at: 2017-10-28T19:26:59.278Z Reads: 67

```
Basing it purely on the facts, not fiction, based on the specs and images listed on your website, not on what I own and happens to look identical.

The esc is well known as are its limitations. It's good for a street build, not really AT.
The li-ion pack he linked to is indeed 50A (you confirmed it yourself elsewhere). By now I know for a fact that you need more amps for a good AT build.
The motors are unsensored. You sell sensored also.
The trucks are springs only, are they not.
They are 10mm, are they not.
You don't sell replacementt parts (yet).

Just voicing my opinion and providing someone with valid feedback..based on true specs.

It is just my opinion that the components are suitable for a beginner build, but if you are looking something that grows with you as you get better, this is not it.

P.S. I work for a sales department, thus I am rather sensitive to certain tactics that are often used.

Anyway, other well informed people can chime in and voice their opinion on the components. By all means, don't let your purchase depend on just mine.
```

---
## \#5 Posted by: telnoi Posted at: 2017-10-28T20:04:31.471Z Reads: 61

```
Just backing up my reasoning for choosing other components, whether they are from diyeboard or not I don't care. Only want you to have a good first experience with the knowledge to make informed purchase decisions.

For a Li-Ion pack it is recommended to go with a 10s5p pack containing for example Samsung 25R or 30q cell with a theoretical discharge of +-100A as opposed to 50. Reason being that the pack will suffer less from voltage sag under high load, which often happens during hill climbs and even grass patches. Braking performance will also be better. Most motors have a theoretical draw of 60A, so having two means you will be severely limiting the performance of the board if you go with 50A. I have first hand experience with that. Does not matter where the pack comes from, a LG MF1 cell is an LG MF1 cell.

Look for unsensored motor cogging if you want to see what startup is like using unsensored motors. Marketing talk will tell you that sensorless startup is perfect, but it never is. Even if you buy a motor controller or Vesc that is 5 times more expensive. There is a sensored version of that escyou linked to that will do better, but it's performance is still capped...and I may be wrong, but it could be just for hub motors.

The cheapest Vesc can output 50a, the more expensive 60A. Dual Vesc will thus give you a max of 120, enough to satisfy most all terrain motors.

As for springed trucks. There is video evidence of a completely different truck (mbs) with and without shock eggs highlighting the poor performance of springed trucks without any additional dampening. I looked for aftermarket shock eggs that will for the diyeboard or diyeboard clone trucks, but there are none that will fit.
```

---

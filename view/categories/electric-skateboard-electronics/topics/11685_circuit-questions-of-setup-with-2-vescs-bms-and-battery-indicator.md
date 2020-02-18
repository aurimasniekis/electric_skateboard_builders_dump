# Circuit questions of setup with 2 VESCs, BMS and Battery Indicator

### Replies: 5 Views: 1221

## \#1 Posted by: freeh18 Posted at: 2016-10-22T13:47:54.432Z Reads: 96

```
Hey guys and girls,

since a few weeks i'm reading quite a lot in this forum and currently i'm planning the setup of my very first electric skateboard.
I'm pretty confident in my setup. Nevertheless i have some questions. Here is drawing, showing the components and the wiring.

<img src="/uploads/db1493/original/3X/5/e/5e0b1afa0c3b6f40a07ab4371a24392bd0288bd4.png" width="566" height="500">

As you can see im planning to get two motors, powered by a 8s1p [battery](http://www.hobbyking.com/hobbyking/store/__80900__Multistar_High_Capacity_4S_20000mAh_Multi_Rotor_Lipo_Pack.html) configuration with 20Ah.
Hopefully im getting quite some range from it. Since i'm totally new to longboarding, speed is not the main aspect.

1.) Is there something completely wrong with it? (would be good to know before i order all the components :sweat_smile:)
2.) What kind of charger do i need? (i thought of some kind of laptop thing, to make is as easy a possible)
3.) The BMS (Battery Management System) stops charging when the batteries a full, right? (so charging over night wouldn't be a problem)

Thanks a lot in advance!
Is it possible that this stuff gets kinda an addiction? :fearful:

Greetings!
```

---
## \#2 Posted by: rubz Posted at: 2016-10-22T14:17:54.563Z Reads: 70

```
Hey,

Are charging cathode CH- and discharge cathode P- connected to each other? You should make sure that you can charge the batteries over the discharge connection of the BMS because the VESCs will send a charge back to the batteries when braking. The rest looks okay, although your battery status indicator is wired in a weird place, it should work like this, but i would just wire it parallel straight behind the bms before splitting the cables to the VESC.
Also, please note that many people have mentioned issues with the nunchuck (not so stable).
```

---
## \#3 Posted by: rpn314 Posted at: 2016-10-22T15:20:53.994Z Reads: 59

```
He's got a red and a black line, so I don't think the CH- and P- are connected.

To second @rubz, if you're looking for a nunchuck, the only one I can really recommend is the NRF that vedder made (it's not just an off the shelf wireless nunchuck though, requires some work). It's definitely the one with the least problems. Everything else looks great.
```

---
## \#4 Posted by: Jinra Posted at: 2016-10-22T16:34:03.057Z Reads: 60

```
P- and Ch- are usually connected on bms's. They're the same port in essence.
```

---
## \#5 Posted by: rpn314 Posted at: 2016-10-22T19:37:34.509Z Reads: 50

```
I would say it depends on the BMS. For example The P- port may allow 60A going out and in, while the CH- port may only allow 5A
```

---

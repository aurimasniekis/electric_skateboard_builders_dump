# Please help me! Battery reading at 4.2v

### Replies: 7 Views: 154

## \#1 Posted by: nativejibroney22 Posted at: 2019-11-21T03:38:39.555Z Reads: 50

```
I built my board and it ran, did everything it needed to so I started designing the enclosure to 3d print it. The board sat for a month (with bluetooth bms and vesc plugged in) and now I am getting everything set up to put together and the battery is outputting insanely low voltage. I made a 10s5p battery out of samsung 30q's so it was originally max charge at 42v. A couple of weeks ago I checked the voltage and it was at 38v. Now for some reason it is at 4.2v which shouldn't be possible. Any advice on where to go from here or why this is happening?? I was so excited to have the board together by next week...
```

---
## \#2 Posted by: JohnA Posted at: 2019-11-21T03:49:40.775Z Reads: 49

```
Is the BMS wired as charge only or wired to discharge? Was the vesc plugged directly into the battery (so always on) or do you have an anti spark switch in between? Able to send pics of the setup or construction?
```

---
## \#3 Posted by: Halbj613 Posted at: 2019-11-21T08:21:08.156Z Reads: 42

```
Sounds like the battery is insanely low and probably won’t be able to get it back together

Though please ask the question on the  forum as much more active and better community

I think the only solution for the problem would be to charge it with a balance charger at an insanely low rate such as 0.1amps

Not 100% sure though
```

---
## \#4 Posted by: nativejibroney22 Posted at: 2019-11-21T19:04:01.311Z Reads: 27

```
So my wiring set up is that the negative lead goes from the battery to the BMS, then the negative goes from the BMS to the VESC and the positive goes straight from the battery to the VESC. I also have a positive to a charge port and the negative of the charge port to the BMS.
```

---
## \#5 Posted by: TowerCrisis Posted at: 2019-11-21T20:31:25.109Z Reads: 25

```
Measure the voltage directly at the battery terminals, not through the BMS.

It's possible undervoltage protection has kicked in and the BMS has switched the pack off.
```

---
## \#6 Posted by: JohnA Posted at: 2019-11-21T22:00:46.380Z Reads: 23

```
sounds like its wired correctly. I second @TowerCrisis, you should check the battery voltage before it goes into the BMS. Or you could unplug the balance wire from the BMS and check each P group voltage.
```

---
## \#7 Posted by: nativejibroney22 Posted at: 2019-11-22T21:42:27.138Z Reads: 15

```
So each pack is reading on average 0.65v and there are two that are at about 0.15v. Not sure what to do with this. I don't think i can afford to build another pack right now and I was so close to being done with my board...
```

---

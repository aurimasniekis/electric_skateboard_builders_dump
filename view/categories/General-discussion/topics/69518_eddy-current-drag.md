# Eddy current drag

### Replies: 15 Views: 356

## \#1 Posted by: amazingdave Posted at: 2018-09-29T07:00:32.807Z Reads: 108

```
I’ve noticed that quite a few motor mounts now have aluminium cross bracing/ protection bars right next to the motor cans. This must be causing some drag, no?

![image|480x270](upload://oP2sCQ37OX9OtP9aY1yQMUBSb7Q.gif)
```

---
## \#2 Posted by: TowerCrisis Posted at: 2018-09-29T07:24:50.682Z Reads: 100

```
Copper's around 2x as conductive as aluminum, so the effect should be much less than what's depicted above.

Plus, a magnetic fiends strength is a function of distance squared, so any significant separation should reduce drag to nearly nothing.

A big part of why brushless stators need plate isolation to reduce eddy currents is because of how fast and how close the magnets are.
```

---
## \#3 Posted by: amazingdave Posted at: 2018-09-29T07:44:24.134Z Reads: 98

```
I see that the effects are less but the 2 real world applications of passive eddy current brakes I have come across use aluminium plates at a separation of 8-15mm (Forest roller coaster in north wales and a vertical drop ride). 

Get a big neodymium magnet, stick on a wooden sled 10mm thick and slide it down an aluminium plate. Then tell me the effect is negligible. (obviously doing a peer reviewed comparison with an equivalent mass) 🤓
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-09-29T07:51:19.829Z Reads: 89

```
You're also ignoring that the magnetic field outside of a brushless motor is very weak. The orientation of the magnets yields a near net 0 magnetic field outside of the can.
```

---
## \#5 Posted by: TowerCrisis Posted at: 2018-09-29T07:57:36.562Z Reads: 84

```
https://photos.app.goo.gl/PLK5f4TwfHrZtkps5

Eddy currents are really something you only need to worry about inside the motor can.
```

---
## \#6 Posted by: b264 Posted at: 2018-09-29T08:02:27.898Z Reads: 78

```
Wrapping the magnets with a steel can should effectively eliminate this phenomenon, but we should get some empirical data...
```

---
## \#7 Posted by: amazingdave Posted at: 2018-09-29T08:02:28.778Z Reads: 76

```
Your motors must be better made than mine! My keda 190kvs and dark matter 190kvs stick pretty well to each other if they end up too close on the bench!
```

---
## \#8 Posted by: TowerCrisis Posted at: 2018-09-29T08:04:03.910Z Reads: 75

```
Exactly why I just purchased some magnetic viewing film with 1 day shipping ;)
```

---
## \#9 Posted by: amazingdave Posted at: 2018-09-29T08:07:57.972Z Reads: 74

```
A motor mounted on the bench with a vesc for current recording and some aluminium plates in a clamp would seem to be the best empirical test to me. I’m all out of spare vescs... anyone?
```

---
## \#10 Posted by: TowerCrisis Posted at: 2018-09-29T08:10:45.452Z Reads: 72

```
I mean the easiest thing to check is if there's any kind of force on an aluminum bar you just dangle next to it. My bet is that there'll be 0 or near 0 force on it. If you can't feel it then it's insignificant.

I can check this out tomorrow
```

---
## \#11 Posted by: Brdchris Posted at: 2018-09-29T11:26:51.235Z Reads: 60

```
they stick together while running? They need to be powered up to reduce magnetic field outside the can.
```

---
## \#12 Posted by: amazingdave Posted at: 2018-09-29T11:32:25.112Z Reads: 59

```
If they stuck together when running I’d have fu*ked something up good and proper!
```

---
## \#13 Posted by: TowerCrisis Posted at: 2018-10-03T00:52:35.255Z Reads: 44

```
Here are some results.

![IMG_20181002_171316|281x500](upload://6psFsldJkMMAH74Cwmhs0komo8M.jpeg) 
This is the motor without the stator inside. The black ring on the outside is the outer steel can. Poles are dark, and the edges are light.

Inside, the field is quite strong. The edges meld together as the poles transition from north to south.

Inside the steel of the can you can see very weak edges. Outside of the can there is nearly no field. The field is nearly zero at any kind of distance from the can. The randomized patterns around the motor are remnants of previous tests, they do not dissipate on their own without a magnetic field. So it is safe to assume that the cans magnets are not affecting those areas.

Here is the side.
![IMG_20181002_171348|281x500](upload://aTn9hi7mTDeMHakknVUkZ0dYVfu.jpeg) 

As you can see, the field is strong on the surface of the can, but not strong at any distance (as depicted in the previous photo.)

The left side shows very sharp magnet corners, while the right is very curved.

That is because the curved side has a steel magnet retainer while the left is aluminum. The additional steel clearly shows us that it is suppressing the field in that area.

Here is the side with the can on the stator.
![IMG_20181002_171542|281x500](upload://z6whcA0bLy8YnSfDOnKs1Vmd4t7.jpeg) 

As you can see, the stator is clearly affecting the magnetic field. This makes sense since the stator is meant to conduct the field by the copper.

Here is the top.
![IMG_20181002_171515|281x500](upload://qutrQhEf2QDEgfWhaR7DOqUIrOO.jpeg)

And again, the field is slightly stronger than before.

However, this is only on the edge of the can. If measured in the middle, there is hardly any field.

![IMG_20181002_174451|281x500](upload://7AYGF0YStlNmZeDbPV9bCcNYSAH.jpeg) 

The can is very effective at eliminating the field. Any attraction between motors is likely from field leakage at the ends. This field is very small and is only strong at very very close distances. The side views of the cans is a perfect indication of this, as it appears very dark but that is only because the film is right up against it.
```

---
## \#14 Posted by: PatRocks Posted at: 2018-10-03T01:13:43.690Z Reads: 38

```
Good answer @TowerCrisis
```

---
## \#15 Posted by: amazingdave Posted at: 2018-10-03T05:25:27.736Z Reads: 33

```
I tested the drag in the basic way you described @TowerCrisis and the results echo yours, within 2-3mm there was a great deal of drag but by 5mm it was imperceptible. That film is amazing for visualisation of the fields, good job. 

 I’ll be making up my aluminium cross bracing tomorrow then!
```

---

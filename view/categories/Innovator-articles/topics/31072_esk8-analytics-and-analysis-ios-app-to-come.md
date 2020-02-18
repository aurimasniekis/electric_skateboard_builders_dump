# eSk8 Analytics and Analysis \[iOS app to come\]

### Replies: 8 Views: 893

## \#1 Posted by: Esrapp21 Posted at: 2017-08-19T23:40:23.479Z Reads: 157

```
**Introducing eSk8 Analytics and Analysis**
----------
This is an app currently only for iOS that is meant to be used with your VESC monitor, such as metr.at or rocket board device. In V1.0, the app can be used to make board specific calculations based on speed, incline, distance, motor power withdrawal, battery watt hours, and more. Using all of these variables, it creates a three dimensional graph that contains every single ride possible on your board. With each ride you input into the app, the more accurate it gets.

**Calibration**
With a normal 2D calculation, you would only need three rides to create a parabolic, logarithmic, sinusoidal, or otherwise trigonetric power curve. However, because there are so many factors that go into these calculations, a 2D graph would not be sufficient. For this reason, a 3D graph is the most favorable option, but there is one sacrifice, and that is the amount of rides needed to create a quadratic, logarithmic, or trigometric curve. You will need to record 10 test rides, 9 of which are for the making of the graph, and the last one being for accuracy. The rides are as follows:

* 3 rides with 0 NE, each with varying amph
* 3 rides with the same NE, each with varying amph
* 3 rides with the same NE, each with varying amph
* 1 zero distance ride, using not using remote to see resting power usage

While these may seem daunting, they are rather simple. First of all, just for clarification, NE means Net Elevation, or end elevation minus start elevation. So, for example, 0 NE means you start at the same altitude you end at. For those 3 0 NE rides, I suggest doing flat rides. As for the other 6, no I didn’t make a mistake. There are two of the same. For the first three, go the same route. For the next three, just do a different route than the previous three, three times. An easy way to accomplish these six is just go on a route out and back three times. The three out are one route, and the three back are another. 

The other acronym is amph. It could also be akph. This is average miles/kilometers per hour. For each set of three rides, you need a different amph for each of the rides. 

It seems complicated, but in the end it is just three flat rides, and three out and backs, varying your average speed. Easy enough. Then, we have one more ride. This is the easiest, you just turn on your board for about half an hour to an hour, and check how much power it has used. Most times it should be zero, but this is just a base. Once you have logged all these rides, I highly encourage you to log every ride you do. The more rides you do, the more accurate it gets.

**Calculations**
Now for what everyone is waiting for. What does it do? Why does it need all of this info? Is this worth my time? Well, using the POWER OF MATH, and all of your logged rides, the app can calculate many numbers. Let’s say you have a 26 mile ride ahead of you, and you don’t know if you can make it. Or you know you can make it, but you know if you just gun the throttle, you won’t. Well, all you need to do is put in the distance of your trip, the altitude of your start point, and the altitude of your destination. Then, it willl tell you if you can make it, and if so, your max amph or akph.

Another feature is caulculating your true range, not hypothetical. Instead of taking your battery’s and motor’s maxes and maxing a max possible range, it takes all of the info you have given the app, and an NE you give it, and calculates not only your max range, but the amph you need to have to get it. If you want a base to compare, try giving it 0 NE to see how far you can go on flats.

There will be some more types of calculations, but if you have any suggestions, PM me and I’ll see if it is practical.

In the future, I’m hoping to add graphs in the near future, but you all know how iOS UI coding is...

**Extra details**
So at the moment the app is still in development, I’m hoping it will be in beta stage within the next week or two. I will update when it is and host a public beta on the forum if you guys want. The app is gonna be free, but in maybe 6 months when I expect to be done with graphs, the graphs may be an in app purchase. 

Please tell me your feedback! What do you think? Any other feature suggestions? I have to say, this community inspired me to make this, and after everything you guys have done for me, I hope this does as much good for you!

----------
```

---
## \#2 Posted by: Rinzler Posted at: 2017-08-20T00:02:58.058Z Reads: 134

```
*slow clap* :clap:...:clap:...:clap: wow, another great innovation on the forum.Soon the diy board will be the most advanced board that you can have because this community just keeps on innovating, we already surpassed most eboard makers in the performance category.Hats off to you!
```

---
## \#3 Posted by: Esrapp21 Posted at: 2017-08-20T00:13:03.233Z Reads: 124

```
Thank you! I also am amazed by what people on this forum have created, and manufactures have nothing on us!
```

---
## \#4 Posted by: Nate Posted at: 2017-08-20T02:12:33.802Z Reads: 108

```
This is actually pretty neat. Is it possible to integrate it into google map or vice versa?

Also, i'm really impress with this.
```

---
## \#5 Posted by: karma Posted at: 2017-08-20T11:17:19.509Z Reads: 96

```
This seems like an advanced app for more irl calculation, great work! 
I don't know how much time I will have now when university start again but I am interesed in helping with the Frontend/UI on iOS
```

---
## \#6 Posted by: Esrapp21 Posted at: 2017-08-20T14:04:27.509Z Reads: 88

```
@Nate It seems like there are some APIs for that, so in the future that seems like something I could implement.

@karma That would be great! I’m currently just throwing together a beta right now, but when it comes time to start introducing graphs, google maps, etc that would be a huge help.
```

---
## \#8 Posted by: Esrapp21 Posted at: 2017-08-27T15:59:57.367Z Reads: 52

```
Sorry for the wait, iOS core data is hell on earth. I expect a beta release within the next week or two.
```

---
## \#9 Posted by: Esrapp21 Posted at: 2017-09-04T15:26:14.052Z Reads: 49

```
The app is finally in the alpha stages! Right now I’m testing the calibration, and one thing I’m noticing is that the phone’s altitude tracking is very inaccurate.[This](https://www.daftlogic.com/sandbox-google-maps-find-altitude.htm) is a better alternative to your phone’s altitude.
```

---

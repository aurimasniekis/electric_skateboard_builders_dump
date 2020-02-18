# Brake system controlled by transmitter

### Replies: 21 Views: 1304

## \#1 Posted by: NeverStopSeeking Posted at: 2018-05-28T21:51:28.461Z Reads: 204

```
Is there any project already made with a brake system that act on the wheels  ( sort of like this: https://i.pinimg.com/originals/17/8e/58/178e58ad9e7bf2e5ff441cb5f40b2686.jpg) but smaller and controlled by the radio transmitter so that when you brake on the radio an actuator moves the brake for you?
```

---
## \#2 Posted by: Deckoz Posted at: 2018-05-28T22:13:40.614Z Reads: 195

```
All you need is a mechanical system that hooks up to a pwm servo. Put the servo on the throttle channel and orient the head in the direction needed to activate the brakes.

There are a handful of examples on the google
```

---
## \#3 Posted by: NeverStopSeeking Posted at: 2018-05-28T23:28:57.029Z Reads: 170

```
Do you have some links? i can not find anithing similar to what i described , thanks :)
```

---
## \#4 Posted by: Deckoz Posted at: 2018-05-29T00:07:22.040Z Reads: 154

```
https://pinshape.com/items/36968-3d-printed-electric-longboard-brake
```

---
## \#5 Posted by: NeverStopSeeking Posted at: 2018-05-29T07:27:50.293Z Reads: 117

```
Thanks you for the link, but ti was looking for examples with proof that the project works in the real world. Online there are some examples, but i could not find one that shows that it really works. 
If anybody knows something would be great !
```

---
## \#6 Posted by: Okami Posted at: 2018-05-29T11:23:54.187Z Reads: 100

```
I was looking into this but the price of larger servo motor put it me off a bit.. though if u got 20usd to spend and then tinker to make it work, i think it is worth it.

I was planning to adapt it to mechanical disk brakes (for mountainboard) so im not sure what can u come up with for longboard..

I think either way u would need some sort of drum or disc, which gets pressed, so that the wheel can start to slow down. 

On youtube there should be a few examples but im not sure i can find them now
```

---
## \#7 Posted by: xilw3r Posted at: 2018-05-29T11:54:23.105Z Reads: 91

```
That design in the link Deckoz gave you did work. There is a video on YT of the design process and testing, but I cant find it right now for some reason.

I came across a similar idea though
https://www.youtube.com/watch?v=wIPTZ6A35Ok

The problem with servo activated brakes IMO is the rather low torque they can put down on the brake pads, you need some clever mechanical advantage to use those if you want to stop fast.  And then we are probably not talking about 180 deg turning servos anymore
```

---
## \#8 Posted by: Bobby Posted at: 2018-05-29T16:21:47.807Z Reads: 74

```
@Kug3lis posted a video of these two guys using a brake system not too long ago... ill look for the post
```

---
## \#9 Posted by: Bobby Posted at: 2018-05-29T16:24:30.270Z Reads: 74

```
https://www.youtube.com/watch?v=snge8JWwJyQ
```

---
## \#10 Posted by: Okami Posted at: 2018-05-29T16:52:25.326Z Reads: 70

```
Looks cool. More details on how he made it would be nice. 

From video (when watching on phone, it was a bit hard to understand what is being pushed against disk rotors.. 

Other than that glad that someone has made it even for longboard
```

---
## \#11 Posted by: Benjamin899 Posted at: 2018-05-29T17:14:49.790Z Reads: 65

```
i can't even see it on my computer.
Another idea would be to use a hydrolic discbrake. I have no real idea how to realise this but if you have enough space under your deck, wouldn't it be possible to build a pump which is controlled over the remote and the energy needed would come from the braking current or from the battery. Those discbrakes would be mounted at the frontwheels.
```

---
## \#12 Posted by: Okami Posted at: 2018-05-29T19:31:27.217Z Reads: 58

```
Interesting idea. Though not sure how much extra weight it might add, plus a bicycle mechanic i know, said that hydralic disk brakes at least for bicycles are really 'touchy', so to speak..

I think he meant they are quite sharp and requires minimum effort to apply, i might be concerned thus that for eboard they might be too strong and sensitive.

Disk brakes ive got on bicycycle works quite nicely.. hard to tell whenever hydraulic ones would be much better

---
Only benefit I see that motor would need to work a lot less, to activate them (pull the cable)
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-05-29T19:40:56.388Z Reads: 52

```
well i wouldnt use a traditional brake, maybe just a oldschool brakepad pressing on one side, since space is an real issue here
```

---
## \#14 Posted by: Okami Posted at: 2018-05-29T19:45:05.262Z Reads: 49

```
Yeh i think this is how it was made on that mountainboard servo brake video i saw a while ago..

Though what @Bobby  posted looks a bit more high tech.. should take a look at on bigger screen
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-05-29T19:46:23.566Z Reads: 46

```
that video of the mountainboard was awfull, that brake hat zero functionality
and that @Bobby video was so low quality that i coulndt see anything. I dont understand why people do videos at night. But yeah like that at the end. But i would install them in the front, so you brake with your motors and in front, spreading the force on all wheels.
```

---
## \#16 Posted by: Deckoz Posted at: 2018-05-29T19:55:04.468Z Reads: 50

```
Regenerative braking is just shorting the motor phases and sending the current back to the battery

Installing brakes on the front only takes away from the torque generating the current for regeneration on the rear motor wheels
```

---
## \#17 Posted by: Benjamin899 Posted at: 2018-05-29T20:00:55.033Z Reads: 49

```
ok good to know
```

---
## \#18 Posted by: Benjamin899 Posted at: 2018-05-29T20:08:49.579Z Reads: 52

```
But still. Where do you add the sattle if the mount is in the way of all that. Seems to me the front is easier to realise or you have hubmotors and somehow add a mounting device to them so they rotate with the hubs together.
```

---
## \#19 Posted by: Deckoz Posted at: 2018-05-29T20:11:22.003Z Reads: 51

```
I'm not saying you can't put brakes on the front.

Just, sharing the load with mechanical brakes, you will regenerate less watts then the motors braking independently on thier own without a mechanical assist.
```

---
## \#20 Posted by: Benjamin899 Posted at: 2018-05-29T20:15:17.399Z Reads: 51

```
no i got that, i just saying, where do i put them with all the other stuff in the way, thats the tricky part
```

---
## \#21 Posted by: Deckoz Posted at: 2018-05-29T20:17:30.589Z Reads: 49

```
Oh just put em on the front trucks :) then they aren't in the way :)
```

---

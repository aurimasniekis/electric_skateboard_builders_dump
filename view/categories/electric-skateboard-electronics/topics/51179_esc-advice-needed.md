# ESC Advice needed

### Replies: 11 Views: 586

## \#1 Posted by: Shoobee Posted at: 2018-04-03T19:19:54.858Z Reads: 116

```
@pat.speed 

You sound like the man to ask!

Hi Pat, My name is Andrew and In my first build I just blew out my esc 120a ha ha.

what would you recommend, considering this is my set up below. thank you.

I have a 270K 1800w 54.05 max amp motor.

3 3s 5000mah 30c-40c lipo's with two series connectors

I just purchased a 12s 120a car esc opto hv and am wondering if the vesc is better and more flexible in its use.

Is it silly to have this 270 kv motor... do I need 190kv for all around better?
```

---
## \#2 Posted by: b264 Posted at: 2018-04-03T19:53:43.433Z Reads: 111

```
[quote="Shoobee, post:44, topic:51004"]
Is it silly to have this 270 kv motor
[/quote]

Yes, on 9S it might be a bit much as a 62,937 erpm will cook a VESC.

[quote="Shoobee, post:44, topic:51004"]
do I need 190kv for all around better?
[/quote]

 No, there is not a magic kv for all-around better

[quote="Shoobee, post:44, topic:51004"]
do I need 190kv
[/quote]

Probably, for your 9S voltage that's good.  Try using [a calculator](http://calc.esk8.today/advanced/) and get the max speed around 27mph and the max erpm around 45,000 to 55,000.  If it goes over 60k you will cook your ESC if it's VESC4-based.  Adjust the kv and the pulley ratio to do this.  Start with 15/36 pulleys
```

---
## \#3 Posted by: pat.speed Posted at: 2018-04-03T23:40:11.592Z Reads: 90

```
Hi Andrew, with your current setup you will be hitting somewhere around 55km/h. Now don’t get me wrong this setup will work just fine on the esc you have but most likely not very well on a Vesc as of the erpm limit. 

Now if you were to switch to a 190kv motor your top speed would be around 40km/h (I am just using 15/36 gearing and 90mm wheels as a reference). And you would be well under the erpm limits of the Vesc. 

Option number 2 with the 190kV motor is obviously the better choice but 1 will still work and you might as well try that first if you have the parts for it already. If you choose to lower the motor kV to 190 there are a few good options out there such as @torqueboards motors, @JLabs’s, Ollin’s and then some cheaper but well used and reliable hobby motors like the Sk3 motor range and even the Keda motors are proving to very good considering the price. (I have used keda motors on both of my builds and they are rock solid. One of my mates ran the board into a concrete block at 30-40kmh because he forgot that the range drops out after a while so he had no brakes to stop it again, all that happened were some minor marks and scratches.

 Good luck with your build mate


@Namasaki could you or someone else please split this thread into another
```

---
## \#4 Posted by: Shoobee Posted at: 2018-04-04T00:16:28.636Z Reads: 81

```
@pat.speed Dude, you rock! looking into your recommendations now.
I will be trying this out tomorrow. 

collections/esc-speed-controller/products/torqueboards-12s-120a-car-esc-opto-hv.

To recap, I should only use 2 of 3s 5000mah 30c batteries.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-04-04T02:44:41.298Z Reads: 65

```
Spot on, if your using a vesc go with 9s and 190ish kV. The other option is 6s with 270 kV on vesc or lastly 9s and 270kV on an esc other than a vesc
```

---
## \#6 Posted by: Namasaki Posted at: 2018-04-04T04:41:09.836Z Reads: 52

```
[quote="pat.speed, post:3, topic:51179"]
@Namasaki could you or someone else please split this thread into another
[/quote]

Done......
```

---
## \#7 Posted by: pat.speed Posted at: 2018-04-04T04:42:25.348Z Reads: 49

```
Thanks, didn't want to derail the other thread
```

---
## \#8 Posted by: Shoobee Posted at: 2018-04-04T22:54:14.696Z Reads: 28

```
So, 9s works with the esc linked.

collections/esc-speed-controller/products/torqueboards-12s-120a-car-esc-opto-hv

As you mentioned wont that burn out the motor or esc with to high of an erpm?
```

---
## \#9 Posted by: pat.speed Posted at: 2018-04-05T00:00:29.787Z Reads: 23

```
That will work perfectly fine, even on 12s. Only the Vesc has an erpm limit, the one linked is just a standard esc
```

---
## \#10 Posted by: pat.speed Posted at: 2018-04-05T00:09:40.194Z Reads: 21

```
Looking at it, it would almost be cheaper for you to buy a vesc and 190kv motor, search HobbyKing for 190kV or 192kV motors they have some great prices
```

---
## \#11 Posted by: Shoobee Posted at: 2018-04-09T22:22:34.267Z Reads: 18

```
Thank you very much for your help Pat!
```

---

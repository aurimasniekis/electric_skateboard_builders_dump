# Electric skate/bike Dyno build

### Replies: 2 Views: 1167

## \#1 Posted by: jacobbloy Posted at: 2016-05-12T11:59:55.855Z Reads: 118

```
Hi guys so I have been looking into making a Dyno for some time, it will allow me to get really accurate measurements on improvements I make on my hubs and fine tune and compare lots of different outrunner a. I'm posting to get feed back and build ideas. I have done some mods and simulations in bldc tool but wanted some thing proven to be accurate. 
As I'm in Australia I have chosen to go for this system http://www.dtec.net.au

I'm planing to make a braking Dyno as the vesc has great control over braking so I can get a really accurate torque, amp and heat measurements.
I will have the first vesc providing braking current to a big 12090 motor (allows me to test big motors and ebikes)
And the second vesc spinning the motor we are testing at a set rpm, as I increase the braking current on the 12090 the vesc will push more current into the test motor until current limits kickin or it reaches 0 rpm.

The 12090 will have a nice big 200kg s type load cell connected to it to read the force the test motor will be applying. This is done by having the 12090 on bearings so if the 12090 is braking and the test motor is trying to spin it then the whole 12090 will rotate on the bearings not just the shaft and outside rotor.
The mounts of the 12090 will be mounted to a torque arm and then to the load cell to stop it from rotating and provide the force reading.

While this is happening the Dyno hardware and software will be reading the load cell data though a load cell amplifier, plus test motor rpm, temp, amps and voltage to provide accurate data. It will even take into consideration weather and humidity.

I have every thing in hand now to get started I just have to build it.

<img src="/uploads/db1493/original/2X/1/197108f8caed2a700e4e14f77ac34d63443ae847.jpeg" width="666" height="500">

This a video of basically I will be doing but with a lot more data recorded. The raptor being the 12090 and my hub being any test motor or ebike.
https://youtu.be/HP8Nk9So_O0

Here are some photos of my plans and of other applications using a alternator and a car disk break but it is all the same method.

 <img src="/uploads/db1493/original/2X/e/e17a5e959f9e6fa563d5edc660642832633a0a1b.jpeg" width="353" height="500">

<img src="/uploads/db1493/original/2X/2/2aada47dfc39a71fd2a2d2b64043db6a508efa1e.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/8/89ea4653eb6b4c0e5ecde68d288778d0d514bc33.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/b/be9e15d39e5d9bcc940f8ceac54a55c4c2b4b848.jpeg" width="666" height="500">
```

---
## \#2 Posted by: EnderWiggin Posted at: 2017-04-03T18:12:01.794Z Reads: 37

```
i am also interested in makeing a dyno. Any updates?
```

---

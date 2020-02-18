# Dual VESC need help!

### Replies: 11 Views: 925

## \#1 Posted by: Donson Posted at: 2017-12-14T01:08:00.826Z Reads: 148

```
Hey builders

i m a swiss german dude and i need help......
i have my 2 vescs over ppm and canbus....... one is selected 0 one 1 and slave is ¨send over canbus¨ 
after i change to normal settings, just one vesc worked
now i have  connected bouth vescs over pwm signal and it work but not  synchron is the german word... i dont know in english .....

have someone the same problem?

<img src="/uploads/db1493/original/3X/8/a/8adf5d0842631559224e48b5208b17466f55b581.jpg" width="281" height="499">
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-14T01:13:37.687Z Reads: 133

```
Using split ppm to control dual vesc.
They will not be perfectly synced but it will be unnoticeable when riding.
You will only notice it if you start the motors slowly with no load.
Split ppm is a more reliable method than Canbus.
If you decide to run canbus, make sure the cable is very secure and won't shake loose with vibration.
There is a certain way to set up for canbus and I can't remember what it is.
Maybe someone else can chime in and give you the low down.

As for me and my house, we use split ppm...
```

---
## \#3 Posted by: Donson Posted at: 2017-12-14T01:31:19.415Z Reads: 124

```
now i have from 60A to 20A motor max....... hit me two times on the foor lol
thx dude i try this tomorow<img src="/uploads/db1493/original/3X/c/7/c7f293b50a64c8e05e2bbcc84113bd41f053bd01.jpg" width="281" height="500">
```

---
## \#4 Posted by: Donson Posted at: 2017-12-14T01:33:17.686Z Reads: 114

```
were is split ppm? one vesc is with pins one is sodered..... i can try soder the 2. to
```

---
## \#5 Posted by: Namasaki Posted at: 2017-12-14T01:38:49.254Z Reads: 112

```
Split ppm means you get a Y signal cable to connect both vescs to one receiver. Each vesc is setup individually as a master.
They both receive the same signal from the receiver but work independently of each other.
When using this method it is important that you run the red 5v+ wire of the signal cable to only one vesc.
```

---
## \#6 Posted by: Donson Posted at: 2017-12-14T01:48:12.276Z Reads: 105

```
now i have ch1 and ch2 over pwm signal one vesc is ch1 one ch2.......
is this the problem?
```

---
## \#7 Posted by: Donson Posted at: 2017-12-14T01:52:44.971Z Reads: 101

```
<img src="/uploads/db1493/original/3X/2/2/22045fc54e5ea62df438574ad14a49397138f680.jpeg" width="281" height="500">
```

---
## \#8 Posted by: cwazy1 Posted at: 2017-12-14T06:00:57.329Z Reads: 86

```
[quote="Donson, post:6, topic:40973, full:true"]
now i have ch1 and ch2 over pwm signal one vesc is ch1 one ch2.......
is this the problem?
[/quote]

no. thats not what split ppm is..
```

---
## \#9 Posted by: Namasaki Posted at: 2017-12-14T18:38:49.238Z Reads: 71

```
[quote="Donson, post:6, topic:40973, full:true"]
now i have ch1 and ch2 over pwm signal one vesc is ch1 one ch2.......
is this the problem?
[/quote]

That won’t work. 
You need a  Y cable to connect both Vescs to channel 2
```

---
## \#10 Posted by: bigben Posted at: 2017-12-14T18:47:50.945Z Reads: 69

```
Or two receivers paired to the same remote?
<img src="/uploads/db1493/original/3X/4/6/4620fc2c56e7f0750e212eeda55a1fb91c729275.JPG" width="375" height="500">
```

---
## \#11 Posted by: Donson Posted at: 2017-12-20T22:53:51.710Z Reads: 53

```
now i have a Wii nunchuk..... but i dont know if the pins are right.... 

<img src="/uploads/db1493/original/3X/d/3/d32cf359871a8bcb13aeff8ab965cdcfd55db1f6.jpg" width="281" height="499">
```

---

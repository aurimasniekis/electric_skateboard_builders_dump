# Any ideas what this is?

### Replies: 13 Views: 571

## \#1 Posted by: Hatman30 Posted at: 2018-03-24T13:54:09.267Z Reads: 172

```
Picked up some old ollin stuff- vesc etc and wondered what this was? It looks to me like a receiver with aerial lead but wondered why it’s got a push button and what the three wires coming out of it were for? Any help appreciated thx ![image|375x500](upload://pzcy0U12TbQX6ZpSllqxkF98Th0.jpeg)
```

---
## \#2 Posted by: Hatman30 Posted at: 2018-03-24T14:02:58.421Z Reads: 158

```
![image|375x500](upload://p9dVqR0udA8rO1tNnIp6tZ8XOcs.jpeg)
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-03-24T14:09:19.700Z Reads: 150

```
is that unhardened jb weld?
```

---
## \#4 Posted by: telnoi Posted at: 2018-03-24T16:18:36.053Z Reads: 128

```
5v in or out, push button would be bind/failsafe.
```

---
## \#5 Posted by: Hatman30 Posted at: 2018-03-24T16:41:43.015Z Reads: 119

```
Nice one 👍
```

---
## \#6 Posted by: telnoi Posted at: 2018-03-24T16:42:45.752Z Reads: 119

```
Forgot, yellow/orange.. The light color is ppm.
```

---
## \#7 Posted by: goldenHusky Posted at: 2018-03-24T17:53:21.224Z Reads: 96

```
I did some research and believe this is an onboard glow driver.
It is basically a constant current switching regulator used to power leds e.g. of a powerswitch

Edit: But this only makes limited sense to me since the vesc has a 5V output.. 
https://hobbyking.com/en_us/hobbyking-on-board-glowdriver-v2.html?countrycode=EU&utm_source=criteo&utm_medium=cpc&utm_campaign=eu
```

---
## \#8 Posted by: ZackoryCramer Posted at: 2018-03-24T18:42:42.863Z Reads: 79

```
I think it's called UBEC(Universal Battery Eliminator Circuit) for short. It's to replace the 5v voltage regulator which gives off as much heat as the energy it outputs.
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-03-24T18:57:26.828Z Reads: 62

```
the 5v on the vesc is unreliable because it comes from the DRV
```

---
## \#10 Posted by: Hatman30 Posted at: 2018-03-24T19:00:10.455Z Reads: 58

```
What would that be doing on an old school ollin Board though ? Usb power ?
```

---
## \#11 Posted by: Hatman30 Posted at: 2018-03-24T19:00:44.852Z Reads: 57

```
It looks like it has an antenna cable on it as well as it comes off the ppm output of the vesc
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-03-24T19:06:25.794Z Reads: 53

```
could be a ppm switch (plugs into reciever to switch power on/off to external sources)
```

---
## \#13 Posted by: ZackoryCramer Posted at: 2018-03-24T19:20:35.825Z Reads: 50

```
The leds and other computing chip probably doesn't have a input range of 6~12s. :stuck_out_tongue_winking_eye:
```

---

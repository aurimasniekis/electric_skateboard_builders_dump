# Help diagnose a damaged vesc. How to test FETs?

### Replies: 15 Views: 1480

## \#1 Posted by: lrdesigns Posted at: 2017-06-20T01:53:41.133Z Reads: 145

```
Hi guys I have a vesc that got a little wet. Its inside a lunch box but it leaks a little bit. The vesc itself was 90% covered in hot glue so I think it might be fixable as most of it seems ok. I didnt cover the connectors and one of the FETS was not completely covered. 

This is the symptoms.

* No power going to motor. 
* No error messages.
* All other functions seem normal. Lights normal. If I conned to BLDC all is normal. If I spin the wheel I get telemetry feed back of the rotation and see some amp detection. The PPM visual is working normal.

My current theory is a blown FET. My question is how can I test the FET's to see if they are normal?
```

---
## \#2 Posted by: Martinsp Posted at: 2017-06-20T05:48:06.917Z Reads: 139

```
Hey! 
We will definitely need pictures to help you! Also from what you wrote so far i would first start with some basic measurements with multimeter... there should be no short between + and - and also between +,- and all of the phases there should be no short. 
Especially check the mosfet that was not cowered. If you are going to replace it you should check the gate resistor because it tends to go with blown mosfet...
hope that helps! :)
```

---
## \#3 Posted by: lrdesigns Posted at: 2017-06-21T02:48:19.616Z Reads: 132

```
Thanks for the tips. Removing it from my board was not easy, then I spend an age peeling of the hot glue. 
<img src="/uploads/db1493/original/3X/a/1/a17312e8ac180ec5fe8840560b9cd552e88a47bb.jpeg" width="666" height="500">

I tested the shorts as you suggested, but no shorts. Still more cleaning to do before I can measure the fets and gate resistors. But I found the main issue. The old goldie, blown DRV. Is it weird there is no error message when I pug it in to BLDC? Is there any other components I should test? 

Small burnt spot and that smell. :confounded:
<img src="/uploads/db1493/original/3X/2/a/2a43da8be67826e52a89d283a9ab26b19fad5e78.png" width="437" height="500">
```

---
## \#4 Posted by: Martinsp Posted at: 2017-06-21T05:54:44.512Z Reads: 122

```
Oh wow :D well then it is a dead giveaway :D 
I dont know how exactly the vesc works when plugged in but i would imagine that the CPU is communicating with your PC and as long as you are not trying to do a motor detection or spin the motor it is not checking the DRV for errors.. I might be wrong though.
The next thing i would do is order (more than 1) and replace the DRV but before you even turn it on try diagnose what was the reason that the DRV blew... You say it got water damage that could mean that the water shorted something and sent high voltage to the DRV hence the burn mark so i would check resistors (you cant measure value in circuit but that is not important... you want to know if the resistor is good so if it has any resistace between its contact points... dead short  ohms is bad and infinite resistance is bad because that could mean that the resistor is not conducting any electricity at all therefore might cause malfunction). Also check capacitors especially the big ones.. if they are shorted they need replacing (if you dont have an expensive multimeter it wont have capacitor checking or measuring its value option.. it is ok you can check a capacitors in diode mode). All of this is not really necessary to do on all parts but only on the ones connected to DRV based on chematic. 
And last thing is checking the actual PCB itself... if it has any obvious damage like burn marks there is a chance that the PCB got fried due to the short because of water... hope not.

Sorry for the long post but I thik that I would rather spend more time diagnosing rather than burn another DRV or possibly worse :D Wish you the best of luck with all this...
 If you wont find anything wrong it is pretty safe to say that you can plug the VESC in without worries :slight_smile:
```

---
## \#5 Posted by: Martinsp Posted at: 2017-06-23T18:18:46.035Z Reads: 99

```
Hey! So how did your troubleshooting go?
```

---
## \#6 Posted by: lrdesigns Posted at: 2017-06-25T02:56:20.761Z Reads: 95

```
Well I got it clean and all the traces look good and the gate resistors are ok. But I don't really understand how to test the fets with the diode mode on my multimeter. I decided to buy a new vesc and keep this as a spare and try to do the drv replacement myself. 

<img src="/uploads/db1493/original/3X/c/2/c220ee6d477561fa1392a4a0f534e0b04264ffb6.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/5/a56695d8a0faaad98657a65804840bf2b380ebf1.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/2/e28d362c3fa9e2ded73cf2e71b45e0119de7715f.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/3/e/3e01428d0f117db41d7f75e68ccf31028c65dab9.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/a/e/aebe4d3190a228c5bf08a70c45e00346ddeacd32.jpg" width="375" height="500">
```

---
## \#7 Posted by: Martinsp Posted at: 2017-06-25T09:40:12.816Z Reads: 86

```
I measure mine based on this video https://www.youtube.com/watch?v=RkWy1EirEu8 
hope that helps... if you dont care about the vesc that much now you could just try to replace the DRV and see what happens... it is not all that expensive after all and there is a high chance that if the fets are good that it will work just fine with new drv
```

---
## \#8 Posted by: lrdesigns Posted at: 2017-07-05T02:31:52.779Z Reads: 83

```
Yeah I watched it several times and tested the fet's but was always confused by the results. I'm not sure the same test can be done with the fet's mounted in the PCB. I couldn't get  them to turn off by touching the legs. 

I got the new vesc replacement so at least I could test that and compare the results to the burnt one. With the new one when I test the drain to source the voltage quickly rises up 1.9volts then it switches off. Same for all fet's. 

On the burnt one the top side does the same rises to 1.9 then turns off. But the bottom side fet's rise slowly to around 1.5 volts but don't turn of they just hover around this constant voltage. So there is some difference but Im still not sure its a clear cut case. 

I think the only true way is to remove the fet's and test them on thier own?
```

---
## \#9 Posted by: lrdesigns Posted at: 2017-07-12T03:46:24.510Z Reads: 76

```
I still have not found an answer to weather the FETs need to be removed or not to be properly tested? 

On the plus side I received some DRVs in the mail, I gotta buy a hot air gun now :smirk: Thinking of getting this cheap one [YOUYUE 858D+](https://www.aliexpress.com/store/product/700W-Hot-Air-Gun-YOUYUE-858D-220V-ESD-unlead-adjust-temperature-Soldering-Station-Welding-gun-LED/703284_32797600905.html?spm=2114.12010615.0.0.a4IKl3)  

<img src="/uploads/db1493/original/3X/5/e/5ecbe3af9fe923dfc19d393a9d67225351f65000.jpeg" width="375" height="500">
```

---
## \#10 Posted by: Eboosted Posted at: 2017-07-12T03:53:59.763Z Reads: 75

```
Where did you buy the DRVs from?
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-12T03:56:08.104Z Reads: 75

```
Not sure about testing the FETs I've tested BJTs before but really not sure if those can be tested in circuit or not either I just had them from some breadboarding making a little amplifier for fun and learning.  Think in general it's better to remove them for testing, think the MOSFETs are actually one of the easier components to remove hard part is not accidentally taking anything with them and then getting them lined up and put back on correctly.  Regarding the DRV chips I got a cheapo hot air rework station too and gave it a go on one board I had fried by shorting it with voltmeter leads.  Unfortunately, the patient died during surgery and had to be put to rest on the shelf.

---

Can use some solder wick to get most of the solder up off the MOSFETs then the hot air gun works well for heating up the area around them and getting them to come loose (but need to avoid blasting anything else loose so need to get the air flow and angle and all right to not blast other components off or cook yourself)
```

---
## \#12 Posted by: lrdesigns Posted at: 2017-07-12T04:03:15.064Z Reads: 70

```
[quote="Eboosted, post:10, topic:25734, full:true"]
Where did you buy the DRVs from?
[/quote]

Sorry not sure, a friend helped me buy them from tao bao for $2.1 usd a piece :astonished:
```

---
## \#13 Posted by: lrdesigns Posted at: 2017-07-12T04:05:12.024Z Reads: 70

```
[quote="wafflejock, post:11, topic:25734"]
Unfortunately, the patient died during surgery and had to be put to rest on the shelf.
[/quote]

:cry::cry::cry::sob::sob::sob::sob::sob::sob::sob::sob::sob::sob::sob::sob::sob: Sorry for your loss.
```

---
## \#14 Posted by: wafflejock Posted at: 2017-07-12T04:06:31.907Z Reads: 66

```
Yeah it's alright was the first time I had tried any SMD rework and wasn't really expecting a positive outcome was more a learning experience on that one while I waited on a new VESC
```

---
## \#15 Posted by: JdogAwesome Posted at: 2017-07-12T04:50:01.863Z Reads: 66

```
You should never rely on that results from a component that's connected, it can completely skue your test results. Only way to test properly is to remove it from the circuit. 

Like a @wafflejock said the FET's shouldn't be hard to replace, though it seems everyone is having a 7530 shortage, Mouser Digikey and Arrow all seem to be either out of stock or on backorder, Mouser has like 11K on backorder! Also I got the same 858D+ hot air station off eBay for $30 US shipping and it's worked very well so far!

EDIT: I actually just replaced 2 FET's on a VESC and you can actually test if they have a drain to source short fine while there on the PCB. Though thats about the only thing you can test reliably on the PCB. Some resistors I tested fine like the gate 4.7Ohm ones which 3 of the 6 were dead and needed replacing.
```

---

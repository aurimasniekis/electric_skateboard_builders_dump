# Motor spinning on own help please

### Replies: 28 Views: 1251

## \#1 Posted by: Exiledd_Top Posted at: 2017-08-13T04:46:33.478Z Reads: 138

```
YESS Hello have allmost finished my build after months of waiting i just got the batteries they were not fully changed but at the same voltage 3.8, i have downloaded the bldc tool for the vesc but i believe it doesnt work with my esc i have the torque boards 120amp esc for 12s and i connected in to the bldc and it says connected for a second and then says firmware not detected , second i have checked all cables and everything everything is fine but when i insert my loop key my motors dont respond at all , then after a few seconds (10) i just move it back and foward the controll and then one motor starts spining and then stops and then they both start spining on there own . i dont know whats wrong can somehelp
```

---
## \#2 Posted by: Exiledd_Top Posted at: 2017-08-13T04:55:32.259Z Reads: 130

```
https://www.youtube.com/watch?v=BjRSOZKbitM
heres a video showing the problem
```

---
## \#3 Posted by: jammin Posted at: 2017-08-13T05:15:36.143Z Reads: 121

```
alrighty, it's hard to see with that lighting but I have some ideas. That looks like a car ESC; unless that's a VESC then you'll need an programming card for it. Are you not using a car ESC programming card or am I mistaken?

I'm guessing that your PPM is off because your motors aren't going into full throttle (and you're still able to control it), meaning that the resting position for your remote is actually telling the ESC to give the motors some juice. Not sure how to fix that on the car ESCs, but I'll try to look around.

The pause from connecting the anti-spark plug -> motors spinning is pretty normal (the ESC has to boot, just like any other computer / microcontroller).
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2017-08-13T05:20:34.002Z Reads: 113

```
I am using this exact esc diy-electric-skateboard-kits-parts/torqueboards-12s-120a-car-esc-opto-hv/
Also one of them has a ubec soderd onto the cable and to connoted the cables for remotes it's two y connectors into one ,I do have the programming box thing I programmed them both to exact everything but am very limited on what I can program , I used this vidoe as a guide https://youtu.be/M-Q4oku_LPk
```

---
## \#5 Posted by: jammin Posted at: 2017-08-13T05:38:54.719Z Reads: 102

```
hmm, what's the 'firmware not detected' error you were getting earlier? Sorry for my confusion but your first post you mentioned both the VESC and your car ESC.
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2017-08-13T06:06:21.993Z Reads: 97

```
I'd click "connect " on the bldc program and I'd say connected and then I forgot because I did it hours ago and am not home but would say something like "firmware not recongonized"or " firmware error" the esc programming card has a USB to connect to computer is what it says advertised but didn't connect
```

---
## \#7 Posted by: cdn Posted at: 2017-08-13T06:07:37.290Z Reads: 91

```
Seems like everything is connected correctly if the motors spin. Torque boards 12s esc's can only be programmed with the programming card. The problem you have is you have to get another remote that has a trimming function on it. Either get the hkgt2b or the mini. Both have trim adjustments. Once adjusted it will stop the motors from spinning when remote is turned on.
```

---
## \#8 Posted by: Exiledd_Top Posted at: 2017-08-13T06:09:59.381Z Reads: 88

```
Whatttt I have to buy another remote boi.... are you sure it's the remote , the remote was quite exspensive ... I have enertions new remote what I heard there pretty reliable for small remotes unlike the rest that's why I went with them .....
```

---
## \#9 Posted by: cdn Posted at: 2017-08-13T06:20:26.292Z Reads: 84

```
Yes, you have to get another remote. I had the same problem using torqueboards 12s esc and paired with the nano style remote. I ended up getting the hkgt2b in a modded master cho case.The nano style remotes don't have a trim function. Your cheapest most reliable option is getting the mini style remote. They can be found on eBay for around $20.
```

---
## \#10 Posted by: Tuomalar Posted at: 2017-08-13T06:23:49.213Z Reads: 80

```
This is ESC and bldc tool is made for VESC (vedders esc) so you can't program that hv opto with bldc tool.
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2017-08-13T06:25:11.512Z Reads: 77

```
Can you confirm the remote theory I feel bummed I wasted 100$ on a remote I can use :(
```

---
## \#12 Posted by: i2oadsweepei2 Posted at: 2017-08-13T10:11:08.742Z Reads: 74

```
There is a neutral position setting on those esc's. You could try setting it to the largest number. I think it's 9 or 7 can't remember off the top. This should make the neutral point a bit bigger and might stop the motor spinning on startup. Also with the nano-x you need to set the end points every time you turn it on. Turn the remote on first then move to full throttle then full brake a few times and then turn on the board. Not sure if any of this will help, but I hope it does.

Good luck.
```

---
## \#13 Posted by: Exiledd_Top Posted at: 2017-08-14T06:32:50.241Z Reads: 54

```
Hey yes I did that and it worked BUT FOR ONE THE MOTORS ONLY , I thought it was the motor or connection or something but it I checked every cable and connection side and everything the same , so I switched esc and then the other motor was fine but it switched I have narrowed it down by that to the esc but I have already put that nuetral range to 9% here's a vidoe https://youtu.be/9YnYWWa7l1g
```

---
## \#14 Posted by: StormTrooperBert Posted at: 2017-09-07T04:11:45.178Z Reads: 48

```
I'm running DIY VESC with an sk3 6374 6s 5000 mah zippy and my motor started spinning/stuttering on its own. It was working just fine for about 6 miles or so. No DRV errors no loose connections. Help!! Note. YES I have used the search functions.
```

---
## \#15 Posted by: Exiledd_Top Posted at: 2017-09-07T06:35:54.636Z Reads: 44

```
Controller maybe it's the controller like the issue I had the vesc that you probably got like one of mine is very sensitive and having a controller like from torqemboards or enertion that are not spring loaded are making your motor spin get the gt2b and yes I left a 110$ remote for a 20$ one but it works so hey give it a go
```

---
## \#16 Posted by: StormTrooperBert Posted at: 2017-09-07T06:46:35.894Z Reads: 42

```
Couldn't I just reprogram neutral position in BLDC Tool if that was the case?
```

---
## \#17 Posted by: StormTrooperBert Posted at: 2017-09-07T16:40:21.567Z Reads: 35

```
@torqueboards hey could anyone chime in here? Motornisnspinning onnitsnown in neutral position all of a sudden. I'm using your guys' nano remote and VESC. Could I just program a new neutral position in BLDC? If so how would I do that? If I pull SLIGHTLY back it stops. But when I let go, white light indicating signal input turn on, on VESC and motor spins :(
```

---
## \#18 Posted by: Exiledd_Top Posted at: 2017-09-07T19:06:01.342Z Reads: 29

```
As I said it's either the remote or the vesc or a combination of both like mine my vesc is at max neutral range would work for a bit then motor start spinning on its on, you probably got a sensitive vesc and need a spring loaded remote that is not like enertion or torqueboards get a mini or gt2b cheap 20$ and test it yourself
```

---
## \#19 Posted by: Tomash Posted at: 2017-09-07T19:16:22.211Z Reads: 28

```
@StormTrooperBert i had similar "thing" when i first connected, remote (I have Alien Power remote) to the VESC.

If you have VESC, and you use PPM control mode, you can adjust the throttle in the PPM Tab in BLDC tool.

The guy in [THIS Youtube Video](https://www.youtube.com/watch?v=OtuofrQr3F8&t=188s&index=28&list=PL066A6DA0AEB45257) explain how to adjust throttle range in BLDC tool.

When i did that, my motor didnt spin anymore on its own.
```

---
## \#20 Posted by: StormTrooperBert Posted at: 2017-09-07T19:25:27.517Z Reads: 27

```
Thank you I'll definitely give this a try. I'm just in denial that I would have to all of a sudden replace my $60 perfectly functioning remote. Ive ridden this setup for miles with zero issues. I hope it's a just a matter of neutral position recalibration. Thanks you both! Will update once looked into.
```

---
## \#21 Posted by: Exiledd_Top Posted at: 2017-09-07T19:27:40.749Z Reads: 27

```
I did that with my enertion remote wasted 110$ and then bought a 20$ remote I DID THAT and it solved my issue I allreadyyy tried programming it several times to make nuetral range at Max, u didn't state that you have ridden this several times ._. I thought this was first time assembly like my situation
```

---
## \#22 Posted by: Sn4pz Posted at: 2017-09-07T21:30:05.572Z Reads: 23

```
im not sure what remote youre using, and my laptop doesnt like to play some videos ( not sure why, i really dont mind ) but something that happens with me is i drop my remote, and the motors start to go on their own. I fix this by opening up the remote and adjusting the spring that is pushed by the trigger. I have the torqueboards regular remote and that fixes it 100% of the time. Not sure if thats the issue, but it could be worth your time to have it touched up on.
```

---
## \#23 Posted by: StormTrooperBert Posted at: 2017-09-07T21:48:04.319Z Reads: 22

```
That's a great idea I will definitely look into this. Will post results tonight.
```

---
## \#24 Posted by: StormTrooperBert Posted at: 2017-09-07T23:02:47.079Z Reads: 20

```
@Sn4pz I did fall the other day but didn't think anything got damaged or out of alignment with the remote because it was working fine for another 5 miles or so. Must've been right there at the cusp. Hmm. Will definitely open up the remote to see if there's a spring adjustment.
```

---
## \#25 Posted by: Sn4pz Posted at: 2017-09-08T00:55:49.476Z Reads: 21

```
its worth a shot :o
```

---
## \#26 Posted by: StormTrooperBert Posted at: 2017-09-08T04:07:32.106Z Reads: 21

```
MOTHA FUCKIN UPDATE plugged into BLDC and wiped everything clean. Started from scratch. Adjusted my max throttle/brake travel and VOÍLA no more motor stutter/ghost spinning. Don't know what happened but I'm sure glad everything is working as it should. i opened up my Torqueboards nano transmitter and there was no adjustment spring though but the tip was much appreciated. Later gonna go shred Las Vegas ✌🏽 Thank you again @Sn4pz !!
```

---
## \#27 Posted by: StormTrooperBert Posted at: 2017-09-08T04:09:13.131Z Reads: 19

```
@Tomash thank you for the advice this is exaclty what I did and presto! I'm so happy it wasn't a drv code. I've already fried a brand new VESC somehow. Didn't even have 1 ride one it. Live and learn.
```

---
## \#28 Posted by: StormTrooperBert Posted at: 2017-09-08T04:17:08.022Z Reads: 20

```
Spent two hours figuring this out FINALLY fixing it. Then it fuckin rains. 😐
```

---

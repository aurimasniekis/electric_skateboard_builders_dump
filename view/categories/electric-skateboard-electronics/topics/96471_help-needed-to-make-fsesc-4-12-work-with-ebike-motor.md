# Help needed to make FSESC 4.12 work with eBike Motor

### Replies: 9 Views: 300

## \#1 Posted by: Chupacabra Posted at: 2019-06-12T23:44:40.879Z Reads: 56

```
Hi Guys,

I'm trying to make this motor work with a Flipsky 4.12 VESC 50 amps. I am running a 52 Volt battery on it. However when i connect the motors I get a motor detection failed error during the VESC setup. I have tried using both the Ackmaniak and the latest Vedder VESC tool.

Here is a link to the motor
https://www.aliexpress.com/item/KUNRAY-MY1020-48V-DC-2000W-Electric-Brushless-Motor-5400RPM-Electric-Scooter-E-Bike-Electric-Bicycle-Motorcycle/32859790697.html

Link to the whole set.
https://www.amazon.com/dp/B07KR2FN89?ref=ppx_pop_mob_ap_share&amp;fbclid=IwAR0gSpWUksSjoyOeh2Nj7MUA9R58y6XhmtsPN09v-uYyFnIDXjKdl0TTxAc

Does anyone have any experience in working  a vesc with a E-bike motor? I'd really appreciate any and all help.
```

---
## \#2 Posted by: Silverline Posted at: 2019-06-13T06:09:12.055Z Reads: 40

```
Just build an drift Trike, around an e-bike hub motor and the vesc6. If i where you, I would buy the vesc 6 Style over vesc 4.12. 50amp is not much, on these motors.... I have set mine Up for 100a and want more 😃

Are you choosing the right motor in the newest vesc tool ? It has to be the e-bike 6kg option, or you have to Play around with the testing values. On the old vesc tool, I had to lower the eRPMs quite a bit, and turn Up the amps, in order to get a succesful motor detention. 
Also have you tried in both FOC and BLDC mode, and with and without hall sensors ?
```

---
## \#3 Posted by: Chupacabra Posted at: 2019-06-13T18:00:25.406Z Reads: 31

```
Thanks that’s great info. 

Yes I have tried the motor with the BLDC option only as I still have to figure out how to connect the hall sensors. 

The first option although optimal is not feasible  due to financial constraints . 

I was choosing the inrunner motor >2000 g. option. Lowering the eRPM eh? I never really understood what that did. I’m still using the default values. 

What do you recommend I set my values to ?
```

---
## \#4 Posted by: Chupacabra Posted at: 2019-06-13T18:16:09.699Z Reads: 26

```
Also please see the battery that is being used with this build. 

https://www.amazon.com/dp/B07L55YYZM?ref=ppx_pop_mob_ap_share

The battery actually charges to 58v so I suspect it’s a 14S.
```

---
## \#5 Posted by: Silverline Posted at: 2019-06-13T18:41:33.511Z Reads: 19

```
14s on vesc... Is like playing with fire. Max 12s....

From your link, it says 48v, that normally means 13s. And that is on the edge for the vesc, specially with a big motor like you are using, that could give lot of voltage spikes. 

Try chose the bigger motor option, when you do a motor detention.
```

---
## \#6 Posted by: Chupacabra Posted at: 2019-06-13T18:57:10.984Z Reads: 19

```
But the largest option in the vesc tool is only >2000 gms. Can you recommend some values to try for the ERPM and amps?
```

---
## \#7 Posted by: Silverline Posted at: 2019-06-13T19:30:51.703Z Reads: 19

```
Dont you have this option for e-bike motor ?
![IMG_20190613_212908997|281x500](upload://2KS3wj0Kr4X0Dd9KdOCSNOhYsvm.jpeg)

In the old vesc tool.... I set the test Amp (I) to 10amp and rpms to 200. This is on vesc 6. Maybe the old vesc 4.12 is a different story.
```

---
## \#8 Posted by: Chupacabra Posted at: 2019-06-13T19:34:39.489Z Reads: 18

```
Yes there is! I just never tried it because it says hub motor.
```

---
## \#9 Posted by: Silverline Posted at: 2019-06-13T19:35:34.440Z Reads: 18

```
Yeah , give it a try. Not everything is obvious in the new GUI imo.

If its not working, i think you have to Play with the test values.... One step at a time
```

---

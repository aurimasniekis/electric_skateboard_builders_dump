# Circuitry Help Please!

### Replies: 21 Views: 2203

## \#1 Posted by: NewtoThis Posted at: 2016-11-14T05:40:31.406Z Reads: 116

```
<img src="/uploads/db1493/original/3X/c/9/c96a8316f251381c6e59c13c3b4893a6bca61201.png" width="690" height="276">
I'm new to electronics and batteries and such and i was wondering if i have the right idea or if i am heading down the wrong path with my circuit plan. My goal in this circuit is to have a primary set of batteries in series to get 10 cells, and then have a secondary battery that i can turn on when the first two are out of juice to get further range. I'd appreciate any criticism that can make this more efficient or prevent explosions if its horribly messed up.
```

---
## \#2 Posted by: DilatedPupils Posted at: 2016-11-14T06:13:27.652Z Reads: 104

```
In your diagram you only have 3 batteries.
What are your batteries?
3 5s batteries?
```

---
## \#3 Posted by: NewtoThis Posted at: 2016-11-14T06:40:00.446Z Reads: 97

```
i have 3x 8000mah 5s batteries. im hoping for the first two to be in series for more voltage and the the third to be a separate battery that will give me some extra range if i need it. i got the idea from 
http://www.instructables.com/id/Make-Your-Own-Electric-Motorized-Longboard/?ALLSTEPS
with this diagram;
<img src="/uploads/db1493/original/3X/3/c/3c68949622dc9ce2bb776ffc8aa47a65533cfda1.png" width="690" height="297">
```

---
## \#4 Posted by: NewtoThis Posted at: 2016-11-14T06:43:21.181Z Reads: 92

```
Also, they have a discharge rating of "30c"... not sure if that has any relevance.
Here is a link to where i got them: 
https://hobbyking.com/en_us/zippy-flightmax-8000mah-5s1p-30c.html
```

---
## \#5 Posted by: DilatedPupils Posted at: 2016-11-14T06:58:08.883Z Reads: 92

```
You can't have 10s as a primary and 5s as a reserve. If you wanna do this, you would need 1 more 5s battery to make your reserve 10s as well.
And based on your diagram, you have the 2 5s in parallel, not in series.
```

---
## \#6 Posted by: NewtoThis Posted at: 2016-11-14T07:17:31.053Z Reads: 86

```
oops my bad. Would you suggest series or parallel for the first two batteries if im going for a good balance of speed and range? Also, i was wondering if the 5s batteries will work with these (https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html) motors that i have. main reason being that on the website it specifies that the motors need "Voltage: 8~10S Lipoly" which made me think i need to double the voltage of my current batteries.
```

---
## \#7 Posted by: ch3m1st Posted at: 2016-11-14T18:38:29.902Z Reads: 63

```
Wiring your two primary batteries in series will give you the 10S your sk3 motor is looking for, but I'm not sure if you can run a 5S backup. I guess that would depend on your vesc/esc settings?
```

---
## \#8 Posted by: NewtoThis Posted at: 2016-11-14T20:47:23.433Z Reads: 48

```
im going to be using two VESCs (v4.12) so i can have a dual motor setup, but im thinking that having a 5s backup is too much of a hassle and might not have a high enough voltage to satisfy both VESCs on its own anyways. Speaking of which, since im using two motors, does that mean that i have to make a 16-20S to satisfy both motors?
```

---
## \#9 Posted by: NewtoThis Posted at: 2016-11-14T21:40:48.715Z Reads: 48

```
Here is a revision of the diagram
the yellow boxes are xt90s and the small rectangles by the batteries are bullet connectors
<img src="/uploads/db1493/original/3X/b/f/bfa0f0b1e9a90f735b508ea3da5dd7d7cc1045af.png" width="690" height="297">
```

---
## \#10 Posted by: Jinra Posted at: 2016-11-14T21:47:13.491Z Reads: 50

```
[quote="NewtoThis, post:8, topic:13034"]
Speaking of which, since im using two motors, does that mean that i have to make a 16-20S to satisfy both motors?
[/quote]

No since the ESCs are connected in parallel, not series. Each ESC/motor gets the same voltage. Your kv is also too high for the VESC. Run 8s max for a 260kv motor or get <200kv motors for your setup.
```

---
## \#11 Posted by: NewtoThis Posted at: 2016-11-15T02:04:54.396Z Reads: 42

```
Is that because of voltage being too high? or is it that the motor will draw too much power? the website says "Voltage: 8V to 60V (Up to 14S LiPo Voltage)". If thats the case then i guess i'll have to just connect the batteries in parallel? Also, could i fix this by placing a limit on the maximum RPM of the motor or some kind of limiting factor?
where i got the VESC (diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/)
```

---
## \#12 Posted by: NewtoThis Posted at: 2016-11-16T06:44:57.919Z Reads: 33

```
[quote="Jinra, post:10, topic:13034, full:true"]

kv is also too high for the VESC. Run 8s max for a 260kv motor or get <200kv motors for your setup.
[/quote]

On the BLDC tool there is an option to set a max rpm or max current. Is that a way to fix this?
```

---
## \#13 Posted by: Jinra Posted at: 2016-11-16T06:58:37.674Z Reads: 34

```
You can limit eRPM, but it's inefficient. You're better off setting up your system right, though you can limit the eRPM if you'd like.
```

---
## \#14 Posted by: NewtoThis Posted at: 2016-11-17T00:13:59.828Z Reads: 30

```
On Vedder's website it says that it features "Voltage: 8V – 60V (Safe for 3S to 12S LiPo)". What i would be running would be a 10s LiPo. It also doesnt specify any sort of maximum kv and almost all sources i came across in my research said any motor under 300kv should be good. Just wondering where the info you have is coming from. Thanks!
http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#15 Posted by: Jinra Posted at: 2016-11-17T00:27:13.680Z Reads: 28

```
it's not a kv limit, is an erpm limit 100k is technically the limit, but the vesc starts having problems after 60k. If you want you can check out the info here.

http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#16 Posted by: NewtoThis Posted at: 2016-11-17T07:32:35.490Z Reads: 24

```
[quote="Jinra, post:15, topic:13034, full:true"]
Run 8s max for a 260kv motor
[/quote]

Since i already have the motors, i have placed an order for a couple 8000mah 4s 30c lipos from hobbyking. Another side question... would it be possible for me to run two 4s batteries in series and 2 4s batteries in parallel in the same circuit to give me 16000mah from the parallel batteries and keep an 8s total voltage from the series batteries? Like this maybe?
<img src="/uploads/db1493/original/3X/e/9/e9c590c34f5dae43f8731dfe978b0fbfb22954b5.png" width="690" height="281">
```

---
## \#17 Posted by: Jinra Posted at: 2016-11-17T07:34:40.092Z Reads: 21

```
Yep that'll work, just consider the weight and extra space of the batteries, not to mention the tediousness of charging 4 packs. You may find yourself content with just the 2x 4s packs. That would get you about 23 km.
```

---
## \#18 Posted by: NewtoThis Posted at: 2016-11-18T04:03:18.956Z Reads: 20

```
Thanks for the info! I have another question; If i were to use multiple batteries as i am planning to, how do i prevent over discharging the batteries? I have a volt-meter that tells me the voltage of each individual cell in a single pack, but this doesnt tell me anything if i use 4 different batteries.
```

---
## \#19 Posted by: Jinra Posted at: 2016-11-18T05:13:50.600Z Reads: 18

```
You can set a low voltage cutoff on the VESC in BLDC tool. I'd recommend a volt/battery meter anyway to visually check.
```

---
## \#20 Posted by: NewtoThis Posted at: 2016-11-18T14:55:34.049Z Reads: 19

```
ok. Here is a revision to the diagram; this should get me 8s 16000mah which should work with my VESC and Motors<img src="/uploads/db1493/original/3X/5/6/56aa58dcb0040faed33e4637f20bd139607fec1d.png" width="690" height="320">
```

---
## \#21 Posted by: NewtoThis Posted at: 2016-11-22T03:57:18.641Z Reads: 16

```
Ok. I have ordered the electronics and they should be here some time in the next few weeks. I will update this post if everything works. thank you for your help!
```

---

# Question about reverse mounting motors

### Replies: 30 Views: 2899

## \#1 Posted by: briman05 Posted at: 2017-12-13T19:40:13.832Z Reads: 328

```
I have been putting together the parts I need to build my board, however one part I'm still having a hard time figuring out mainly because I do not have them yet.  I had planned on using bear trucks that I have laying around and was looking at getting @marcmt88 motor mounts.  After some research I have come to find that the 181mm bear trucks that I had planned on using will not work as a dual setup using the racerstar 5065 motors.  I had looked at getting caliber trucks but they are only 3mm longer then the bears  Would this be enough to have them both on the same truck maybe if I added some speed rings between the hanger and the wheels.  I feel like having a rear drive board would be better then a front drive board.  Another option I have seen is reverse mount hing where one motor is behind the board and the other is underneath the board.  I'm working if that would be the answer that would fix my issue.  But how would you set it up in the BLDC tool because they would be rotating different ways. If there is another option for mounting that will allow me to use the trucks I have  that would be helpful. I tried to search for it before asking but not quite sure what terms to search

Also on a different topic has anyone ever had issues running the kegels on caliber trucks for some reason I want to say I saw that on silverfish a few years back.
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-12-13T19:45:28.444Z Reads: 320

```
I can't help much about the mechanical side of the question, but regarding the BLDC tool settings, it's a non-issue. If the motor spins the opposite of what you want, just swap any two of the three wires going to it, and voila, it's reversed.

I reverse mounted my motors (6355) on caliber IIs (the long ones) and there's about 2mm between the motors.
```

---
## \#3 Posted by: bigben Posted at: 2017-12-13T19:47:16.471Z Reads: 306

```
The 5065s won't fit in the same orientation on the same caliber truck, not even with some clever speed ringery. You could use torque board trucks or like you say, one forward and one reversed.
No problem with the motors running in different direction, you just need to swap 2 phase wires until they are in the right direction. I have keels on calibers no problem, just need the right driver pulley.
```

---
## \#4 Posted by: briman05 Posted at: 2017-12-13T19:54:14.039Z Reads: 293

```
Is there any downside to having one forward and one reversed on a rear wheel drive board? And I was between the 5065 and the 5045 and went with the 65 because it had because it had more power
```

---
## \#5 Posted by: bigben Posted at: 2017-12-13T19:56:56.718Z Reads: 280

```
I guess some people can’t get over the look of it?
```

---
## \#6 Posted by: briman05 Posted at: 2017-12-13T19:58:16.839Z Reads: 279

```
If it works the same with no downsides i see no problems with it
```

---
## \#7 Posted by: marcmt88 Posted at: 2017-12-13T20:00:46.644Z Reads: 275

```
dual 5045s on Caliber II

<img src="/uploads/db1493/original/3X/9/e/9ed3e2461b060e3ffe932669b64d2b1bfbc92e95.jpg" width="640" height="408">

dual 5045s on Ronin cast<img src="/uploads/db1493/original/3X/6/a/6a20d58933709b17122fd76ae1947232bc7ca3f2.jpg" width="640" height="492">
```

---
## \#8 Posted by: banjaxxed Posted at: 2017-12-13T21:09:31.884Z Reads: 259

```
You can probably set them up as normal in the tool then simply power down and switch two phase wires on the one which needs to turn the motor pulley 'the other way'. I was going to go this way but not possible on the board I'm working on right now, I think it could look well but the execution is all important to not having it look cack

Dual APS 6355 on caliber 11 50s, @WSB mounts and @johnny_261 15mm pulleys, @akhlut x-thingamajigs   
<img src="/uploads/db1493/original/3X/e/5/e5246eef9965d80f32f804c7e002cc77ae3edfa6.JPG" width="666" height="500">
```

---
## \#9 Posted by: pat.speed Posted at: 2017-12-13T21:12:34.551Z Reads: 249

```
You could get torqueboards 218mm trucks and they will fit easy
```

---
## \#10 Posted by: briman05 Posted at: 2017-12-13T21:16:54.832Z Reads: 248

```
I was hoping not to have to get the torqueboards trucks because I can get the cals for about 30 and I already have the bears
```

---
## \#11 Posted by: briman05 Posted at: 2017-12-13T21:19:03.998Z Reads: 242

```
I know the 5045 would fit but I got the 5065 because they had more power.  I was also thinking of getting 12mm belts if it would make it work.
```

---
## \#12 Posted by: pat.speed Posted at: 2017-12-13T21:22:59.094Z Reads: 239

```
You could shave down the insides of your wheels to gain an extra 15mm or so but I've never tried and I could ruin the wheels
```

---
## \#13 Posted by: briman05 Posted at: 2017-12-13T21:31:44.369Z Reads: 228

```
I do not have a lathe so that would not be someone I'm willing to try out.
```

---
## \#14 Posted by: aigenic Posted at: 2017-12-13T22:39:35.873Z Reads: 219

```
You can run diagonal set up, one motor on front truck, the second one on the rear truck :)
```

---
## \#15 Posted by: briman05 Posted at: 2017-12-14T02:13:09.991Z Reads: 206

```
I had thought about it but unsure of it
```

---
## \#16 Posted by: psychotiller Posted at: 2017-12-14T02:16:16.821Z Reads: 213

```
They'll fit perfectly on these.
https://psychotiller.com/product/surfrodz-tkp-trucks-with-thick-custom-quick66-mounts
```

---
## \#17 Posted by: briman05 Posted at: 2017-12-14T04:04:15.916Z Reads: 202

```
Thanks for the offer @psychotiller but they are are a little out f my range and I would want an rkp truck. I will probably look to you for an enclosure though.
```

---
## \#18 Posted by: psychotiller Posted at: 2017-12-14T04:26:58.208Z Reads: 196

```
Like this one? haha

https://psychotiller.com/product/surfrodz-177mm-rkp-trucks-with-dual-quick-66-mounts
```

---
## \#19 Posted by: vishal_tejwani Posted at: 2017-12-14T04:46:39.938Z Reads: 189

```
I have done the same thing and now thinking of mounting both the motors in opposite direction on same truck(back)
```

---
## \#20 Posted by: briman05 Posted at: 2017-12-14T04:52:08.945Z Reads: 189

```
Sumbitch you have an answer for everything. I must say no as I am trying to stick to my budget so I can get more boards in for my custom boards.
```

---
## \#21 Posted by: chuttney1 Posted at: 2017-12-14T12:14:29.858Z Reads: 173

```
There's nothing wrong reverse mounting the motor. I'm guessing we decide motors inside the board was better probably because it protected them. I had to do reverse cause I ran out of room because of battery pack and ESC.
```

---
## \#22 Posted by: marcmt88 Posted at: 2017-12-15T15:06:34.091Z Reads: 158

```
It's not so much the width of the belt that causes the problem but the width of the wheel pulley.
```

---
## \#23 Posted by: briman05 Posted at: 2017-12-15T16:23:52.543Z Reads: 151

```
The pulleys are a 36T 12mm
```

---
## \#24 Posted by: marcmt88 Posted at: 2017-12-15T16:35:57.171Z Reads: 145

```
You just gained 6mm for dual motors which bring you to a total of 10mm between motors.  There are 20mm difference between 5045s and 5065.  Running a dual 5065s side by side is not possible.
```

---
## \#25 Posted by: briman05 Posted at: 2017-12-15T16:53:41.845Z Reads: 137

```
So I’ll have to run one reversed out the backand the other under the board.
```

---
## \#26 Posted by: DEEIF Posted at: 2017-12-15T16:55:14.478Z Reads: 135

```
Or you could get TB 218mm trucks
```

---
## \#27 Posted by: briman05 Posted at: 2017-12-15T16:59:45.124Z Reads: 132

```
That was discussed earlier in the thread
```

---
## \#28 Posted by: DEEIF Posted at: 2017-12-15T17:00:05.725Z Reads: 136

```
Oh sorry I didn’t know
```

---
## \#29 Posted by: luis99945 Posted at: 2017-12-27T22:18:27.427Z Reads: 123

```
You have more pictures of your build
```

---
## \#30 Posted by: banjaxxed Posted at: 2017-12-27T22:31:11.708Z Reads: 123

```
Sorry for the derail 1 time
https://www.electric-skateboard.builders/t/magharees-puca-caliber-ii-fifty-2-x-aps-6355s-wsb-v1-0-mounts-johnny-261-pulleys-akhlut-x-bolt-plates-agniusm-n-e-s-e-cell-holders-samsung-25r-12s4p-freebord-s2-bindings/41278/19
```

---

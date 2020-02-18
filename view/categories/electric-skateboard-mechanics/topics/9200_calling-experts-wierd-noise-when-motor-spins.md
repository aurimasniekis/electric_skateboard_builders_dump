# Calling experts, wierd noise when motor spins

### Replies: 15 Views: 1515

## \#1 Posted by: listgaus Posted at: 2016-09-08T13:00:09.072Z Reads: 165

```
Hi all, 
First let me say that this is my 1st build.
The parts im using are Torqueboards 6372 230kv motor, V4 1bolt mount, 83mm wheels 16/36T@12mm belt running with VESC and GT2B remote. juice is 6S 3700mah (got two of these, bus using them 1 at a time) 
I've finally received the parts, assembled everything on a pintaill bamboo sektor 9 that i had waiting for this project, and set up the vesc via BLDC

after all set and done went for a spin, it runs really nice and takes up on hill really easy but the noise that comes from the motor is quite wiered, was wondering if anyone can help me figure what's wrong since i wanna enjoy this ride for a long time now :slight_smile:

attached are videos of noise while it spins...

Any ideas?! i'd love to understand whats wrong. since i lined everything up to the max, and it was all ordered from diyelectric, im guessing that i dont need to make extra modifications for the parts. or should i?

Also, one more thing i wanted to ask, i couldent set the motor to run in reverse, can anyone help with that too?

Links to the viedos: 
http://sendvid.com/xsn3s1j5
https://sendvid.com/xic31zv5
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-08T13:22:04.101Z Reads: 155

```
I cannot watch the videos at the moment with sound so i will answer what i can:

[quote="listgaus, post:1, topic:9200"]
Also, one more thing i wanted to ask, i couldent set the motor to run in reverse, can anyone help with that too?
[/quote]

Connect the VESC to BLDC-Tool and go to App-Configuration. Under "PPM" you can set the control mode to "Current". Then you should be able to break and after the break (when you go 0rpm) it goes backwards ;)
```

---
## \#3 Posted by: popopopop Posted at: 2016-09-08T13:24:49.518Z Reads: 135

```
Doesn't sound like motor to me. Something's rubbing against something? Spin your belt by hand and see if there's a place where it catches. Is your belt wobbly just a bit and rubbing against the wheel?
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2016-09-08T13:43:23.229Z Reads: 138

```
I had a similar noise when I first hooked up my TB dual setup. My problem was there was a slight wobble with the wheel pulley and it was hitting the motor mount screws slightly. Pop the wheel off and look at the inside edge of the pulley. The black paint had been scraped off mine on one of the wheels. This is how I found out what the noise was. Also you can remove the belt and slide the wheel back on and spin it to see the wobble if any.

If you used power tools to do the final tightening of the wheel pulley to the wheel this might be why as well. I did final tightening by hand. The wobble was my fault.

Good luck to you.
```

---
## \#5 Posted by: listgaus Posted at: 2016-09-08T14:05:10.695Z Reads: 124

```
i've uploaded this after reading your comment, 

maybe its the belt tension? i've checked and there nothing rubbing againt anything

http://sendvid.com/lbkwcjn6
```

---
## \#6 Posted by: listgaus Posted at: 2016-09-08T14:06:02.099Z Reads: 118

```
`[quote="DeathCookies, post:2, topic:9200"]
Connect the VESC to BLDC-Tool and go to App-Configuration. Under "PPM" you can set the control mode to "Current". Then you should be able to break and after the break (when you go 0rpm) it goes backwards :wink:
[/quote]

silly me, it was right infront of me and i marked earlier no reverse haha!!! thanks! ;)

@i2oadsweepei2 ive checked, no paint has come off, and i've only used hand power for everything :)
```

---
## \#7 Posted by: popopopop Posted at: 2016-09-08T14:25:12.876Z Reads: 112

```
I had a similar issue like i2oadsweepei2, but it was because I replaced my bolts with longer ones. It made a similar noise.

Remove the belt and run the motor, that'll narrow it down a bit further.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-09-08T17:32:33.722Z Reads: 100

```
Could be the pulley rocking on the shaft?
```

---
## \#9 Posted by: torqueboards Posted at: 2016-09-09T04:11:16.769Z Reads: 91

```
It does look like your belt is rubbing against your wheel. You can move the motor mount and/or add another axle washer to space it out a bit more.
```

---
## \#10 Posted by: Namasaki Posted at: 2016-09-09T04:22:25.827Z Reads: 82

```
Looks like the motor can is rubbing on the truck base. See the 2 rub lines on the motor.
```

---
## \#11 Posted by: listgaus Posted at: 2016-09-10T09:58:31.174Z Reads: 70

```
@popopopop thanks for the advise but i used the bolts that came with the kit. i've also removed like you advised the belt and  all goes smooth 

what i did notice @torqueboards is that the wheel pulley that comes with the kit is too narrow and the belt sticks out few mm and no matter how i zero the two pulley and how straight the belt is, it will always be sticking out 1-3mm and i think that thats what causes the sound

@Namasaki youre right about the lines. but thats thanks to me not securing the bolt when i 1st programmed the motor with the vesc via bldc and it hit the truck for few spins, lesson well learned for a beginner, but that not the case right now :)
```

---
## \#12 Posted by: popopopop Posted at: 2016-09-10T10:41:08.421Z Reads: 66

```
You're saying the sound is there with the belt off? It's known that torqueboard's wheel pulley does that. There shouldn't be a noise from that.
```

---
## \#13 Posted by: listgaus Posted at: 2016-09-10T11:15:34.199Z Reads: 63

```
the oppusite. only when belt is on.
```

---
## \#14 Posted by: torqueboards Posted at: 2016-09-10T18:07:09.217Z Reads: 55

```
@listgaus - The belt hangs off about 1mm. I can send you a 2mm washer if you want the full 12mm. The 1mm hanging is ok though.
```

---
## \#15 Posted by: listgaus Posted at: 2016-09-17T20:39:54.667Z Reads: 48

```
@torqueboards that would be perfect.
i'll pm you soon with details
```

---

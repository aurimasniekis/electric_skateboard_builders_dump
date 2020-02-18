# Slow going board

### Replies: 22 Views: 571

## \#1 Posted by: temo Posted at: 2018-07-11T09:33:21.961Z Reads: 156

```
Hello 
Thanks for letting me into the forum. 

I’ve a opposite problem than most people in here, I want to make a slow going board to my niece, preferably with a hub motor. Is there such a thing as a geard hub motor that will limit the top speed to say 5-6 km/h so she want outrun my sister. 

Terje
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2018-07-11T09:34:49.185Z Reads: 155

```
Just go 4s

Lower voltage
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2018-07-11T09:38:22.614Z Reads: 147

```
Or simply limit the travel of the throttle so she can’t pull the trigger all the way in. If you have a trigger type...You can use those small round rubber cushions that they put under vases and stuff so it dont scratch the table.... place it behind the trigger thick enough so she can only creep along

Same principle if you have a thumb throttle...limit range of  movement
```

---
## \#4 Posted by: Grozniy Posted at: 2018-07-11T09:53:11.247Z Reads: 133

```
Also smaller wheel size, smaller hub will impact speed
```

---
## \#5 Posted by: willpark16 Posted at: 2018-07-11T09:57:30.070Z Reads: 127

```
I just give kids niquil to make em sleep, but a 6s 60kv hub with throttle limitations should work fine
```

---
## \#6 Posted by: Maxid Posted at: 2018-07-11T09:59:49.224Z Reads: 126

```
Top speed can be set via VESC firmware.
```

---
## \#7 Posted by: temo Posted at: 2018-07-11T10:10:35.027Z Reads: 120

```
Thanks, many good suggestions here. So fare I think that limit the software will be the way to go, as she have a older brother that gladly would take the pads off. 
I don’t see many options for hub motors with low kv out there. Would anyone have a link and maybe a link to some instructions to program the VESC?
```

---
## \#8 Posted by: ROFEN13 Posted at: 2018-07-11T10:37:11.460Z Reads: 112

```
https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
Do you have a board already, and are modifying it? Or are you trying to build a board?
```

---
## \#9 Posted by: temo Posted at: 2018-07-11T11:26:32.195Z Reads: 100

```
It will be a new board from the ground up
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-07-11T11:34:53.053Z Reads: 99

```
Definintely 4.12 vesc has the software necessary to control al the factors needed to make this not only slow top speed but also slow acceleration, you can get them cheap now $60 or thereabouts if yo search hard enough, they come up regularly on the parts market of this forum, HK have them quickly available here
https://hobbyking.com/en_us/turnigy-sk8-esc-v4-12-for-electric-skateboard-conversion-w-bec.html

The alternative is one of those cheap eBay ESCs, but you can't limit them other then setting them to 6s and that can be too fast, would not advise controller modification as that will not limit the acceleration much or at all and 6s could be frightening and dangerous for a child let alone a teenager. a controller mod could fall out or fail in some way.

A cheap(ish) VESC will not be stressed by this at all and you should not experience any dreaded DRV/FET failures, especially running it in 6s. Also you get the lovely smooth FOC startup if you buy a sensored motor, again they can be had cheap, have a look at sensored motors under 200kv here
https://hobbyking.com/en_us/power-systems-1/electric-motors/size/above-50mm.html?dir=asc&order=price
```

---
## \#11 Posted by: Holyman92 Posted at: 2018-07-11T11:49:33.101Z Reads: 94

```
durring the setup process for the controller i believe you can set the max throttle for when the trigger is fully pulled.
```

---
## \#12 Posted by: temo Posted at: 2018-07-11T11:51:18.490Z Reads: 93

```
Yes this has been my concern from the start, that thing can fail, that's why I initially tough that if the motors itself cold not reach more than 5-6 km/h it would in it self be a safety feature.

To have a slow and controlled start would be very good, but is that mainly possible for out out-runner motors with the /s description and not in the in-wheel hub motors?

What would be the preferred RPM for a setup like this? If i'm correct low KV will mean less RPM but more torque.
```

---
## \#13 Posted by: Holyman92 Posted at: 2018-07-11T12:10:05.269Z Reads: 81

```
TBH i dont see it failing... i push my build hard and have a throttle limit so when the cops stop and ask, the board will never hit 30 mph
```

---
## \#14 Posted by: Kug3lis Posted at: 2018-07-11T12:26:46.903Z Reads: 78

```
max throttles will mean that at that position throttle will be 100% so at middle of your throttle it will be 100%.
```

---
## \#15 Posted by: temo Posted at: 2018-07-11T12:56:46.183Z Reads: 67

```
So that want help much then, only reach 100% power more quickly, not so as you only have 50% power at full trottle?
```

---
## \#16 Posted by: Sebike Posted at: 2018-07-11T13:10:28.907Z Reads: 64

```
I use the acmaniac app with my vescs to limit speed. Have a "kids mode" setup with a software limited speed of 6km/h. Works great!
Without speed limit - 45 km/h, so it'd better not fail :sweat_smile: (remote stays in my hand though!)
```

---
## \#17 Posted by: Maxid Posted at: 2018-07-11T13:15:24.578Z Reads: 64

```
where are you from? I might have a single sensored Lou Hub motor I could part with including trucks and wheels. I am in Germany.
```

---
## \#18 Posted by: Holyman92 Posted at: 2018-07-11T13:19:08.228Z Reads: 61

```
Same I use ack and I know there's a way to do it but I'm not sure I'm getting it across correctly
```

---
## \#19 Posted by: Sebike Posted at: 2018-07-11T13:34:07.326Z Reads: 55

```
My app settings for "kids mode"
Motor max 16 A
Batt max 25 A
Motor min -20 A
Batt min -8 A
Max speed 6.0 km/h
```

---
## \#20 Posted by: temo Posted at: 2018-07-11T14:13:20.475Z Reads: 54

```
Interesting I’ll look into that, but will anyone who’s with the kids have to run the app in real-time or is it a one time setup. 

I’m from Oslo, Norway and are soon to retire, so in need of a hobby, haha!
```

---
## \#21 Posted by: Sebike Posted at: 2018-07-11T14:57:46.265Z Reads: 47

```
You can have a number of preset modes, and when with kids, just switch to that mode. It's literally one click away. 

If you want to you can make any mode the default mode.
```

---
## \#22 Posted by: b264 Posted at: 2018-07-11T15:03:04.921Z Reads: 47

```
Don't use hub motors
```

---

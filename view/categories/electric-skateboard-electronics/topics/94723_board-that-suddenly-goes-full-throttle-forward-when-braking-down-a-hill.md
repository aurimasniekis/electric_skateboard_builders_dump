# Board that suddenly goes full throttle forward when braking down a hill

### Replies: 17 Views: 225

## \#1 Posted by: mikedv Posted at: 2019-05-23T09:51:52.291Z Reads: 111

```
Something crazy happened this morning while i was riding to work...
When i arrived at work i have to go down a steep hill that goes to a garage.
At the end of the hill i braked but instead of braking my board went full throttle forward and crashed into the parking wall.
On the way to work everything went flawlessly .
Unfortunately iam still at work and cannot check the vesc settings .
I think i have set my battery regen settings way to high for a 10s5p , if i remember well ive set it at -30 .
Does anyone have an idea what could have cause this weird behaviour?
I have currently 3 builds and this build is my only single motor build.

APS6374 170kv
Turnigy vesc (never had a single issue with it for more than 600km)
Crappy 10s5p diyeboard battery (50a)
Motor max : 75
Motor min: 75
Bat max : 50
Bat min : -30 (not 100% sure maybe -35)

Any idea what could have caused the full throttle forward when applying the brakes?
My board still powers up and so does the vesc and the remote. When applying throttle nothing happens anymore :frowning:
```

---
## \#2 Posted by: mikedv Posted at: 2019-05-23T09:52:52.664Z Reads: 106

```
Forgot to mention that I already did at least 50km withiout any issue with this setup
```

---
## \#3 Posted by: Andy87 Posted at: 2019-05-23T10:02:21.914Z Reads: 101

```
check your remote. is it charged? is your fail safe adjusted right? is your connection solid? maybe the antenna broke or something similar.
```

---
## \#4 Posted by: mikedv Posted at: 2019-05-23T10:06:11.806Z Reads: 99

```
I never adjusted failsafe tbh , i know it's stupid...
the remote connection seems ok , it isn't fully charged but the charging level seems ok. The problem is that iam stuck at work and do not even have a usb cable to connect my vesc on my laptop. I will need to walk to my car at a few km's from work...dammit
```

---
## \#5 Posted by: mikedv Posted at: 2019-05-23T10:07:01.027Z Reads: 94

```
will try to find a cable here to fully charge the remote and test again.
```

---
## \#6 Posted by: mikedv Posted at: 2019-05-23T10:13:38.376Z Reads: 87

```
No fuckin' usb cable here, will try again when back home and report back.Let's go for the walk of shame (3km carrinyg a 7kg board....).To many hills to push it...
```

---
## \#7 Posted by: brenternet Posted at: 2019-05-23T10:21:15.253Z Reads: 84

```
[quote="mikedv, post:4, topic:94723"]
I never adjusted failsafe tbh
[/quote]

Ding ding. Andy knows his stuff
```

---
## \#8 Posted by: lrdesigns Posted at: 2019-05-23T11:40:21.891Z Reads: 72

```
Which remote you have? 

I know the gt2b will start to act weird when the battery is too low. 

Badly set failsafe is also plausible. And fucking dangerous!
```

---
## \#9 Posted by: mikedv Posted at: 2019-05-23T11:40:38.656Z Reads: 70

```
indeed he does :slight_smile:Always there eto herlp people out.
```

---
## \#10 Posted by: mikedv Posted at: 2019-05-23T11:42:42.200Z Reads: 68

```
i have the maytech remote mtskr1712.
I just arrived home and tested everything....
Apparently my remote is broken.
I tried with the nano x i use with my mountainboard and it works flawlessly....
Crazy that the remove gave up on me at the moment i arrived at work and when riding downhill....
I will test my board now with the nano x , on the bench everything works fine now!
```

---
## \#11 Posted by: mikedv Posted at: 2019-05-23T11:58:02.155Z Reads: 61

```
Ok , thanks guys, test around the block done.
No more issues now. 
I cannot even imagine what would have happened if the incident occured a few meters before i arrived at work...i work in the city and there is a lot of traffic...
Anyways , i'll use the nano x for now .
@mmaner topic can be closed. Thanks.
```

---
## \#12 Posted by: lrdesigns Posted at: 2019-05-23T12:00:36.693Z Reads: 59

```
If it broke then going to full throttle could have been a result of bad failsafe setup. 

Please take the time to set and test the fail safe with new remote.
```

---
## \#13 Posted by: mikedv Posted at: 2019-05-23T12:01:16.100Z Reads: 56

```
i'll do so , thanks for the advice.
```

---
## \#14 Posted by: mikedv Posted at: 2019-05-23T14:20:30.593Z Reads: 41

```
After checking throughly I noticed one of the cables of the maytech remote receiver came loose....
```

---
## \#15 Posted by: brenternet Posted at: 2019-05-23T15:49:54.389Z Reads: 32

```
When a nano is considered the resolution to your remote problems I worry for our future 😞
```

---
## \#16 Posted by: mikedv Posted at: 2019-05-23T16:15:11.216Z Reads: 23

```
I totally agree with you. It's a terrible remote.no idea why it's being hyped that much. The maytech remote was rather good. I didn't have to calibrate it each time I turned on my board. Also,The build quality of the nano x really sucks balls.
```

---
## \#17 Posted by: mikedv Posted at: 2019-05-23T16:17:10.511Z Reads: 21

```
I was reffering to the Nanon x from Enertion. I never had a bad experience however with the Chinese nano or winny remote.
```

---

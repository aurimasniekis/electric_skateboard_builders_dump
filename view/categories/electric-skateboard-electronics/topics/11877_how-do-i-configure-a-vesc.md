# How do I configure a VESC?

### Replies: 21 Views: 2810

## \#1 Posted by: NickTheDude Posted at: 2016-10-25T18:16:24.175Z Reads: 198

```
So I'm having a lot of trouble figuring out the correct settings for my VESC, the guides I've found have been quite vague, and when searching through the forum I seem to be finding a ton of arguments about what is going on inside the VESC, and many, many, conflicting suggestions.

Does the limit on batt max really matter since I have lipos that can discharge a lot of current? What are the recommended settings for votlage min, batt min and motor min? What kind of effect does min ERPM have? If i set this too high will breaks cut out on my board when going down hills? Are the voltage limits for the battery/VESC input side or the VESC output/motor side? Are the default temperature cutoff settings good enough? What is absolute max amps? Is startup boost something that allows the motor to give an initial "shove" of torque to get you rolling? If I raise it will the board have a more aggressive launch?

These are my settings right now running 6S lipos with dual 230kV motors:

<img src="/uploads/db1493/original/3X/7/0/70df84ade460d589851c3d9e902503e3acbf3a88.png" width="690" height="388">

Sorry for all the questions, I'm just having a lot of trouble tracking down some solid answers.
```

---
## \#2 Posted by: sl33py Posted at: 2016-10-25T18:28:19.622Z Reads: 175

```
I've almost always kept the defaults and they work well.  I have 5 or 6 VESCs now... but am not an expert in the configuration as the defaults just work...

If you've run motor detection and it's working fine on the bench - i would not start out going downhill, but do some ride/testing.  

The only time i've had overvoltage or abs errors on my VESCs was during hard bench testing.  I adjusted settings specific to the errors and they ran fine after.  It was easy to duplicate on the bench - very distinct 3 flashes and unresponsive for 1/2 sec or so.  Easily fixed, but i don't recall which setting exactly at the moment.
```

---
## \#3 Posted by: NickTheDude Posted at: 2016-10-25T19:46:44.457Z Reads: 160

```
Alright, so I took it out for a spin using those settings. Everything was going fine and felt super smooth and perfect on flat ground, so I decided to test it on a hill. First I rode down the hill and braked on the way down. Then I started trying to climb a gentle slope with momentum, and both motors cut out. I felt the batteries, VESCs and motors. The batteries were a little warm, but everything else was fine. After that I just kick pushed it home.

The receiver is bound, and seemingly working fine. I checked the voltages on my batteries and they are fine as well. 

Then I plugged the first VESC into my computer and opened up BLCD tool. When I used the arrow key throttle absolutely nothing happened, I tried to get the motor to spin however possible but still nothing.

Then I tried the second VESC, and whenever I try to spin the motor using the arrow keys or any other method, the motor twitches...

Anyone know whats going on?
```

---
## \#4 Posted by: NickTheDude Posted at: 2016-10-25T19:59:12.097Z Reads: 149

```
Okay, looked at faults in the terminal and the first VESC that wasn't doing anything has a fried DRV... FUCK. 

This is super annoying... I don't think I was putting it under any particularly high amount of stress, and it seems like my settings are fine. It is possible that two of the phase wires touched together. Would that cause a short and fry the VESC?
```

---
## \#5 Posted by: NickTheDude Posted at: 2016-10-25T20:17:15.752Z Reads: 144

```
Did a little more testing, both motors are working fine, so it was only the VESC that got messed up...

I still have no idea what caused it.
```

---
## \#6 Posted by: Jinra Posted at: 2016-10-25T20:49:03.187Z Reads: 139

```
You'll have to replace the VESC or DRV. When you do, leave your max voltage at the default 57v, no need to change it. Also make sure to always test with slight throttle. If you go full throttle (high current) while the motor struggles to move due to a bad setting or other factors, you can easily blow a DRV.

I've had issues trying to get keyboard control to work too, I've never relied on it and just used my controller to test my motors.
```

---
## \#7 Posted by: NickTheDude Posted at: 2016-10-25T20:54:29.232Z Reads: 137

```
Yeah I messaged Johnny to try and use his VESC repair service. Everything was going fine up until the point where it blew. With the blown VESC removed it seems to be running fine on a single motor. Any idea what could have caused it? I'd like to be able to use the board while I wait for a repair/VESC.
```

---
## \#8 Posted by: Jinra Posted at: 2016-10-25T20:55:23.911Z Reads: 134

```
Paste more screenshots. BLDC tab, advanced tab, app config tabs.
```

---
## \#9 Posted by: NickTheDude Posted at: 2016-10-25T20:57:29.228Z Reads: 135

```
<img src="/uploads/db1493/original/3X/1/0/10411edd09732ef7097423c923aeeeab428004ba.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/6/c67b7b3ee9cdeffc79448a2fc9d075b5358ad848.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/c/4/c462fa9b91fdf41d70dacd09d6a56578ec316758.png" width="690" height="388">

<img src="/uploads/db1493/original/3X/6/a/6a6a7058f7e021bb1e3a2888546185c6c202e753.png" width="690" height="388">
```

---
## \#10 Posted by: Jinra Posted at: 2016-10-25T21:03:02.236Z Reads: 116

```
is this a picture of the slave vesc? Make sure to remove the erpm limit on the motor tab and use the default voltage when you get the vesc back. send status over can should only be used on the slave vesc
```

---
## \#11 Posted by: NickTheDude Posted at: 2016-10-25T21:07:55.854Z Reads: 113

```
I used the same settings for each VESC, the one connected to the receiver was the one that blew.

Remove the ERPM limit? The checkbox above the Min ERPM field?

And do you mean default voltage for just the voltage max or all the other voltage settings as well?
```

---
## \#12 Posted by: Jinra Posted at: 2016-10-25T21:12:11.665Z Reads: 112

```
Yea you need to configure the VESC differnetly depending if it's master or slave if you're using CAN.  "Send status over CAN" should ONLY be on the slave VESC and "multiple escs over can" should be only be on the master. Send status on both can lead to motors freaking out and blowing your controller.

the eRPM on the motor time is a hard limit and will cut off your VESC if you hit it, it's better to setup correctly for your max eRPM. You won't need it given your kv and battery.

Just the max voltage, leave at 57v.
```

---
## \#13 Posted by: NickTheDude Posted at: 2016-10-25T21:28:04.175Z Reads: 104

```
Alright, so right now I'm only running a single motor setup. I set the max voltage back to 57, unchecked "Send status over CAN" and "Multiple ESCs over CAN" and set the ERPM limit back to 100,000.

Would that ERPM limit kick in if I was going down hill fast enough to exceed the limit I set? At that point would the VESC stop, turning off your breaks?
```

---
## \#14 Posted by: Jinra Posted at: 2016-10-25T21:29:57.934Z Reads: 103

```
If you gear correctly, you shouldn't be hitting the limit and if you're going down hill, at least there won't be a ton of current in your system after the 60k soft limit. You shouldn't ever hit 100k.
```

---
## \#15 Posted by: NickTheDude Posted at: 2016-10-25T22:03:56.114Z Reads: 104

```
Alright, I just went for my first extended ride, feels much tamer with a single motor. But despite blowing up my first VESC nearly instantly, I still have a huge grin on my face :grin:

Thanks for the help dude!
```

---
## \#16 Posted by: chewydinosaurs Posted at: 2017-01-19T01:20:54.010Z Reads: 84

```
m not able to see my errors due to an issue with the BLDC window sizing as it covers up the fault error in the realtime data. Is there any other way to check the faults? I cant accelerate with my weight on the board for more than 3 seconds at any throttle percentage before the three red lights flash on the vesc and I have to wait 2-3 seconds to try again. Running a 6s with 280 kv motor, I have no issues throttling up when the motor isn't connected to the wheel, but when I try riding it, even super slowly I cant last more than 5 seconds at 2mph without the vesc cutting out.
```

---
## \#17 Posted by: Esrapp21 Posted at: 2017-01-19T01:30:50.268Z Reads: 80

```
I'm going to use a VESC with a single carvon v2.5 motor. I have small hills, like 10-15%. Should I be worried about blowing a DRV? Also, I plan to use foc, does this change anything from this perspective?
```

---
## \#18 Posted by: sl33py Posted at: 2017-01-19T19:27:54.112Z Reads: 78

```
on the system with windows sizing issue - check your screen resolution, or connect an external monitor, or address the driver that's giving you 800x600 or similar screen res.  Then you should be able to see the screen to get error messages.

I'm curious on your setup - what's your gearing for your 6s, 280kv ?
```

---
## \#19 Posted by: chewydinosaurs Posted at: 2017-01-23T04:26:27.869Z Reads: 70

```
I haven't tested out trying bldc on a different computer yet as I'm waiting for a new gear to show up, but my gearing ratio is 2.25.1
```

---
## \#20 Posted by: sl33py Posted at: 2017-01-24T01:22:52.333Z Reads: 69

```
Motor teeth and wheel teeth?  HTD5 or something different belt wise?  9/12/15mm wide belt?  What wheels are you using?

will give lots of info to suggest edits if needed, but ultimately just want to confirm your setup.  should not be cutting out on you - likely an error you can't see w/ your screen resolution issue.  Fix that and we can see what's really going on...
```

---
## \#21 Posted by: chewydinosaurs Posted at: 2017-01-24T02:17:28.053Z Reads: 65

```
I plugged into a separate monitor but while holding the motor (not mounted as I'm changing a few things) and it ran fine with no stopping. I think it may have to do with the gear being off center from the wheel and causing changing tensions on the belt and motor, as I was able to hold the motor pretty steady without any tension issues last night. I got the new gear tonight and will line it up for sure tomorrow to make sure it's centered on the wheel but the real test will come when I put weight on it. The other issue is if I do get the error again I'm not entirely sure how to skate with a laptop and monitor in each hand connected to the board lol. Motor teeth are 36 and wheel teeth are 16, belt is HTD5 9mm on 83mm wheels.
```

---

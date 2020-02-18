# Correct FOC settings? Controller Bugging Out

### Replies: 13 Views: 906

## \#1 Posted by: Dougieman1001 Posted at: 2017-06-25T19:35:36.387Z Reads: 113

```
So I'm just toying around with FOC and its capabilities and wanted to see if my settings were alright and wont fry my VESC.. I also wanted to try out reverse as it'd be quite useful for me but when I did just try it out it felt a bit sloppy like wasnt the most responsive, does this have anything to do with the Motor Min?
Setup - 
200KV 6374 Motor
10S battery
VESC-X (FOCBOX - Purchased before its name what changed but makes no difference I believe..)
Enertion Nano-X controller

Here are my BLDC Settings:

<img src="/uploads/db1493/original/3X/7/f/7f1910ddf8800cecce6fba1ae2176491092bf813.PNG" width="690" height="389"><img src="/uploads/db1493/original/3X/4/2/42c0af244b39f7d539812763b28016a9a0fb07df.PNG" width="690" height="389"><img src="/uploads/db1493/original/3X/a/a/aac92dd78cdfb941cf449c8a8bb4b8041d63c225.PNG" width="690" height="389"><img src="/uploads/db1493/original/3X/9/5/95fd8bb1556627e671cf56c2e47442a8cb028d52.PNG" width="690" height="388">

Thanks

***EDIT***
**Controller Bugging Out** 
So I just took it on another test run and it is doing weird shit.. I first pull away as normal out of my little road onto a bigger road which is slightly uphill. Whilst going uphill, I let go of the throttle to slow down a bit and rather than just cruise on the speed I had it slowed down and jerked a bit. Going back to pushing the throttle, I then had to push it much further to actually get any speed coming out of the motor. I thought it might be because I was on a hill so got to the flat road and tried again - similar thing happened, I had to push the controller much further than normal to actually get any speed. After accelerating, I pulled back and slowed to a stop before going into reverse to test that out. Pulling the trigger back obviously made me go backwards, it was okay until I let go of the trigger to slow a little and just roll, it doesn't. Rather than not powering the motor, I think the trigger must be slightly out and it was giving the motor power to continue driving backwards even when I wasn't pushing the trigger, the only way to stop it was to nudge it forwards a bit which disengaged the motor. Any ideas what is happening?
```

---
## \#2 Posted by: Blasto Posted at: 2017-06-25T19:39:40.319Z Reads: 88

```
Dis you do a foc motor detection? I would drop you batt max to 40A and your motor min to -60A
```

---
## \#3 Posted by: Dougieman1001 Posted at: 2017-06-25T19:40:40.600Z Reads: 86

```
Yeah, did the motor detection and Ill change those now.
```

---
## \#4 Posted by: Martinsp Posted at: 2017-06-25T19:50:29.717Z Reads: 82

```
What I always do is read the default configuration on motor tab and then set my voltages and currents again and then do motor detection... i do this whenever i am switching between BLDC and FOC. I know that it might only be a rumor that you have to load the default configuration when changing but Benjamin said that it should be done and.. i mean.. he is the VESC GOD right? :D :D 
Anyway.. that is what I do and I have never had problems when i loaded the default config. Apart from all of this, you can just never be too safe and i think that  5 minutes of setting up a bunch of parameters is worth potentially saving you 150€... :D 
Hope that helps
```

---
## \#5 Posted by: Martinsp Posted at: 2017-06-25T19:51:25.598Z Reads: 79

```
**IMPORTANT** always set your app to "no app" when doing motor detection because it can mess up the parameters a lot. :)
```

---
## \#6 Posted by: Dougieman1001 Posted at: 2017-06-25T19:55:59.493Z Reads: 73

```
So turn it off, do the motor detection and then turn it back on?
```

---
## \#7 Posted by: Martinsp Posted at: 2017-06-25T19:58:45.104Z Reads: 73

```
Exactly. You dont have to read the default config on the app tab because selecting "no app" disables it. So no reconfiguration of that is needed afterwards. Disabling it is enough.
```

---
## \#8 Posted by: Jinra Posted at: 2017-06-25T20:56:02.323Z Reads: 69

```
FYI the nano x does not record min max ppm until you start using it when turning it on.

This means that when you turn it on, just the slightest throttle or brake will constitute as 100% throttle or brake. To fix this, you have to throttle to max and completely brake every time you turn it on so it knows the min max values.
```

---
## \#9 Posted by: Dougieman1001 Posted at: 2017-06-25T21:02:24.106Z Reads: 66

```
Really? It does when I get it up on the screen, It does increase smoothly etc.. As if I was to accelerate fully, I'd probably fall off! So surely it is?
```

---
## \#10 Posted by: Jinra Posted at: 2017-06-25T21:11:34.178Z Reads: 65

```
I'm not sure what you're saying here
```

---
## \#11 Posted by: Dougieman1001 Posted at: 2017-06-25T21:23:13.729Z Reads: 65

```
Hang on.. I've just reread what you just said. So before I ride each time, I just need to put my controller at max and min so it knows?
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-25T21:33:55.328Z Reads: 60

```
yep that's it
```

---
## \#13 Posted by: Dougieman1001 Posted at: 2017-06-25T21:34:17.101Z Reads: 61

```
Ahh cool, just sorted all my problems in one sentence xD Cheers
```

---

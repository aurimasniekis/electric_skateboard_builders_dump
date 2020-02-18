# Have I broken it?

### Replies: 34 Views: 597

## \#1 Posted by: Freddiecook Posted at: 2019-01-21T19:52:54.323Z Reads: 218

```
Long story short, my board was working fine until my battery died (wouldn't charge), fast forward 2 months and I got a new battery, plugged her in and one of my VESCs from esk8.de isn't responding. Its just flashing red three times over and over again, tried checking for faults in the terminal but nothing, it will detect the motor but can't set it up in bldc, foc, sensored, sensorless, any of the combination, I assume that I've got a DVR error but I have no idea how this would have happened, if anyone could shed some light on my issue and how it would have come about it would be much appreciated. Thanks, and break it to me easy :broken_heart:
```

---
## \#2 Posted by: J0ker3366 Posted at: 2019-01-21T19:54:53.955Z Reads: 213

```
@JohnnyMeduse
```

---
## \#3 Posted by: Freddiecook Posted at: 2019-01-21T19:55:16.911Z Reads: 206

```
Oh no, bringing in the big guns
```

---
## \#4 Posted by: Andy87 Posted at: 2019-01-21T20:17:29.624Z Reads: 190

```
Was there a spark when you plugged in the battery?
```

---
## \#6 Posted by: Freddiecook Posted at: 2019-01-21T23:11:08.333Z Reads: 167

```
Nope, no spark.
The other vesc powered up nicely
```

---
## \#7 Posted by: Battosaii Posted at: 2019-01-21T23:42:58.173Z Reads: 156

```
Have you checked the terminal for fault codes in the Vesc tool?

Also does the Vesc flash red when you hit the throttle only?
```

---
## \#8 Posted by: Blasto Posted at: 2019-01-22T00:10:16.033Z Reads: 148

```
If the red led flashes repeatedly and shows no fault in the terminal, most likely your “minimum batt” voltage setting is something else than 8V

What is the input voltage you are supplying?
```

---
## \#9 Posted by: pat.speed Posted at: 2019-01-22T00:51:15.428Z Reads: 139

```
Probably not related to your issue but if you are running Can bus make sure to connect both vescs simultaneously or you can fry the can chips
```

---
## \#10 Posted by: Freddiecook Posted at: 2019-01-22T11:24:18.629Z Reads: 110

```
When I say I checked for faults I mean I typed in ‘faults’ and it returned that there were no faults since start up, is there another way?

And I can’t try the throttle because when I powered them up I updated the firmware on the so whipped their values. I did note that the flashing was happening before and after the firmware update
```

---
## \#11 Posted by: Freddiecook Posted at: 2019-01-22T11:26:02.272Z Reads: 106

```
I’m giving it power from my 10s pack, outputting 38v currently
```

---
## \#12 Posted by: Freddiecook Posted at: 2019-01-22T11:27:08.998Z Reads: 96

```
Yeah I am using can but I haven’t touched the can cable at all, I even wiped the vescs as I wanted to change the battery maximums and stuff
```

---
## \#13 Posted by: Andy87 Posted at: 2019-01-22T11:29:00.075Z Reads: 92

```
[quote="Freddiecook, post:10, topic:81636"]
And I can’t try the throttle because when I powered them up I updated the firmware on the so whipped their values. I did note that the flashing was happening before and after the firmware update
[/quote]

what you mean with it?
you updated FW on the faulty vesc?

[quote="Freddiecook, post:12, topic:81636"]
I even wiped the vescs as I wanted to change the battery maximums and stuff
[/quote]
 this one too. what you mean with "wiped".
you deleted stock settings?
```

---
## \#14 Posted by: Battosaii Posted at: 2019-01-22T12:21:14.838Z Reads: 76

```
Usually the red light has to be flashing for the fault code to show. You have to induce the failure during fault detection basicly.
```

---
## \#15 Posted by: Freddiecook Posted at: 2019-01-22T13:42:59.405Z Reads: 75

```
I updated the firmware on both of the vescs, red light was flashing before and after the update. When i mean wiped I mean I updated the firmware so it got rid of my previous settings, is that not how it works?
```

---
## \#16 Posted by: Freddiecook Posted at: 2019-01-22T13:44:54.360Z Reads: 74

```
It starts flashing as soon as it is powered on, I tried powering off the vesc then plugging the vesc into my pc then powering it up but still didn't get anything in the terminal
```

---
## \#17 Posted by: Andy87 Posted at: 2019-01-22T13:55:37.110Z Reads: 71

```
Power everything on, than try to start a motor detection which will fail and than have a look in the terminal if faults are written.
```

---
## \#18 Posted by: Freddiecook Posted at: 2019-01-22T20:10:33.609Z Reads: 68

```
When you say motor detection do you mean connecting it to the vesc tool?
```

---
## \#19 Posted by: J0ker3366 Posted at: 2019-01-22T20:12:32.717Z Reads: 61

```
&lrm; Yes.
```

---
## \#20 Posted by: dareno Posted at: 2019-01-22T20:13:37.616Z Reads: 58

```
Three red lights flashing usually means a drv fault.  I have a few like that and none of them connect to the vesc tool.
```

---
## \#21 Posted by: beasted_board Posted at: 2019-01-22T20:33:49.102Z Reads: 55

```
It could be the voltage regulator on the vesc that is dead. You can check it with a multimeter.
```

---
## \#22 Posted by: Andy87 Posted at: 2019-01-22T20:35:14.927Z Reads: 54

```
I have a focbox with drv fault too.
I can’t see the fault in the terminal, but if I connect the focbox via Bluetooth to any app I get directly the drv fault displayed.
If you have a bt module maybe that would be an option for you too.
```

---
## \#23 Posted by: Freddiecook Posted at: 2019-01-23T00:26:19.663Z Reads: 51

```
I just bought one but haven't set it up yet, I'll have a go next time I'm home.
Motor detection works btw
```

---
## \#24 Posted by: Freddiecook Posted at: 2019-02-04T21:04:27.198Z Reads: 45

```
Still no luck with the troubleshooting, took off the case to take a look, anyone see anything wrong? ![image|375x500](upload://tqSGUE63CZD4PBVuG6mxVxaFgZT.jpeg) ![image|666x500](upload://snWBCGQQkKXkDyN8Gxbhy4dQKcF.jpeg)
```

---
## \#25 Posted by: bigben Posted at: 2019-02-04T21:21:26.376Z Reads: 36

```
Can you reach out to esk8.de?
```

---
## \#26 Posted by: Freddiecook Posted at: 2019-02-04T21:48:58.412Z Reads: 35

```
I’ll have a go and see what they say
```

---
## \#27 Posted by: Freddiecook Posted at: 2019-02-04T21:59:04.564Z Reads: 36

```
Welp, just powered it up to see if it has magically fixed itself, lovely puff of smoke, crack it open to see the drv chip has blown, anyone know repairs for in the eu :wink:
```

---
## \#28 Posted by: bigben Posted at: 2019-02-04T22:09:00.218Z Reads: 32

```
@Martinsp used to do them. Not sure he's still around though.
```

---
## \#29 Posted by: Martinsp Posted at: 2019-02-04T22:13:29.365Z Reads: 32

```
I am around! :D Thank you for mentioning me @bigben :) 
@Freddiecook I am located in Slovakia offering repairs on all versions of "VESC ®" based ESCs.
[Here you can find more information](http://sprusi.com/index.php?id_product=22&id_product_attribute=0&rewrite=vesc-based-esc-repair&controller=product)  on the service, if you are interested please contact me via PM here.
```

---
## \#30 Posted by: 702vegas Posted at: 2019-02-04T23:12:10.384Z Reads: 26

```
I'm still waiting on the replacement from last year
```

---
## \#31 Posted by: Martinsp Posted at: 2019-02-05T18:30:36.221Z Reads: 24

```
Ill Pm you to sort this out
```

---
## \#32 Posted by: Andy87 Posted at: 2019-02-05T18:34:29.236Z Reads: 23

```
Maybe it’s just me, but your link is not working.
```

---
## \#33 Posted by: Martinsp Posted at: 2019-02-05T18:36:34.082Z Reads: 21

```
Oh thank you, I have just swapped the domain so in fact, no link I ever posted to electricskateboard.repair is now not working :D will put the new one there thanks :)
```

---
## \#34 Posted by: Andy87 Posted at: 2019-02-05T18:38:22.645Z Reads: 20

```
That would be nice! May need your service for two of my broken vescs too @Martinsp 😉
```

---
## \#35 Posted by: Martinsp Posted at: 2019-02-05T18:39:42.818Z Reads: 20

```
Sure, PM me some more details on what happened and Ill try to help you out! :)
```

---

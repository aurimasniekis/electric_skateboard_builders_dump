# Firmware update motor wont detect

### Replies: 26 Views: 1292

## \#1 Posted by: rexpepper651 Posted at: 2018-05-15T02:23:26.411Z Reads: 139

```
for the last week i have been trying to get my dual 6374 motors on two enertion focboxs to connect with can bus but cannot using bldc tool from enertion website (which i got motor detection). so i tried ackmaniac tool. i updated my firmware as it told me it was too old. i am able to set everything up motor wise besides it will not detect either motor. i also cannot get the can bus to work what so ever either. ive ran both set up wizards for motor and input and still nothing. no clue how to figure this out. this is my first build  and it is becoming very frustrating. if it helps im using a 12s5p battery as well. please any help would be much appreciated.
```

---
## \#2 Posted by: Slak Posted at: 2018-05-15T08:48:10.030Z Reads: 115

```
What tutorial did you use to set your Focboxes up ?

Did you remove the motor pulley and belt/chain before each launching motor detection in BLDC Tool ?

When you tried to set the 2 Focboxes up, have you powered only 1 focbox while the CAN bus was plugged to both Focboxes ?
```

---
## \#3 Posted by: rexpepper651 Posted at: 2018-05-15T12:20:38.752Z Reads: 111

```
I followed a video on YouTube of a guy setting up two hub motors. I did not keep can wire plugged in while configuring the motors settings using the setup wizard. No belts on the motor just the pulley. It's so weird that it will spin and work but no detection.  Motors fail hall sensor detection as well  even when using the bldc tool that will  detect the motors. So old firmware detects motors but not hall sensors.  Newer doesn't detect anything. There are no fault codes even after failing motor detection
```

---
## \#4 Posted by: Sender Posted at: 2018-05-15T12:27:28.219Z Reads: 97

```
@Slak is referring to when you did try to hook up canbus.  If you have both FB hooked up via CAN and don't power both Vescs at the same time, you can blow can chips...  I believe. 


http://www.electric-skateboard.builders/t/racerstar-hall-sensor-fail/54023/24?u=sender

Try this from @JohnnyMeduse
```

---
## \#5 Posted by: rexpepper651 Posted at: 2018-05-15T12:42:31.117Z Reads: 88

```
I was using my battery to.power both at sane time.  Never tried pwering one vesc at a time. I'll give tat a go when I get off work and let ya know how  it goes thanks
```

---
## \#6 Posted by: Bjork3n Posted at: 2018-05-15T12:45:11.812Z Reads: 86

```
Just to clarify do NOT power the vescs individually if you have the Canbus cable connected.
```

---
## \#7 Posted by: ShawnyP Posted at: 2018-05-15T12:53:23.948Z Reads: 83

```
If it wont detect and you have sensorless motor, you cud try raising the duty cycle i think is the d value next to the motor detect the default value is 0.05 raise it up.

There are couple good vids to show setting up can, best to check them out:

https://www.electric-skateboard.builders/t/how-to-program-canbus-properly-video-tutorial/52606?u=shawnyp
```

---
## \#8 Posted by: rexpepper651 Posted at: 2018-05-15T13:27:49.777Z Reads: 73

```
yeah i figured it would be bad to power them up seperatly which i never have or intend to do.
```

---
## \#9 Posted by: rexpepper651 Posted at: 2018-05-15T13:28:21.497Z Reads: 73

```
i have maytech 6374 with sensor wires but i will try that thank you
```

---
## \#10 Posted by: ShawnyP Posted at: 2018-05-15T14:08:14.778Z Reads: 68

```
Not sure if it will help for sensored, did you have the sensor cable connected when you tried to run the detection?
```

---
## \#11 Posted by: rexpepper651 Posted at: 2018-05-15T14:11:24.787Z Reads: 67

```
yes. i had everything but can wire plugged in while trying to get everything working. its so strange that the old firmware with a different bldc tool would detect the motors but with newer firmware would not. i will also post pics of my  vesc settings if that will help
```

---
## \#12 Posted by: Wallgreeens Posted at: 2018-05-15T15:57:46.849Z Reads: 62

```
I was not there after the update, but before it the motors were detecting just fine.  As for the CanBus issue, I tried using one of my spare focboxes on rexpeppers setup in place of each focbox and got the same issue with the Canbus not communicating.   I've also tried rotating the master/slave vesc with no luck. Each motor  works individually as the master, but no the salve just wont' work.  We thought it may be a janky cable, so he ordered a canbus cable from psychotiller.
```

---
## \#13 Posted by: rexpepper651 Posted at: 2018-05-15T16:13:55.057Z Reads: 59

```
i tried the new wires yesterday wallgreens and no luck which was what led me to try firmware update
```

---
## \#14 Posted by: Wallgreeens Posted at: 2018-05-15T16:17:55.638Z Reads: 62

```
What firmware are your boxes running now?
```

---
## \#15 Posted by: rexpepper651 Posted at: 2018-05-15T16:23:01.734Z Reads: 59

```
i reverted them back to 2.18 since the ackmaniac tool wasnt detecting the motors or sensors. i think it was 3.1 for firmware
```

---
## \#16 Posted by: briman05 Posted at: 2018-05-15T16:30:03.966Z Reads: 60

```
are you trying in bldc or in FOC I had one motor that would get picked up in bldc on the bldc tool but not the other one.  I tried bldc in Acks vesc tool and neither worked.  Tried FOC and both motor and hall sensor were detected
```

---
## \#17 Posted by: rexpepper651 Posted at: 2018-05-15T16:33:58.472Z Reads: 58

```
ive was originally trying to set up in foc but have tried bldc as well with no success with ackmaniacs tool
```

---
## \#18 Posted by: rexpepper651 Posted at: 2018-05-15T16:40:16.534Z Reads: 60

```
 this is the one i had used https://www.youtube.com/watch?v=v1glLDO-EjA&t=529s
```

---
## \#19 Posted by: Wallgreeens Posted at: 2018-05-15T17:55:53.710Z Reads: 58

```
@longhairedboy  Any ideas or things to try on this one bro?  I'm thinking of trying his vescs inside my board to try and isolate the problem, but you or Jake's expert advice would be greatly appreciated.
```

---
## \#20 Posted by: Esk8t.nz Posted at: 2018-05-16T10:28:36.278Z Reads: 53

```
It doesnt detect or you get the hall error 255?
```

---
## \#21 Posted by: rexpepper651 Posted at: 2018-05-16T13:50:32.113Z Reads: 47

```
it doesnt detect no hall error or faults.
```

---
## \#22 Posted by: longhairedboy Posted at: 2018-05-16T16:20:40.039Z Reads: 46

```
[quote="Wallgreeens, post:12, topic:55503"]
As for the CanBus issue, I tried using one of my spare focboxes on rexpeppers setup in place of each focbox and got the same issue with the Canbus not communicating.
[/quote]

Solder that cable and ditch the connector.
```

---
## \#25 Posted by: Wallgreeens Posted at: 2018-05-16T23:04:07.578Z Reads: 41

```
@longhairedboy I was considering that, but how do you solder onto such tiny pins? I was thinking separate them with a tiny piece of plastic and dribble a little solder onto each connector.
```

---
## \#26 Posted by: longhairedboy Posted at: 2018-05-17T19:52:32.927Z Reads: 38

```
* slip 3mm heat shrink onto wire
* flux the pins
* flux the wires
* tin the pins
* tin the wires
* hold the tinned wire to the tinned pin
* tap the iron on it so they melt together
* slip the heat shrink over the solder joint and cover the whole pin
* apply heat from rework station or heat gun to shrink the heat-shrink, don't use a torch
* repeat for second pin
```

---
## \#27 Posted by: Wallgreeens Posted at: 2018-05-18T09:51:56.928Z Reads: 33

```
Sweet, thanks for the instructions.  Seems much better than the route inwaa going to take.  He ended up using a y servo cable splitter and called it a day.
```

---
## \#28 Posted by: rexpepper651 Posted at: 2018-05-20T15:51:27.037Z Reads: 28

```
Thanks @longhairedboy
```

---

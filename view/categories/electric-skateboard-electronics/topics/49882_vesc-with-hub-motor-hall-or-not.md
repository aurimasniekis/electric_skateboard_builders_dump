# VESC with Hub Motor hall or not?

### Replies: 5 Views: 683

## \#1 Posted by: Harley164 Posted at: 2018-03-22T22:26:03.981Z Reads: 133

```
Hi all,

Very new to the forum and have yet to build my first board.   After all the research I'm looking to build a board with dual VESC and the dual hub motor that's similar to the Meepo setup.

I'm assuming that since we know the individual motors are 550W and 70kv, we can adjust the VESC so it doesn't blow the motor out - that's simple enough (or so I think)  Haven't gotten too much into VESC programming yet, but I understand you need to set the output so it doesn't send too much power to the motors.

The VESC has a 6 pin Hall pinout - the extra being for the temp sesnor.  The dual hub motor only has a 5pin hall connector.  Question is - do you just make an adapter leaving out the temp sensor or just dump the hall sensors all together?  I've read the pro's and cons and am not convinced the hall sensor is necessary - just adding some acceleration smoothness if i'm not mistaken.

the reason why i'm opting for the dual VESC vs the specific dual esc that's meant to work with the hub motors is that in the future if i'm able to upgrade to some motors like the ones hummie makes or torque - i'd like the option to just upgrade and reprogram the VESC.  

i'm sure you guys are familiar with what i'm writing about, but this the truck/motor combo.  https://kvboards.com/collections/motors/products/powerful-90mm-dual-hub-motors-1100w
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-22T22:28:13.123Z Reads: 127

```
Once you go sensored you will never go back to sensorless..
```

---
## \#4 Posted by: goldrabe Posted at: 2018-03-23T02:36:24.615Z Reads: 101

```
I would say it depends on which Vesc you are using.
If you have a good Vesc capable of Foc, running the motors with hall sensors makes everything even more smooth and silent. I think that is the main reason for choosing hubs over a different drive train.
If you run the motors in BLDC, for me there is little reason to bother with the hall sensors.
```

---
## \#5 Posted by: evoheyax Posted at: 2018-03-23T05:32:27.433Z Reads: 90

```
I sort of agree... Yes, sensors are great. But they are one more very fragile piece that can break. Once you get a hub motor to a certain size, sensors have a minimal effect. In small hub motors, yes, it's night and day different. Lets remember, sensors are only useful for 0-3 mph. After that, they have are actually a down side. This is why the vesc has a hybrid mode in bldc and foc automatically turns the sensors off after about 3 mph.

With hummies latest hubs, I have no issues of cogging from a stand still. I have to pull the trigger more carefully, or I could cog, but once you learn, it's not an issue. It's also better for the motors to give a push anyways, sensors or not.

Sensors can be really nice when they work, but it's one more sensitive part that can fail. Simpler in this case is more reliable.
```

---
## \#6 Posted by: RedEagle Posted at: 2018-03-27T14:46:31.044Z Reads: 57

```
I wholeheartedly agree, but sometimes the pros outweigh the cons. It's true that cogging won't be a problem with a little practice. On the flipside, why not use a feature when it's there anyway? It's not like it's a big pain to deal with.
If it's there and it's a good feature _and_ you don't mind dealing with it, use it. :slight_smile:
Otherwise don't. :sweat_smile:
```

---

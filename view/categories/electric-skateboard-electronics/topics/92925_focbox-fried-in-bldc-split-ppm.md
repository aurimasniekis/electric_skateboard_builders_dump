# Focbox fried in bldc, split ppm

### Replies: 24 Views: 462

## \#1 Posted by: Bjork3n Posted at: 2019-05-06T04:23:32.313Z Reads: 127

```
Hey guys! So i got a message from the guy who bought my previous build and apparently his focbox fried hard! 

https://imgur.com/a/NwHYyNT
Tried to post pictures on the forum but apparently it didnt work this morning..

The settings/setup were
- Torqueboard 190kv 6355 motor
- 10s4p battery 80A bms
- split ppm between the boxes
- ackmaniac fw 3.101
- bldc mode
- motormax 60A, batterymax 35A, batterymin -8A,  motormin -50A. 

It's only one of the focboxes that fried. 
When it broke the motor was twitching and it occurred during acceleration after a downhill with braking. 
The owner told me he saw flames and smoke from the board so he immediately stopped. 

What can cause this failure? My first theory is motor short? 
Also worth mentioning is that this setup has been flawless for the last 1000km with no problem what so ever. 

Thanks.
```

---
## \#2 Posted by: b264 Posted at: 2019-05-06T04:29:50.727Z Reads: 120

```
I also just had one single FOCBOX fry 

* 190kv Dark Matter motors
* 10S10P, bypassed BMS
* Dual independent PWM (dual "PPM")
* @Ackmaniac fw 3.103 
* BLDC hybrid mode
* motormax 60A, batterymax 29A, batterymin -11.6A, motormin -40A

It’s only one of the FOCBOXes (1.6) that fried. When it broke the motor was twitching.  I don't see/smell smoke but I'm taking it apart right now...

Oddly similar :thinking:

My motor is good, I [hand-tested it](https://forum./t/how-to-hand-test-a-bldc-motor/568) and then connected it to a VESCX (FOCBOX 1.3) and it's totally fine.
```

---
## \#3 Posted by: Bjork3n Posted at: 2019-05-06T04:33:36.855Z Reads: 109

```
This setup has been running without any issue for the last 1000km so this came out of the blue. 
Im just glad it didnt set the batterypack on fire...
```

---
## \#4 Posted by: Dirt_Bag Posted at: 2019-05-06T04:44:35.588Z Reads: 104

```
Are you running new firmware? I have seen so many people complaining of bricked or fried vescs following the update
```

---
## \#5 Posted by: dareno Posted at: 2019-05-06T04:50:17.449Z Reads: 105

```
Thats a bad one certainly.  I've fried many a vesc but not to that extent.  That definitely looks like a short to do that much damage.  Don't think over voltage could cause that devastation.
```

---
## \#6 Posted by: Jansen Posted at: 2019-05-06T05:36:57.740Z Reads: 104

```
Dude! Crazy! I just had this randomly happen to me on two different builds in the same week that were otherwise running fine for the last 6 months plus. Didn't change anything and all of a sudden after breaking downhill one day my power/breaking was cut in half on my R2 and realized one of my motors wasn't spinning only to get home and have one of the same pieces on my focbox blown out. Ride this board daily since October. Luckily enertion was good and got me a new focbox within a week, only to have the same thing happen today and now I have to hit them up again. No issues before this happened and no changes on anything.

Got the new TB DD and it's fried 2 focboxes in the last couple of weeks, both on initial test runs and I can't figure out why... VESC(s) showing no sign of damage at all, no red light, just dim blue.... They will not connect anymore to VESC of BLDC and I've tried everything.... using the same set up from a prior DIY set up I had so I know it was working fine for close to a year. Switch to the DD's, passed motor detection with ack's firmware no problem and motors sounded great, 5 mins into first test run not even going above 60-70% throttle and one motor goes out with focbox fried and not connecting anymore to either tool.... any clue why this could happen? The same motor took out both focboxes, the other focbox is fine and still is and it's my oldest one.... running 10s4p brand new R2 spare battery, loopkey, focboxes with TB dd's and 110's on the new EVO deck and settings were  conservative at 60, -40, 25, -10. I reached out to dexter too already and am thinking something is up with the motor cause everything else is fine. Interested to see where this goes. Sorry for the long post, super annoyed and frustrated. Still haven't even got to take the DD's out for a real ride yet after almost a month of having them! FML. Watching this.....
```

---
## \#7 Posted by: Jansen Posted at: 2019-05-06T05:43:21.111Z Reads: 90

```
running split PPM and not canbus or anything either....
```

---
## \#8 Posted by: taz Posted at: 2019-05-06T08:36:24.194Z Reads: 78

```
Split ppm can lead to vesc failure

https://vesc-project.com/node/80
```

---
## \#9 Posted by: Bjork3n Posted at: 2019-05-06T09:24:22.757Z Reads: 72

```
How do you check a motor for shorts?
```

---
## \#10 Posted by: Creavenger Posted at: 2019-05-06T10:13:22.004Z Reads: 72

```
Focboxes frying left n right :roll_eyes:
```

---
## \#11 Posted by: b264 Posted at: 2019-05-06T10:17:52.974Z Reads: 70

```
I haven't heard that yet, just now tried @Ackmaniac's  firmware.  I'm moving them both back to Vedder/3.34 right now
```

---
## \#12 Posted by: arzi7 Posted at: 2019-05-06T11:16:11.641Z Reads: 66

```
![MVIMG_20190320_145336|666x500](upload://tnhQvRhwesQ0DXaruWDlzhg2ZEI.jpeg) 

Absolutely same situation. 2 minutes after setup happened to me.
```

---
## \#13 Posted by: Andy87 Posted at: 2019-05-06T14:48:53.219Z Reads: 61

```
Which firmware was on your focbox?
```

---
## \#14 Posted by: Bjork3n Posted at: 2019-05-06T14:57:03.052Z Reads: 59

```
Ackmaniac 3.101.
Been working fine for over 70miles then this happend.
```

---
## \#15 Posted by: Andy87 Posted at: 2019-05-06T14:58:00.219Z Reads: 60

```
Sorry it was question to @arzi7
```

---
## \#16 Posted by: arzi7 Posted at: 2019-05-06T15:07:52.135Z Reads: 60

```
The latest on early April. I don't remember. Opened from a box, connected, installed latest firmware, made 3 meters :slight_smile:
Returned to my Maytech Vescs and happy with it
```

---
## \#17 Posted by: Andy87 Posted at: 2019-05-06T15:10:22.134Z Reads: 60

```
But the stock vesc firmware not ackmaniac, just to get it clear.
```

---
## \#18 Posted by: thisguyhere Posted at: 2019-05-06T15:30:40.549Z Reads: 55

```
[quote="taz, post:8, topic:92925"]
Split ppm can lead to vesc failure

[https://vesc-project.com/node/80 ](https://vesc-project.com/node/80)
[/quote]

good to know.

been on one remote - dual receiver for a while now, guess that was a good move...
```

---
## \#19 Posted by: b264 Posted at: 2019-05-06T17:51:49.466Z Reads: 48

```
I was running dual receiver when mine died, but it didn't blow the FET apart.
```

---
## \#20 Posted by: Jansen Posted at: 2019-05-06T18:28:19.312Z Reads: 44

```
![IMG_0409|375x500](upload://oIDJvC96WPy8HkzsSEvJLPwx8ON.jpeg) 

I was on @Ackmaniac and always use his but this is the first time I had an issue. The other ones that blew didn't blow mosfets and I'm not sure what's wrong with them. One gets a dim blue light and won't connect and can't flash anything on it, one says DRV but not the code that everyone usually gets just DRV with no numbers after, the other just doesn't respond....
```

---
## \#21 Posted by: Bjork3n Posted at: 2019-05-06T18:45:50.068Z Reads: 37

```
Odd that most have failures with ackmaniac? What fw does you other guys use? I love the ack fw, it made my board smooth as butter
```

---
## \#22 Posted by: Jansen Posted at: 2019-05-06T18:57:50.253Z Reads: 37

```
Does anyone see anything wrong on the other 3 that are not working.... it's just weird cause it happened in my R2 on stock firmware and nothing was changed, then happened on my new TB DD set up from the same motor 2 times but yet the other one is fine still....
![IMG_0402|375x500](upload://m6yP3EewEySpv3JP5GhStgxdW5A.jpeg) ![IMG_0404|666x500](upload://48qCQzWYPkPnEbJT1iDD1jiVILz.jpeg) ![IMG_0406|375x500](upload://uDCNMikGPLmgN9pBpBLVmijSpgP.jpeg) ![IMG_0407|666x500](upload://9k9xrYtLidSyvqfxvtROceEtLEY.jpeg) ![IMG_0408|375x500](upload://1iiONycOQIzKLng8sLTueTfBOlt.jpeg) ![IMG_0409|375x500](upload://oIDJvC96WPy8HkzsSEvJLPwx8ON.jpeg) ![IMG_0411|375x500](upload://u1AnxCCGa0LnWPevQJLbMgnbwqn.jpeg) ![IMG_0413|375x500](upload://ecGxnS3EC2B8rAP5L6ArSKUwZD2.jpeg) ![IMG_0415|375x500](upload://mOuqQ8Uh90cyVFBsgsehLCIMeNT.jpeg) ![20574365-D74C-4BDF-A0C7-963F7356418B|375x500](upload://86Lydoj15Y0Ew1zJjSdycWZT4We.jpeg)
```

---
## \#23 Posted by: Jansen Posted at: 2019-05-06T18:58:45.849Z Reads: 33

```
@JohnnyMeduse How much to repair 3-4 VESC, any type of deal for multiple?
```

---
## \#24 Posted by: JohnnyMeduse Posted at: 2019-05-06T20:44:53.872Z Reads: 30

```
Same price as usual 45USD each (return shipping include)
```

---

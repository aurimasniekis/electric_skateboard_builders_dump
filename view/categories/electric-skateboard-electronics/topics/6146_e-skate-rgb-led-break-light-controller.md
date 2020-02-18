# E-Skate RGB LED / Break light Controller

### Replies: 6 Views: 1984

## \#1 Posted by: DerBrecher Posted at: 2016-07-15T13:27:08.082Z Reads: 195

```
Hi Guys,

i recently had to much free time and therefore started to built a RGB LED controller for my E-Longboard.
First off i simply built an normal controller with allowed me to set static Colors and let the LEDs fade in different patterns and speeds. But then a friend of mine had an idea why not let the throttle you give the Board also control the LEDs.

Therefore i added two new modes:

1. The throttle controls the fade speed. More throttle --> faster fade

2. The throttle controls the Color of the LEDs.
    When the throttle is in the idle position the LEDs are Blue when you start to accelerate they fade from blue to green and      
    finally to red when you maxed out the throttle. 

Here you can the the controller which uses an Arduino Mini and 3 N-Channel MOSFETs. You can also see the RGB strip which is temporary mounted with Duct tape :sweat_smile:
<img src="/uploads/db1493/original/2X/6/647e744559fe36c8fa7e35e0c54a4b47c20b2101.jpg" width="690" height="388">
/
/
I then also got the idea to add an fourth MOSFET to control a LED break light. Since i already got the throttle value for the RGB modes i simply had to add 5 extra lines and got a nice break light. The IR-Receiver is mounted in the cutout for the trucks, so it is easy to reach while standing on the board. 
<img src="/uploads/db1493/original/2X/3/3eab7290ade41d7f26113613bcbd1dc24528078e.jpg" width="690" height="388">
```

---
## \#2 Posted by: Skitzor Posted at: 2016-07-15T14:36:37.028Z Reads: 180

```
Nice find! I'm looking to so something similar but with a VESC, would you mind posting your parts used, schematics and arduino code? Would appreciate it!
```

---
## \#3 Posted by: Ulfberht Posted at: 2016-07-15T21:49:43.359Z Reads: 165

```
KILLER!!!
 You might want to switch to an RF controller, but I absolutely love this idea and can't wait to see more!  I have been advised that IR controller can have issues when used outside and the IR beam can be easily interrupted. 
I'm excited to see such awesome work! 
THANKS dude!!
```

---
## \#4 Posted by: torqueboards Posted at: 2016-07-15T22:04:05.049Z Reads: 159

```
Sounds like fun!
```

---
## \#5 Posted by: DerBrecher Posted at: 2016-07-16T11:05:15.342Z Reads: 129

```
@Skitzor  will post my code when i get back home tomorrow. What website do you suggest i use for sharing?
And i dont have any schematics ready but maybe i can draw something for you.

[This](http://www.ebay.de/itm/5pc-CH340G-USB-Nano-V3-0-ATmega328P-5V-16M-Micro-Controller-Board-Arduino-TE359-/201426905480?hash=item2ee5faa988:g:R1MAAOSwnNBXV9Yh) is the Arduino i used. To power the Arduino I use the BEC from the ESC. I used [these Buck Converts](http://www.ebay.de/itm/10PCS-Mini-360-DC-DC-4-75V-23V-to-1V-17V-Buck-Converter-Step-Down-Module-TE383-/201465558677?hash=item2ee8487695:g:USoAAOSw7hRWQ3Gs) to get 12V from the 6s Battery i am using. Four of [these N-Channel MOSFETs](http://www.ebay.de/itm/10-x-IRLZ34-N-Channel-MOSFET-/152139995484?hash=item236c40195c:g:RJ0AAOSwe7BWvh-y). And a common Anode LED Strip. The break light uses the same MOSFETs and this [LED break light](https://www.amazon.de/Dritte-Bremsleuchte-Auto-Bremslicht-Stopplicht/dp/B00B5989OY?ie=UTF8&keywords=led%20bremslicht&qid=1459807128&ref_=sr_1_5&sr=8-5)


@Ulfberht I am already using an IR Remote to control the different modes. Similar to this one http://cdn.instructables.com/F9P/659Z/HNL5QQHT/F9P659ZHNL5QQHT.MEDIUM.jpg

@torqueboards Night rides are awesome with this setup. People stare at you and think you are a wizard.
```

---
## \#6 Posted by: DerBrecher Posted at: 2016-07-18T11:51:19.290Z Reads: 104

```
@Skitzor I just uploaded the code to my Google Drive. I hope you can understand the Code because i only have a few Comments in it. O lot of the code is just copy from examples which were provided with the libraries i used. Speaking of these you need the RGBMood, IRremote and PinChangeInt libraries. Here is the [link to my Code](https://drive.google.com/file/d/0Bz0sjLiz6-0jTWxjM01TaEprbXc/view?usp=sharing).
```

---

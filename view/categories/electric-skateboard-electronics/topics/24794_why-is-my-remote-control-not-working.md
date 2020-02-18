# Why is my remote control not working?

### Replies: 18 Views: 1786

## \#1 Posted by: Geddi Posted at: 2017-06-07T10:10:57.379Z Reads: 130

```
I am testing my parts and I cannot figure out how to connect the remote control properly or set the settings in the bldc tool.
As you can see on this picture the remote control is connected (Channel 2) and everything looks good, but when I pull the trigger the motor won't move.
I have the remote from alien. Click on this [link](http://alienpowersystem.com/wp-content/uploads/2016/09/APS-EVT3-DIGITAL-PROPORTIONAL-RADIO-CONTROL-SYSTEM.pdf) to see the description of the remote.
In the BLDC tool I set under the category "App Configuration General" PPM and UART ( I tried many of the available settings actually). And under PPM I set "Control Mode" to "Current no reverse with brake" (here I also tried out multiple settings"). Everything else is set to default since the firmware update.

<img src="/uploads/db1493/original/3X/0/2/0278ab15c8f6e3aee831abe53dbc8256e852046f.jpg" width="666" height="500">
```

---
## \#2 Posted by: L3chef Posted at: 2017-06-07T10:21:36.135Z Reads: 118

```
I think the servo signal cable is wrong. It should be where the brown one is
```

---
## \#3 Posted by: L3chef Posted at: 2017-06-07T10:24:34.426Z Reads: 119

```
Looking from left on the reciever it should be signal-poitiv and negativ
```

---
## \#4 Posted by: Geddi Posted at: 2017-06-07T10:25:34.297Z Reads: 118

```
@L3chef so you think i should switch the connecter at the receiver arround 180°
```

---
## \#5 Posted by: L3chef Posted at: 2017-06-07T10:31:05.139Z Reads: 113

```
Yes, but please first double check that you have signal +&- connected right on the vesc.

<img src="/uploads/db1493/original/3X/7/7/77e78d1a33753f6471cf58ecd400068141abc7ff.PNG" width="690" height="265">
```

---
## \#6 Posted by: Geddi Posted at: 2017-06-07T10:33:28.668Z Reads: 113

```
<img src="/uploads/db1493/original/3X/1/f/1fa26491e7772c0eec455fc2bc00e7850d683fce.jpg" width="375" height="500">
@L3chef  hope so it was shipped like that.
```

---
## \#7 Posted by: L3chef Posted at: 2017-06-07T10:34:05.439Z Reads: 109

```
Looks good. Now switch on the reciever
```

---
## \#8 Posted by: Geddi Posted at: 2017-06-07T10:41:17.974Z Reads: 109

```
alright thanks, I will try it out later :slight_smile:
```

---
## \#9 Posted by: L3chef Posted at: 2017-06-07T10:42:12.238Z Reads: 107

```
Let me know if it works :)
```

---
## \#10 Posted by: Geddi Posted at: 2017-06-07T12:17:04.655Z Reads: 103

```
@L3chef
Thanks! It does work now!
Can you explain what those different modes are?
Alle the control modes with "current" work really shity. They only work properly if I move the trigger very slowly at the beginning otherwise the motor just kind of gets "stuck". The "duty" and "PID" modes work really well, but I could not spot a difference there. Do you know the difference?
```

---
## \#11 Posted by: L3chef Posted at: 2017-06-07T12:56:21.141Z Reads: 99

```
Great! :slight_smile:
It's been over a year since I last played with bldc tool, so I'm not the right person answering your qurstion.. Maybe @Jinra or someone else could help you with that
```

---
## \#12 Posted by: Jinra Posted at: 2017-06-07T16:43:46.673Z Reads: 92

```
Current is the most natural feeling mode (and best in the default BLDC tool IMO). Running it on the bench is different than how it'll perform when your ide. It applies current to the motor and will spin at full speed once load has been overcome. When testing on the bench, there's very little load so it spins up to max RPM straightaway. This won't be the cause when you actually stand on the board.

Duty and PID control control the RPM of the motor directly, but also have the drawback of managing that RPM through the throttle. This means that while accelerating would be okay, letting go of the throttle will cause the board to brake.

Duty cycle controls the % of throttle to voltage in the range of 0-95%. 0% duty cycle = 0 voltage, 95% duty cycle = max voltage.

PID control relies on configuring a target eRPM in which 0% throttle would be 0 erpm and 100% throttle would be the configured target erpm.
```

---
## \#13 Posted by: L3chef Posted at: 2017-06-07T18:36:17.975Z Reads: 78

```
What's the calculation for max erpm?
```

---
## \#14 Posted by: Jinra Posted at: 2017-06-08T00:18:16.189Z Reads: 66

```
You can use an esk8 calculator to get your intended max erpm
```

---
## \#15 Posted by: L3chef Posted at: 2017-06-08T04:31:56.254Z Reads: 60

```
:beers:  
Thanks
```

---
## \#16 Posted by: Gorfo99 Posted at: 2018-05-17T23:05:25.327Z Reads: 26

```
i have no idea how to create a new thread so im responding here and hoping for the best. When i connect my receiver to my vesc it powers on and pairs with the remote control, but my inputs have no control on the motor. I checked the servo cable and its all just as you guys said it should be. Its my first build so it might be something super simple.
```

---
## \#17 Posted by: TowerCrisis Posted at: 2018-05-18T00:16:45.254Z Reads: 22

```
You have programmed your vesc I haven't you? Make sure you've thoroughly read up on how to do so.

Also, as a brand new user you cannot start threads yet until you meet certain requirements, I forget what they are. Something about read time and time since registered.
```

---
## \#18 Posted by: Gorfo99 Posted at: 2018-05-18T00:29:48.632Z Reads: 21

```
yeah i used the bldc tool to set up the vesc, ill watch some more tutorials on it and report back
```

---

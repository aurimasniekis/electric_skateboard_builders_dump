# Programing/Reprogramming experience?

### Replies: 10 Views: 2264

## \#1 Posted by: JustACruiser Posted at: 2015-12-17T07:48:54.663Z Reads: 110

```
Hey i wanted to know if anyone knows or has experience reprogramming. I want to know if anyone can reprogram a Yuneec E-Go board to go above the speed limit they put on the board. The board tops out at a rather pathetic 12mph, i'd rather it have a max speed of around 20mph. If anyone can do this, please contact me when you get a chance
```

---
## \#2 Posted by: treenutter Posted at: 2015-12-17T13:56:28.143Z Reads: 105

```
@JustACruiser I haven't heard of anyone altering that board in this way. The drivetrain may not be robust enough to handle 20MPH. If you are really determined, though, you could replace the current ESC and [with a VESC which you can then use to control current][1] and test the limits of the board's mechanical system. You'd need to also replace the controller. 

If you look for a teardown of the E-Go you might get some better info about the ESC; perhaps it's using a standard ESC that you could connect to a programming card or standard software tool.


  [1]: http://vedder.se/2015/01/vesc-open-source-esc/
```

---
## \#3 Posted by: jakeyb2525 Posted at: 2015-12-17T22:12:37.270Z Reads: 99

```
The drivetrain is better than most 9mm DIY builds, it runs 15mm belt & pulleys and Abec clone wheels so 20mph is easily doable.

If you want to hit close to 20mph you have two options really...

* you can do what others and i have done and remove the 7s battery pack and replace it with 2 x 5s lipos in series giving you 10s 36v rather than the slower 7s 27v..more volts = more power, people have done this with no problems, mine still runs and hasnt blown up yet but its a risky mod as one person over on ES has blown there ESC

* Buy a VESC and again run more Volts and a larger 50mm motor

From my past experience i would sell it and build your own....a Turnigy 6374 motor with a 6s ESC will blow the E-go into the water in every way :+1:
```

---
## \#4 Posted by: torqueboards Posted at: 2015-12-18T05:44:45.682Z Reads: 89

```
lol go single motor DIY. Don't ruin a completely decent board :smile:
```

---
## \#5 Posted by: treenutter Posted at: 2015-12-18T13:15:18.966Z Reads: 84

```

[quote="torqueboards, post:4, topic:747"]
ol go single motor DIY
[/quote]

@JustACruiser what @torqueboards and @jakeyb2525 said ^ ! By the time you replace a motor, esc, or battery, and figure it all out, you'll pretty much have built a DIY esk8 anyway! Perhaps sell the E-go and use the cash to build something new?
```

---
## \#6 Posted by: KMeyerson Posted at: 2016-03-17T12:10:56.105Z Reads: 67

```
I've ordered a pair of the 9-Pin cables that the E-Go motor uses.

When I figure out the pinout of the motor wire, I can send you the info for using a VESC. How can I best keep in touch with you?
```

---
## \#7 Posted by: claudiofiore88 Posted at: 2016-03-17T17:48:32.128Z Reads: 64

```
The op hasn't been seen since signing up in mid December. You're not likely to reach him.
```

---
## \#8 Posted by: KMeyerson Posted at: 2016-03-22T04:06:20.566Z Reads: 64

```
For those interested, here is my replacement of the Yuneec ECU with a VESC and Wattmeter.

http://www.electric-skateboard.builders/t/yuneec-e-go-budget-upgrade/1196/41?u=kmeyerson

Running silently with FOC (stock battery and motor). When the next project needs a VESC, I'll install a new Yuneec ESC.
```

---
## \#9 Posted by: GreenF0X Posted at: 2017-03-11T15:56:27.649Z Reads: 25

```
Hello
Im planing to upgrade my ego with a vesc as well cause my esc is dead
Can you pls tell me all i need to buy to keep the original motor like you do and how to do it?
```

---
## \#10 Posted by: GreenF0X Posted at: 2017-07-25T04:47:58.866Z Reads: 14

```
Everything works fine
Still cant figure out the perfect programming :frowning:
```

---

# Max amps the battery will draw

### Replies: 5 Views: 762

## \#1 Posted by: franky0581 Posted at: 2017-09-28T16:08:03.295Z Reads: 137

```
Hello All,
I have the following motor available and use the following setup in the VESC.
My question is, how much AMPs will the controller / motor pull out of the battery at full acceleration / start.
My battery supplier is asking it to setup the BMS etc.
The battery is a 10s3p.

Here the motor type:
220kV, 1170W output max, 30A max
http://www.michobby.com/product/hot-combo-5055-220kv-sensored-motorvedder-vescremote-for-electric-skateboard/

My settings in the VESC:
Max Motor Amp: 30A
Max Batt Amp: 30A
Absolute Max: 130A

I really appreciate any feedback on this.
As I saw in some you tube videos that the max amps the battery had where above the limits that were set in the VESC configuration.

Thanks a lot in advance 
Frank
```

---
## \#2 Posted by: chinzw Posted at: 2017-09-28T16:53:12.179Z Reads: 117

```
[quote="franky0581, post:1, topic:34184"]
Max Batt Amp: 30A
[/quote]

You just typed it right there... If the builder is giving you the option, go with the highest amp rated bms he can provide.
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-09-28T17:07:02.344Z Reads: 113

```
Set your motor max to 60a or so, it'll improve low-end acceleration. What cells as the supplier using to make that pack?
```

---
## \#4 Posted by: franky0581 Posted at: 2017-09-28T18:11:35.966Z Reads: 107

```
Thanks a lot for your replies. 
Can I set the motor max to 60A even if the specification of the motor says max Amps of 30?

I understand the supplier will use 18650 cells.

Basically I would like to get a better understanding what will be the Amps the battery will roughly see at acceleration. I saw some videos on You Tube with live data-tracking and it looks like the real max values something exceed the max values that were set in the VESC by quite a bit.

Thanks
```

---
## \#5 Posted by: MysticalDork Posted at: 2017-09-28T18:19:01.402Z Reads: 98

```
Motor specifications are best taken with a few pinches of salt. I meant, what KIND of 18650 cells? Brand, capacity, discharge current? The maximum amps the battery will see are exactly what you program into the vesc, that's the whole point of programming them. The specifics of the battery will determine what you can safely program the vesc for.
```

---

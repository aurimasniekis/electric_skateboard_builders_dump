# Vesc + nano X reverse?

### Replies: 10 Views: 788

## \#1 Posted by: Bloop Posted at: 2017-06-13T22:08:44.070Z Reads: 137

```
Hi 

Right now my nano x + vesc configuration allows me to go forward and to break.
Is there a way to configure the remote so i can press a button and then the board will go backwards ?

I know there i a way to set it to go backwards but i want to keep the first configuration to forward+break and use the reverse just when i need to go back ?

Thank you
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-13T23:15:22.782Z Reads: 124

```
I actually don't think the vesc can go backwards but I could be completely off.
```

---
## \#3 Posted by: Skitzor Posted at: 2017-06-14T03:00:30.790Z Reads: 118

```
a little hint. Look in the PPM control mode for the VESC. And use search on this forum. :wink:
```

---
## \#4 Posted by: Bloop Posted at: 2017-06-14T05:07:45.091Z Reads: 108

```
@Skitzor  i did read tons of post here now and before but couldn't find anything related to what i asked.

I'll put it again: i want to know if is possible to program the vesc/nano-x so when i press one button on the remote it will change the PPM control mode from 'current no reverse with break' to something else that will allow me to go in reverse. 

And switch between this 2 modes when i need to.

Thank you.
```

---
## \#5 Posted by: yaca Posted at: 2017-06-14T08:25:33.779Z Reads: 94

```
I don't think it is possible like you want but you could try it with @ackmaniacs firmware and his android app. With the app you can switch between modes in a few  seconds. About reverse in wattmode read the first post his firmware thread.
```

---
## \#6 Posted by: SpeedSloth Posted at: 2017-06-14T10:55:25.158Z Reads: 88

```
I'd try setting the VESC to current mode and see how you get on with it. It only reverses the board once the wheels have completely stopped so it behaves as normal going forward and breaking until you actually stop.

I personally love it as it adds the reverse function and feels the same as your used to. I'd recommend you try it and see what you think.
```

---
## \#7 Posted by: Bloop Posted at: 2017-06-14T11:10:40.169Z Reads: 84

```
@SpeedSloth  Alright i will give it a try thank you.

The only problem i.ve read about this, people said is dangerous when riding and that they had problems or the board don't break nicely.  

Honestly i dont really know i will test in a few days. Till then i would love to hear more opinions from people with more experience than me. 

Thank you.
```

---
## \#8 Posted by: SpeedSloth Posted at: 2017-06-14T11:17:37.680Z Reads: 81

```
I personally noticed no difference in the breaking but that may not always be the case. Without my weight on the board you can stop the wheel and get it to skid in reverse but it's fine with me on it.
```

---
## \#9 Posted by: SpeedyGornzallez Posted at: 2017-09-12T08:59:38.921Z Reads: 54

```
did you ever find out if this was possible?
```

---
## \#10 Posted by: Bloop Posted at: 2017-09-12T09:05:55.627Z Reads: 54

```
Well i dont know if is possible to switch between the modes (maybe it is)

You should try the current mode on the vesc -> this will allow you to go forward and backward.

Or you could test the ackmaniac firmware for vesc it has a mode where if you move forward and throttle back it will act as break full break. But if you stand still and throttle back it will move back. so you have both ways to controll .
```

---

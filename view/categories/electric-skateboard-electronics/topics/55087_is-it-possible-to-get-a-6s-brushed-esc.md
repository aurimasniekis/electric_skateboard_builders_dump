# Is it possible to get a 6S brushed Esc

### Replies: 9 Views: 814

## \#1 Posted by: ricoghardforth Posted at: 2018-05-11T07:54:20.552Z Reads: 64

```

Hi 

Does any one know of a Brushed car esc which goes up to 6S and has breaking.

I've put together a cheap esk8 board for my very light 8 year old son using ebay motor mount and an old 24v brushed my6812 scooter motor.  I'm currently using an Hobbywing QuicRun WP 860 Dual Brushed 60A ESC which only goes up to 4S and the speeds topping out about 11-13MPH.  He's wanting a little bit more speed.   I'm assuming the motor will be ok up to 6S but can't find Rc car esc's with breaks that goes up to 6S.  Doesn't necessarily have to be liposised as I'm using a lipo alarm on the balance leads.
Wheels are 70mm Lush Avalanche. 48T wheel pully, 16T motor pully.

![Capture|281x499](upload://j7AZ70o5Umt1XOrK7OoFafFzUkD.PNG)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-05-11T08:05:46.216Z Reads: 56

```
I don't know of any but you may have more luck trying to search for brushed motor controller
```

---
## \#3 Posted by: b264 Posted at: 2018-05-11T08:29:44.338Z Reads: 50

```
Pretty sure the HW4.12 can do this, no problem.
```

---
## \#5 Posted by: Der6FingerJo Posted at: 2018-05-11T08:54:03.218Z Reads: 43

```
In Vesc Tool you got the option of DC Motor and it says to just use phases A and C (I think the outer 2 phases). So in theory there's nothing holding you back from using DC Motors with the Vesc.
```

---
## \#6 Posted by: Martinsp Posted at: 2018-05-11T08:56:02.110Z Reads: 41

```
Just found this thread, sorry my mistake. I will delete my reply to not confuse anyone. 
http://vedder.se/forums/viewtopic.php?t=664
```

---
## \#7 Posted by: Bor.inc Posted at: 2018-05-11T09:09:13.835Z Reads: 42

```
Did you use the MY6812 DC motor? You can try to use a normal motor speed controller that can use up to 24v
```

---
## \#8 Posted by: ricoghardforth Posted at: 2018-05-11T09:40:20.004Z Reads: 38

```
I was considering using a cheap ebay 24v scooter controller but they don't usually do dc breaking and was't sure how to interface my 2.4ghz Rc receivers ppm signal into the throttle input which is usally a hall effect sensor.

I've also been looking at 24 dc controllers but again not sure what breaking will be like and their usally controlled by a pot so not sure how to use rc receiver control.
```

---
## \#9 Posted by: Bor.inc Posted at: 2018-05-11T10:04:13.530Z Reads: 31

```
Oh aha didn't think of the breaking problem..

You can change the potentiometer on the controller with a digital potentiometer and control it with the remote via an arduino (maybe a bit complex(
```

---
## \#10 Posted by: ricoghardforth Posted at: 2018-05-11T10:09:18.125Z Reads: 27

```
I've actually got a turnigy vesc on hardware 4.10 from the kit I purchased for myself from hobby king which I'm still putting together.  I may look into using this in DC brushed mode on my sons board and then get the updated turnigy vesc at hardware version 4.12 which I see they are doing now.
```

---

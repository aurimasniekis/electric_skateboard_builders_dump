# Using VESC controller with a hubmotor ebike wheel

### Replies: 13 Views: 564

## \#1 Posted by: Silverline Posted at: 2019-04-30T15:07:20.628Z Reads: 79

```
Hallo Forum

Anybody who is using a VESC controller together with a hubmotor wheel on a ebike ??

Its going to be a 12s build (48v), and I would like to use a Throttle Hand Grip like this : https://www.banggood.com/24V-36V-48V-3-Wire-Twist-Throttle-Hand-Grip-For-Electirc-Scooter-Bike-78-Handlebar-p-1072620.html?rmmds=search&amp;cur_warehouse=CN

But is this even possible, to use with the VESC ? And what about regenerative braking, like i have on my esk8 boards, is this even possible with a handgrip ??

Thanks
```

---
## \#2 Posted by: venom121212 Posted at: 2019-04-30T15:10:42.032Z Reads: 79

```
Haha hell yeah! I used to rock one of these on my very first board. 

![image|666x499](upload://sRVK93D7Kya4ctvhUUxnsC0YYSi.jpeg) 

Check [this thread](https://www.electric-skateboard.builders/t/how-to-activate-e-brake-on-e-scooter-with-the-throttle/92226) out for some more info on the topic.
```

---
## \#3 Posted by: Silverline Posted at: 2019-04-30T15:13:52.510Z Reads: 71

```
Thanks..... not much info though.... How do these handles work..... ? I mean, on my boards i push the throttle forward to brake, how is it done with a handle in practice ?
```

---
## \#4 Posted by: venom121212 Posted at: 2019-04-30T15:20:37.813Z Reads: 71

```
Yeah they're not designed to rest in a neutral position (~50% of throttle) so they're not ideal for regen breaking setup. I was using a manual brake on that board. I'd suggest familiarizing yourself with a new throttle type. There are zero hand thottles used that I've seen in esk8.
```

---
## \#5 Posted by: trampa Posted at: 2019-04-30T15:25:31.063Z Reads: 71

```
Watch Benjamin's Youtube channel. He has a bike with two hub motors and two ADC throttles. One for acceleration, one for braking. Works a treat. 

https://www.youtube.com/watch?v=LPjsen0D2mE
```

---
## \#6 Posted by: Silverline Posted at: 2019-04-30T15:28:11.998Z Reads: 70

```
Hmm... but how is it done on a "normal ebike" ?? With those cheap chineese controllers..
```

---
## \#7 Posted by: venom121212 Posted at: 2019-04-30T15:53:16.815Z Reads: 61

```
You said you wanted to use vesc?
```

---
## \#8 Posted by: Silverline Posted at: 2019-04-30T16:05:29.830Z Reads: 60

```
Yeah... I was just wondering how reg. braking works on those cheap chinese speed controllers that often comes in the kit together with the hub Wheel.
```

---
## \#9 Posted by: venom121212 Posted at: 2019-04-30T16:09:54.293Z Reads: 55

```
On cheap hub motor setups: I believe when you use the physical brake, it electronically switches your motor to a generator, applying a small electrical resistance as well. Very inefficient regen compared to a fully electrical brake but physical brakes are necessary at higher brake loads.
```

---
## \#10 Posted by: trampa Posted at: 2019-04-30T16:55:57.006Z Reads: 50

```
They don't regen, simple as that
```

---
## \#11 Posted by: Namasaki Posted at: 2019-04-30T17:07:27.108Z Reads: 48

```
[quote="Silverline, post:1, topic:92333"]
Its going to be a 12s build (48v)
[/quote]

12s= 44v nominal. 

13s= 48v nominal

48V Ebike batteries are 13s
```

---
## \#12 Posted by: Silverline Posted at: 2019-04-30T17:56:36.280Z Reads: 43

```
Okay okay.... 44v then :-P
```

---
## \#13 Posted by: Silverline Posted at: 2019-04-30T17:58:44.604Z Reads: 43

```
Thanks guys...

Maybe i just use the mechanical brakes then....
Plan is to use this Btw. https://flipsky.net/collections/new-accessories/products/high-current-fsesc-200a-60v-base-on-vesc6
```

---

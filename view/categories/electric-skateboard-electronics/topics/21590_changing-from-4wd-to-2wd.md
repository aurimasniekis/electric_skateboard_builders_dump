# Changing from 4wd to 2wd

### Replies: 8 Views: 663

## \#1 Posted by: ieatflys Posted at: 2017-04-23T06:17:01.073Z Reads: 147

```
hello all... 

I am in the process of building a 4wd board and would like to implement the capability to switch between 4wd to 2wd.
i understand that i will probable half to come to a full stop but i have a few specific questions to ask everyone!!

I will run the front tied together with one master and same for the rear so all ill half to do is switch one bank of escs into some sort of coast mode.

My questions are....

1. Will I need to come to a full stop when switching?
2. Are the escs and motors safe to put into a coasting mode while not putting forth any work? i know if you have a typical rc car speed controller off  and coast down a hill the voltage created will blow the esc... is this the same story with the vesc?
3. How to I actually implement this? I will be using the wii nunchuck setup so instead of using z for reverse how can I go about assigning it to put the front vescs into a coast mode of some sort?\\

Hope this is not too confusing and i want to thank everyone in advance...  thank you !!!!!
```

---
## \#2 Posted by: Okami Posted at: 2017-04-23T12:45:24.192Z Reads: 124

```
@Duffman can perhaps shed a quick reply..

or @evoheyax
```

---
## \#3 Posted by: lowGuido Posted at: 2017-04-23T13:36:26.588Z Reads: 109

```
1. No, so long as all the ESCs are powered to begin with.
2. Yes. so long as all 4 ESCs powered at all times. 
3. the best way I can think of would be to have a split PWM wire for the front two and the rear two ESC's and then a switch on the PWM signal wire.
using a nunchuck probably wouldnt be ideal for this setup as you cant split the PWM easily.
```

---
## \#4 Posted by: Duffman Posted at: 2017-04-23T13:40:36.617Z Reads: 101

```
As long as the VESCs are powered up you can coast as long as you want. 

I'm using a small switch to cut the CAN connection to each of my VESCs to deacrivate them in case of a fault.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-04-23T16:58:58.701Z Reads: 81

```
I second what @lowGuido said!

Interesting idea. I just always want the most power possible, so I never thought about switching from 4wd to 2wd.
```

---
## \#6 Posted by: lowGuido Posted at: 2017-04-23T17:09:58.451Z Reads: 78

```
so I reckon that if you ditch the nunchuck and use a GT2B you could actually use one of these connected to your 3rd channel switch. switch into 4X4 whenever you like
Job done.
https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-04-23T19:37:35.137Z Reads: 66

```
You can use my firmware mod. By simply setting a lower max motor amps value then the minimum current value in the advanced tab it wouldn't power the motor. So you could use that in the front. By this it would also be possible that the the front motors still would brake. And you could comfortably switch between 4wd and 2wd by the app. 
Another advantage is that you could use 70% of power at the back wheels and 30% at the front wheels for acceleration and the other way round for braking. 
But you also could disconnect the front motors from the can bus. So the vesc will be switched on but simply idles.
```

---
## \#8 Posted by: ieatflys Posted at: 2017-04-24T01:23:45.945Z Reads: 49

```
thanks for the replys guys!!!!

i believe splitting the signal is as simple as runnning two wires from the nun chuck dongle between the banks with one esc powering the dongle from its bec...   i may just use a switch if its as simple as not giving the esc a signal...  i like that hobbyking pwm switch however what is the besc controller to do this with? i want something small like my nunchuck so i can have my hands in my pockets in the winter....

and @Ackmaniac i like this mod your mentioning... is it doable with the nunchuck? how do i go about doing this
```

---

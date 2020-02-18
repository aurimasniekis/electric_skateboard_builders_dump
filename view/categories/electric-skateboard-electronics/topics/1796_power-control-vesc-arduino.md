# Power Control VESC arduino

### Replies: 14 Views: 2419

## \#1 Posted by: Flo Posted at: 2016-03-14T08:45:03.069Z Reads: 163

```
As I'm building an electric bycicle I have to limit the longterm power output to 250 Watt to be able to drive it legally. I'll control the VESC with an arduino, will use that library: https://github.com/RollingGecko/VescUartControl and I know the rough efficiency of my motor... So to start up or to accelerate I can use as much power as I want but I must be able to limit the longterm power output. Is there any possibility to directly tell the VESC how much electric power it should send to the motor?. The only idea I had is to read out input Current and input voltage -> calculate power input -> adjust motor current until power_out < power_allowed.
I think that's a pretty dirty solution... Does anybody have a better idea?
```

---
## \#2 Posted by: trbt555 Posted at: 2016-03-14T11:03:39.574Z Reads: 161

```
You can only set the current, the RPM or the duty cycle so there is no way of setting the power directly.
You can do it externally via an Arduino as you describe, or you could write a custom application for the VESC and do the calculations in the VESC. Probably not as straightforward as it sounds though.

How is longterm power defined ?
Speed is not limited ?
```

---
## \#3 Posted by: elkick Posted at: 2016-03-14T11:11:23.606Z Reads: 148

```
Speed limiting would be easy through soft ERPM limits in the app tab.
```

---
## \#4 Posted by: treenutter Posted at: 2016-03-14T13:05:03.242Z Reads: 141

```
I've never understood why PEV laws focus on wattage. There's no way for law enforcement on the street to determine wattage without taking the device to a lab for analysis. Does anyone know why speed isn't the metric of concern, as @trbt555 asks? 

Furthermore, for us DIY'ers, it seems like figuring out the speed that a 250 Watt device can achieve, and then setting a speed cap, would be the easiest way to stay out of trouble.
```

---
## \#5 Posted by: Iceni Posted at: 2016-03-14T13:21:40.603Z Reads: 128

```
You could set the current limit in the vesc to effectively keep it below 250w, you'd have to calculate the max amps and set that as a limit.

For example, if you use a 36v battery you would end up pulling a max of 7 amps. 36v x 7A = 252W
```

---
## \#6 Posted by: Flo Posted at: 2016-03-14T13:22:14.029Z Reads: 117

```
So speed is also a matter. It is not allowed to have paddle assist on a speed over 25 km/h. So my idea would have been to set motor_current=0 if speed>speed_allowed.. 
How does ERPM behave? will it just set current = 0 at higher velocities or will it try to brake to not exceed the RPMs?
I'd like to have a moder "private property" on my bike where I will switch of all these limitations. So I don't want to set the RPM limitation in the VESC. I think it would be easier to do all that with the arduino and not VESC?
```

---
## \#7 Posted by: Flo Posted at: 2016-03-14T13:24:11.001Z Reads: 112

```
I also thought of that possibility. But I think most of the times the motor_voltage will be much less than battery voltage. So I would give away a lot of power...
```

---
## \#8 Posted by: Iceni Posted at: 2016-03-14T13:38:17.464Z Reads: 111

```
I guess the most accurate way of doing it is setting a probe somewhere monitoring the volt/amp/watt draw and hook it up to the arduino.
It's gonna add another layer of complexity to it though.
And I have no idea how one would go about implementing it.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-03-14T14:38:05.850Z Reads: 107

```
Unless you're into programming the VESC with a custom application, it would be easy to program this in an Arduino, it also allows you to keep your code independent from the VESC.

You can use the code you linked to get real-time data feedback from the VESC and control accordingly.
You have access to voltage and current so your control algorithm could calculate the power and limit it to 250W.
You have access to RPM data so your algorithm can limit max speed.
You can add an override switch to one of the digital inputs for removing the cap when you're on private property.
You could even have a small OLED dashboard.
Sounds like a fun project.
```

---
## \#10 Posted by: Iceni Posted at: 2016-03-14T15:27:23.582Z Reads: 96

```
Oh yea, the vesc can output all that data, didn't think of that.
That would certainly be easier than standalone probes.
```

---
## \#11 Posted by: Flo Posted at: 2016-03-14T15:40:04.006Z Reads: 97

```
Ok that's exactly what my plan is :) getting real time data from the VESC and do a control loop with the arduino. I'm not into programming but I can handle the arduino programming stuff. Just thought someone possibly has an easier solution... 
and it definitely is a fun project... :) 
<img src="/uploads/db1493/original/2X/9/990ad7660a7c5fa071eb81c5070103da0bcc7802.JPG" width="333" height="500">
```

---
## \#12 Posted by: trbt555 Posted at: 2016-03-14T15:41:07.811Z Reads: 91

```
What country are you in ?
```

---
## \#13 Posted by: Flo Posted at: 2016-03-14T15:42:36.515Z Reads: 91

```
I live and study in Germany - Munich
```

---
## \#14 Posted by: facepalmsareus Posted at: 2017-06-24T17:26:14.318Z Reads: 42

```
why do you have to limit it at such low wattage?
```

---

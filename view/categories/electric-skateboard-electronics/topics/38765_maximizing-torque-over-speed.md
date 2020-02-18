# Maximizing torque over speed

### Replies: 7 Views: 676

## \#1 Posted by: WeNeedTorque Posted at: 2017-11-19T18:37:09.443Z Reads: 140

```
Hi I'm trying to build a winch using a 190kv motor and vesc from diyelectricskateboards. The winch would need to lift 20 lbs. So other than some basic speed I'm trying to maximize torque as much as possible. Beyond the gearing I was hoping to get advice on how to configure the bldc tool. I found these basic settings in a tutorial but I figured they're probably not ideal for what I'm trying to do. I also have not purchased a battery yet and have been using a power source with a 3amp max so battery advice would be really appreciated. 

<img src="/uploads/db1493/original/3X/1/a/1a76448f708cd5dacb993fefaa65852039d87b41.png" width="690" height="407">
```

---
## \#2 Posted by: E1Allen Posted at: 2017-11-19T20:14:58.735Z Reads: 122

```
More details. Is it stationary? How far are you lifting the weight ect. How are you controlling the motor?
```

---
## \#3 Posted by: ugothakd Posted at: 2017-11-19T20:20:45.253Z Reads: 117

```
For max torque, it seems simple. High voltage high gearing. I'd go with a 12s battery capable of at least 50 amps. 12s * 3.7 = 44.4volts. multiple volts times amps (50) and you have 2.2kw. divide by 750watts is around 3 horsepower. Now for torque, gear it as steep as you can. You have a Max RPM of (190*44.4) 8,436.
```

---
## \#4 Posted by: Hummie Posted at: 2017-11-19T20:22:23.684Z Reads: 113

```
if you want max torque go for the lowest kv you can find.  if you're going to be winching at lowest speeds upping the motor amps would be key.  those two things will do a lot.  or gearing is another way as explained above...if you can do that.  
theres surely a formula but bet even with your 3amp supply you could get the 20lbs up if you have the right kv and enough motor amps.  or gearing.
```

---
## \#5 Posted by: WeNeedTorque Posted at: 2017-11-19T23:00:37.308Z Reads: 80

```
It is stationary and will be winching a long way about 2000m. There's a spool of width 4.5 inches attached to the motor. The motor is controlled by an arduino.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-11-20T02:48:59.773Z Reads: 67

```
turning the motor max up to 80a  will help.
You can go even higher but keep an eye on motor temp.
You can also turn the Absolute max up. According to Vedder, don't go higher than 150a. I run mine at 140a
Lipo batteries with a high C rating 60C or higher.
```

---
## \#7 Posted by: squishy654 Posted at: 2017-11-20T23:15:11.428Z Reads: 35

```
I am fascinated by the fact that you are asking to how to winch something beyond the height of the worlds tallest cliff face..what in the world are you doing? and is this a vertical environment?
```

---

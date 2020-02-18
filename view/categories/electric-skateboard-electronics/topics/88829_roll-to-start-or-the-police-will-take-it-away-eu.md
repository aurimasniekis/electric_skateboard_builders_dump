# Roll to start or the police will take it away (EU)

### Replies: 32 Views: 951

## \#1 Posted by: hornet90 Posted at: 2019-03-30T22:04:16.267Z Reads: 340

```
I have a trampa kaly built by the man him self.
Right now in dublin ireland the garda are taking electric scooters, one wheels and skateboards 
Unless you can show them that it needs a push before the motors will kick in.
So the vescs are escape .
If any one has a way of doing this let me know.
```

---
## \#2 Posted by: DEEIF Posted at: 2019-03-30T22:04:53.878Z Reads: 342

```
Depends what Vesc/esc he is using.
```

---
## \#3 Posted by: hornet90 Posted at: 2019-03-30T22:11:23.944Z Reads: 334

```
http://www.electric-skateboard.builders/t/hw6-4-based-esc-escape/37579

Escape hw 6.4
```

---
## \#4 Posted by: anorak234 Posted at: 2019-03-30T22:12:27.822Z Reads: 326

```
Easiest way I can think of is to unplug the sensor cables on your motors. That way it won’t move until you give it a push.
```

---
## \#5 Posted by: rusins Posted at: 2019-03-30T22:14:18.511Z Reads: 321

```
What? That sounds like a very strange rule to have, but I guess it's safer that way. Some people in the push to start switch tread https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879 have had a faulty batch where the switch would turn off instantly when the wheels weren't spinning. Although it's bad for them, this would be perfect for you :smiley: You could try reaching out to see if someone would sell you their broken one.
```

---
## \#6 Posted by: hornet90 Posted at: 2019-03-30T22:30:18.800Z Reads: 312

```
If you dont need to push with your foot you need road tax but you cant get that. Its a mpv
```

---
## \#7 Posted by: pat.speed Posted at: 2019-03-30T22:32:21.566Z Reads: 300

```
I agree with above, get a push to start switch and ask the creator @Martinsp if he could custom code yours so that it turns off within a few seconds that the wheels stop
```

---
## \#8 Posted by: Andy87 Posted at: 2019-03-30T22:34:05.319Z Reads: 288

```
That’s going to be fun at each street corner you need to stop a second to look if a car is coming from the other side 😂
```

---
## \#9 Posted by: Balta_6 Posted at: 2019-03-30T22:42:24.659Z Reads: 277

```
You can setup the shut down speed yourself, I don't know if such a short time is possible though
```

---
## \#10 Posted by: DEEIF Posted at: 2019-03-30T23:26:39.842Z Reads: 262

```
I changed the title so people recognize it more :wink:
```

---
## \#11 Posted by: pat.speed Posted at: 2019-03-30T23:38:38.216Z Reads: 250

```
I prefer to kick off when starting anyway. It feels more natural
```

---
## \#12 Posted by: rusins Posted at: 2019-03-31T01:39:48.251Z Reads: 228

```
minimum time is 5 minutes according to the calculator Martin has online
```

---
## \#13 Posted by: BigZwatt Posted at: 2019-03-31T02:06:25.757Z Reads: 216

```
I changed your title slightly.  It seemed click baity the way it was.
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-03-31T02:09:18.829Z Reads: 213

```
All the turning on and off is only going to kill it faster as well :man_shrugging:

really seems like a lose lose situation x.x
```

---
## \#15 Posted by: Andy87 Posted at: 2019-03-31T03:35:50.258Z Reads: 199

```
Yeah but keep in mind it takes 5-10s till your escs run again and have connection to your remote. Means each time you stop it takes 5-10s till everything works again.
```

---
## \#16 Posted by: Pedrodemio Posted at: 2019-03-31T04:40:15.514Z Reads: 191

```
You could put an arduino between the receiver and the VESC, connected to it via UART, would be a pretty simple code 

Basically the arduino will read the ERPM from the VESC and only allow throttle if is turning above a set rpm, brakes would always work for safety
```

---
## \#17 Posted by: pat.speed Posted at: 2019-03-31T04:45:31.812Z Reads: 183

```
Does it really take that long? Mini remote connects within 2 sec very time
```

---
## \#18 Posted by: Vanarian Posted at: 2019-03-31T05:03:49.884Z Reads: 179

```
What @Pedrodemio said. Reliable and cost effective too. And turning on / off a switch repeatedly could be risky given the failure rate of current AS modules ? 

BTW is it possible via VESC-TOOL to set an ERPM dead zone under which the board doesn't react to remote input?
```

---
## \#19 Posted by: ZachTetra Posted at: 2019-03-31T05:20:57.022Z Reads: 172

```
Put a tiny "alternator" on the drive motor and a transistor in the data line from the remote, if the motor RPM is to low the voltage will not be enough to pass the remote data and you won't accelerate, this may also be an awful idea but it's cheaper than an aduino and much simpler
```

---
## \#20 Posted by: hornet90 Posted at: 2019-03-31T06:51:04.085Z Reads: 164

```
On the kaly i have to pair the remote every time it powers on.
The vescs need to have power allthe time or i wonder does the receiver only need ti have power all the time
```

---
## \#21 Posted by: ninja Posted at: 2019-03-31T07:04:09.623Z Reads: 151

```
Just use PID acceleration with brake control. Use Ackmaniac app, make some different modes and one of them PID..... so when police asks, just switch to PID mode. It's like hybrid between electric and push board. So u start with pushing, than press fully throttle and board will maintain same speed how hard u pushed. Brakes also works on this mode.
```

---
## \#22 Posted by: hornet90 Posted at: 2019-03-31T07:40:31.393Z Reads: 137

```
I will look at that now, i use that app all the time
```

---
## \#23 Posted by: b264 Posted at: 2019-03-31T07:55:28.987Z Reads: 135

```
The best way to do this is to modify the VESC firmware to have a new mode for this in the "App" section.
```

---
## \#24 Posted by: pat.speed Posted at: 2019-03-31T08:47:32.082Z Reads: 131

```
I like the idea but this would need some additional parts. The main one being a voltage reg to stop overvoltage at high rpm. It will also put more rolling resistance on the drive train and take up added space on the drive train.
```

---
## \#25 Posted by: Andy87 Posted at: 2019-03-31T08:54:56.191Z Reads: 128

```
My focbox need min 2sec as well to power up.
Idk I just think for me it wouldn’t be comfortable like this driving in the city and traffic. It’s a lot of stop and go and the moment you push, thsn push the trigger expect the board to accelerate but it doesn’t because it’s not ready yet and than two seconds later when you already don’t expect anything it starts to shoot out under your feet.
I think it takes a lot of practice to drive save like that. But not saying it’s not possible, just not convenient.
```

---
## \#26 Posted by: hornet90 Posted at: 2019-03-31T09:45:49.249Z Reads: 119

```
The remote and vesc would need to be on all tbe time
```

---
## \#27 Posted by: ninja Posted at: 2019-04-02T19:48:34.611Z Reads: 83

```
So, did you tried PID control?
```

---
## \#28 Posted by: Acido Posted at: 2019-04-02T20:01:44.295Z Reads: 82

```
just use the eswitch with the push to start function
```

---
## \#29 Posted by: hornet90 Posted at: 2019-04-07T08:51:07.720Z Reads: 81

```
I tryed it its not great ill look at it again today
```

---
## \#30 Posted by: hornet90 Posted at: 2019-04-07T08:53:06.872Z Reads: 79

```
That might not work with my kaly you have to bind the remote every time you turn the board on
I have email the lad who makes that switch im waiting for a reply
```

---
## \#31 Posted by: Deodand Posted at: 2019-04-07T14:27:02.724Z Reads: 57

```
This would just be a simple firmware adjustment via custom app. Very easy to code actually, essentially you could look at the app_ppm.c and under current control you just need to something like 

     if(mc_interface_get_rpm() > 1000)
      Send current to motors

    Else
      Send no current


Then make sure to do that only for current commands greater than 0 also.
```

---
## \#32 Posted by: Tangent Posted at: 2019-04-07T19:49:43.157Z Reads: 38

```
@Deodand, any plans to implement thus on the  Unity on a future release? Could be very handy for us folk in Ireland..

I had heard the reports of scooters being sized in Dublin, and assumed this would probably not be isolated to only scoots, so checked the law and it does appear that a push to start may exempt a skateboard, see below, though not sure it is completely black and white:

 What is the law on e-bikes / pedelecs / battery powered scooters? Regardless of the type of bike, the rule is as 
follows: If it can be powered by mechanical or electrical power alone (i.e. it can go without you pedalling or scooting 
it) then it is considered to be a mechanically propelled vehicle (MPV). Under Road Traffic Law, if an MPV is used in a 
public place it is subject to all of the regulatory controls that apply to other vehicles. Therefore, it must be 
roadworthy, registered, taxed and insured. The driver of the vehicle must hold the appropriate driving licence and is 
obliged to wear a crash helmet. 

What is the definition of ‘mechanically propelled vehicle’? The Road Traffic Act 1961 at Section 3(1) (a) and (b), 
defines a mechanically propelled vehicle as: “a vehicle intended or adapted for propulsion by mechanical means, 
including:
(a) a bicycle or tricycle with an attachment for propelling it by mechanical power, whether or not the attachment is 
being used,
(b) a vehicle the means of propulsion of which is electrical or partly electrical and partly mechanical, but not 
including a tramcar or other vehicle running on permanent rails.”
```

---

# Remote controlled light switch

### Replies: 10 Views: 1524

## \#1 Posted by: florensvb Posted at: 2017-07-15T13:27:40.250Z Reads: 218

```
Hey guys,

I have bought [this remote.](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-nano-remote-controller/)

And also [these lights here.](https://hobbyking.com/en_us/hobbyking-1-5-and-1-8-off-road-led-light-set-with-functional-brake-lights.html)

I think connecting the lights to the remote receiver should be pretty much plug'n'play but I also want to achieve that I can turn the lights on and off from the remote, if possible.

Any ideas?

Cheers!
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-07-15T13:32:10.720Z Reads: 216

```
You will likely get more response if you will post your components within the thread. Type out what each item is or upload a picture within the post.
```

---
## \#3 Posted by: Martinsp Posted at: 2017-07-15T16:36:56.843Z Reads: 193

```
Hey! 

I dont have the remote but there is one channel for your throttle, the connector has 3 wires so signal and power from ESC/VESC and one channel that is switched by the receiver based on the input from the second channel from your remote. So to be able to turn the lights on and off from your remote you will have to take power from the output of that second channel on your receiver and to achieve the brake lights you will have to take the signal from the remote going to the ESC/VESC and connect that to the signal input on the wire of your lights.
```

---
## \#4 Posted by: Ishayc Posted at: 2017-07-18T09:08:31.453Z Reads: 167

```
Hi!

In order to control the lights from the 2nd channel on your remote you need to have a Receiver Controlled Switch.
For example:
https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html

just connect the Receiver Controlled Switch to the 2nd channel on your receiver.

Notice: If you want to connect it to the eboard battery make sure the Voltages are the same. If you are planning on connecting it to a diff battery you need to make a common ground between the receiver power source(the eboard battery) and the Lights one otherwise it will not work.

 If you need help with the wiring PM me.
```

---
## \#5 Posted by: florensvb Posted at: 2017-07-18T21:19:16.807Z Reads: 138

```
Hey thanks a lot for your answers! Okay so basiclaly i just need that remote controlled switch and i am good to go. 

About powering the lights, i was actually thinking to use the vescs in built power supply directly through the receiver. i read somewhere that this should work, but i am not at home to check where. Do you think that would be possible? i bought this vesc

 diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
```

---
## \#6 Posted by: jmasta Posted at: 2017-07-18T23:15:59.955Z Reads: 132

```
I have remote-controlled lights on my board, using the R/C switch linked above. I've actually had it working for months but have been too busy finishing grad school to post my build thread

The switch needs a power supply under 30V, so anything above 7S won't work directly from pack voltage.  I use a 12V BEC for the lights and also the switch.  But you could use the 5V buck converter from the VESC. Just plug a servo cable into an unused port on your receiver (5V is middle pin, Ground is opposite of signal pin)

http://www.fatlion.com/sailplanes/images/jrconnector.png

That said, I haven't found the R/C light switch to be too terribly useful. Typically you know before riding if you need lights or not.  The only exception would be flashing your lights to alert careless drivers..  But overall, a mechanical switch on the board for the lights is all you need.  The RC switch would be better served for a function like an electronic horn
```

---
## \#7 Posted by: florensvb Posted at: 2017-07-19T08:41:19.400Z Reads: 122

```
Hey thanks for the reply! I guess i could live with not having the switch because i actually use an 8S pack.. but can i power the lights straight from the vesc and what kind of mechanical switch should i get? :)
```

---
## \#8 Posted by: florensvb Posted at: 2017-07-19T19:09:12.281Z Reads: 116

```
So as i understand, i can just plug in that switch into a free channel / port on my receiver. i can then just plug in the lights into the switch and it will work? 

sounds too easy- what am i missing?
```

---
## \#9 Posted by: mmaner Posted at: 2017-07-24T21:46:43.633Z Reads: 108

```
<img src="/uploads/db1493/original/3X/3/9/3996bac8c7c975ea51ac2c1fd54dc4d5ba8e7f42.jpg" width="533" height="407">
```

---
## \#10 Posted by: composites_r_awesome Posted at: 2018-07-06T11:47:23.144Z Reads: 61

```
Hei! Talking about electric alerting device - I looked up good ol' taobao and the likes but only found electric horn with terrible, like overcharge-lipos-burn-your-house-down terrible sound options. There are no classical _dring-dring!_ ones available afaik. I would Love to have a classical bike bell sound, [something like this](https://youtu.be/IjoePLT_cFw). Would be even better if we could use those mini 2€ audio players with memory card input and get them working remotely, playing 1-time the sound on demand or a loop or something...  
Thing is people instinctively know the ringing sound and it's not so 'intrusive' as something like ...
 [...this.](https://youtu.be/QQqGwM13Yy4?t=19s) 
breaking glass has more rhythm than that.. Ooor maybe, just maybe, we could upload our own files there?
```

---

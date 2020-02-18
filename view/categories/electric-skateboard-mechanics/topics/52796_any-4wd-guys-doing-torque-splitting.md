# Any 4wd guys doing torque splitting?

### Replies: 33 Views: 1339

## \#1 Posted by: evoheyax Posted at: 2018-04-19T17:27:29.885Z Reads: 185

```
Title says it all. I'd love hear any results as this is something I've been looking into.
```

---
## \#2 Posted by: Hummie Posted at: 2018-04-19T17:30:12.003Z Reads: 185

```
What's torque splitting
```

---
## \#3 Posted by: trancejunkiexxl Posted at: 2018-04-19T17:31:48.675Z Reads: 181

```
Ya tell me more, is this can bus stuff?🤣
```

---
## \#4 Posted by: E1Allen Posted at: 2018-04-19T17:33:35.679Z Reads: 178

```
It's when one engine on my Blackhawk provides more torque to the main transmission than the other engine
![IMG_4823|281x500](upload://9G4gVzNI1F0sdSAl1jxFHUQtXgJ.jpg)
```

---
## \#5 Posted by: evoheyax Posted at: 2018-04-19T17:48:02.940Z Reads: 174

```
The better name might be watt splitting. The key is I have a certain amount of watts I can put through the wheels (due to li-ion battery limit), do you then push more through either the front motors, the back motors, or even?

On more exspesive 4wd cars for example, they will send 80% torque to the rear and 20% torque to the front in sport mode. In other cases, it might be the opposite. I’m just curious if anyone’s messed around with the idea of splitting torque between motors un evenly in this sense.
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-19T17:53:01.141Z Reads: 172

```
Try instead of making 4 vesc independently try can bus making it just 2 vesc with traction control and 2 receivers  one remote ? Idk maybe limiting back vesc to 40amps and front to 80?
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2018-04-19T17:53:16.569Z Reads: 166

```
what if u use different motor max in front and rear, same effect? just curious
```

---
## \#8 Posted by: E1Allen Posted at: 2018-04-19T18:10:51.145Z Reads: 158

```
That makes sense.  Still going to have same maximum rpm all other considerations aside
```

---
## \#9 Posted by: pakue Posted at: 2018-04-19T18:33:07.564Z Reads: 151

```
Isn't this mainly done to keep traction during acceleration?
```

---
## \#10 Posted by: Ackmaniac Posted at: 2018-04-23T00:05:35.305Z Reads: 130

```
You can try it with my firmware mod 3.101. Different power ratio is also adjustable via my app, there you can select the settings for the front truck individually. And the throttle signal is shared to all motors instead of the current like in the original firmware. this way you can give each motor a different setup.
So a battery max setting of 60A at the front and 40A at the back will result in 60% power at the back and 40% power at the front.
```

---
## \#11 Posted by: Cobber Posted at: 2018-04-23T00:16:31.229Z Reads: 127

```
[quote="Ackmaniac, post:10, topic:52796"]
So a battery max setting of 60A at the front and 40A at the back will result in 60% power at the back and 40% power at the front.
[/quote]

So 60A at the front = 40% power & 40A at the rear = 60% power that hurts my head bro can you give another example is it inverse or... ?
```

---
## \#12 Posted by: Ackmaniac Posted at: 2018-04-23T00:45:19.590Z Reads: 114

```
[quote="Ackmaniac, post:10, topic:52796"]
So a battery max setting of 60A at the front and 40A at the back will result in 60% power at the back and 40% power at the front.
[/quote]

Sorry mixed it up, correct is:

So a battery max setting of 60A at the back and 40A at the front will result in 60% power at the back and 40% power at the front.
```

---
## \#13 Posted by: Cobber Posted at: 2018-04-23T00:49:41.666Z Reads: 111

```
Gotcha bro, that hurts my head less :exploding_head:
```

---
## \#14 Posted by: evoheyax Posted at: 2018-04-23T00:56:20.117Z Reads: 108

```
When I accelerate my wheels slip. So I need more traction haha.
```

---
## \#15 Posted by: E1Allen Posted at: 2018-04-23T01:06:52.929Z Reads: 108

```
What size wheels? @evoheyax
```

---
## \#16 Posted by: evoheyax Posted at: 2018-04-23T01:29:35.246Z Reads: 115

```
83mm. Running current control mode and latest firmware and it delivers one hell of a ride. Jumps and slips wheels but once they catch, man it’s a rocket.
```

---
## \#17 Posted by: Pedrodemio Posted at: 2018-04-23T01:37:44.582Z Reads: 112

```
Have you tried traction control? This video from Jed is quite impressive

https://www.instagram.com/p/BbY9uEqnds6/?taken-by=jedboards
```

---
## \#18 Posted by: evoheyax Posted at: 2018-04-23T02:31:31.561Z Reads: 111

```
I’ll try it cause I haven’t. But I’d imagine it might hurt the acceleration in the end by cutting too much power.
```

---
## \#19 Posted by: Pedrodemio Posted at: 2018-04-23T03:21:41.057Z Reads: 108

```
I still have to play with it, but I think by setting the rpm that it comes into play you can tune how much slip you want to allow to maximize acceleration
```

---
## \#20 Posted by: E1Allen Posted at: 2018-04-23T05:39:07.481Z Reads: 101

```
Bigger wheels though! Less slippage.
```

---
## \#21 Posted by: banjaxxed Posted at: 2018-04-23T09:22:04.356Z Reads: 86

```
I guess different kv front and rear, they have to stay the same on each end to avoid torque steer, v4 there is a possibility to use mixed kv

https://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---
## \#22 Posted by: Ackmaniac Posted at: 2018-04-23T10:08:31.630Z Reads: 78

```
Maybe i need to explain a bit better and compare the original firmware to my firmware.

Original: 
Back Motor max 60A
Front Motor max 40A
At 50% throttle the back will get 30A and the front 30A // current if master is shared
At 75% throttle the back will get 45A and the front 40A // current if master is shared but front reached limit
At 100% throttle the back will get 60A and the front 40A // current if master is shared but front reached limit

My firmware mod 3.101:
Back Motor max 60A
Front Motor max 40A
At 50% throttle the back will get 30A and the front 20A // throttle is shared so front wil use 50% of it's own motor max current
At 75% throttle the back will get 45A and the front 30A // throttle is shared so front wil use 50% of it's own motor max current
At 100% throttle the back will get 60A and the front 40A // throttle is shared so all in

For the brakes it works the same. So with my firmware mod it would be possible to have a precise ratio of front and back. (in the example it is 40:60)
```

---
## \#23 Posted by: evoheyax Posted at: 2018-04-23T14:54:19.425Z Reads: 69

```
I have to say for the price point, that 4wd jed board is impressive. But I've done similar things with hummie hubs with no slipping issues without traction control. I just don't full throttle, lol. I have a bigger surface area than pretty much anyone else, since you can't belt drive a centrax wheel. Should mean more traction, which is the key to a strong acceleration. It's tough because once I get traction, I'm gone.

My whole goal of this thread was to see if putting more torque one way or another helped traction to get a good acceleration without reducing power.
```

---
## \#24 Posted by: Pedrodemio Posted at: 2018-04-23T15:22:16.314Z Reads: 67

```
I would try the @Ackmaniac aplit function. When you accelerate you have a load transfer to the rear wheels, how much is hard to calculate since the rider stance is a big influence in it

What i would do:
- find a street with consistent pavement and with no dirt to provide a constante traction
- use a camera, preferable  with slowmo'ish capability to record the board from the side, you can try to do this by feeling the wheels spin
- floor it without torque split to see what is slipping, if its just the front wheels reduce the split to them until no slip occur

Do the wheels also spin when at speed? say flooring at 10 km/h

For launch you don't maximum torque that the system can gives, you want maximum torque that  the friction with the street can sustain without slip. Slip = dynamic friction coefficient, that is lower than the static one
```

---
## \#25 Posted by: barajabali Posted at: 2018-04-23T15:25:48.286Z Reads: 62

```
Where can I get you 3.101 fw/tool. for my 2 4wd Trampas
```

---
## \#26 Posted by: SeanHacker Posted at: 2018-04-23T15:29:30.846Z Reads: 61

```
Here it is. When you open the tool you can select the firmware you need. 

https://www.dropbox.com/sh/t7dl90owz5ccbyl/AAB7h8PuyUZ1Mk3Oya3USscla/ACKMANIAC-ESC-Tool_3_101?dl=0
```

---
## \#27 Posted by: barajabali Posted at: 2018-04-23T15:29:51.994Z Reads: 61

```
Thanks buddy!
```

---
## \#28 Posted by: evoheyax Posted at: 2018-04-23T15:31:42.583Z Reads: 62

```
Any idea why I was getting really poor performance from watt control vs current control?

Used same settings to a tee. But watt control was maybe 60% the power that current control is giving me right now. Wheels never slipped in watt control, but do in current control, and the acceleration in general is way better with current control. Would love to know why cause watt control is way smoother than current control and I'd prefer to run it. Just can't sacrifice 40% of my acceleration for it though.
```

---
## \#29 Posted by: E1Allen Posted at: 2018-04-23T16:46:50.960Z Reads: 62

```
Isn't that because watt control is more limited than current Control.  Your board will output higher Max Watts on a full battery vs a 20% battery.  But if you limit the watt output you basically tell it to draw less current therefore not as punchy or fast potentially.
```

---
## \#30 Posted by: Ackmaniac Posted at: 2018-04-23T19:04:03.268Z Reads: 58

```
You can achieve the same power output as current control. Actually exactly the same. You simply need to pull the trigger more.
I know you are using very high motor max and relatively low battery max. This way you give full power in current control even if you pull the trigger only a bit. In watt control you have the full range at all times.
```

---
## \#31 Posted by: Hummie Posted at: 2018-04-23T19:08:38.040Z Reads: 53

```
i tried @evoheyax board in watt control and it didnt have nearly the torque it had before.  unexplained.  I hit trigger all the way.  It's a long story and maybe it has to do with the new motors being wye vs delta?  otherwise i think they were almost the same...except maybe a hair less battery amps

but i thought the standard traction control on the vesc would stop any spinning wheels at startup.  it wont let one wheel spin out in slippery stuff or on a sharp turn.
```

---
## \#32 Posted by: Ackmaniac Posted at: 2018-04-23T19:34:57.363Z Reads: 54

```
Which watt and amp setting did you use define? 
Because finally the power output is exactly the same at full throttle when the settings are right.
Current control only feels stronger because you have less trigger to control the power output, but it all depends on the settings.
```

---
## \#33 Posted by: Hummie Posted at: 2018-04-23T19:37:43.989Z Reads: 53

```
i dont know and it's @evoheyax board, but he said he used watt control both times and we're trying to figure why it would put out less torque or power.   dont know much other than i pulled the throttle all the way.   dont even know for sure what luke was set at.
```

---

# Motor Size vs KV

### Replies: 24 Views: 1643

## \#1 Posted by: IsTalo Posted at: 2017-02-26T12:59:39.845Z Reads: 182

```
Hello, I have a Alien 42mm motor that have 300kv, but I saw a lot of guys on youtube that people use motors 50mm size that have 430kv (Like Great Scott) and Go fast and have power. Everybody said that my motor will blow, I'll test it, But @Vieo uses one and said that works perfectly, but now is my question, does Motor size matter? Or it's just Kv?
```

---
## \#2 Posted by: Sander Posted at: 2017-02-26T14:12:05.502Z Reads: 171

```
What do you mean with motor size? Btw can you give me the specs of your motor?
```

---
## \#3 Posted by: IsTalo Posted at: 2017-02-26T14:23:24.941Z Reads: 170

```
[quote="Sander, post:2, topic:18271"]
Btw can you give me the specs of
[/quote]

I mean like, my motor is 4260 so it is 42 mm diameter, sk3 6374 have 63mm diameter.
Specs: 300kv 1500w 6s
```

---
## \#4 Posted by: Sander Posted at: 2017-02-26T15:01:45.668Z Reads: 168

```
[quote="IsTalo, post:3, topic:18271"]
1500w 6s
[/quote]

6S Max volt ~25.2V

1500W / 25.2V = ~60A

So the motor should be fine to use. As long as you do not exceed 60A with a 6S battery. 
So you could set max Amp in the VESC to 55A. And everything should work just fine ;)
```

---
## \#5 Posted by: Hummie Posted at: 2017-02-26T15:03:21.714Z Reads: 157

```
Motor size is more important than kv. You can adjust the voltage and pulleys with different kv motor but if the motor isn't big enough it won't have the power needed and will run slower relative to what it should be going with a given input (relation to no-load speed) and get hotter. Possibly too hot and damage the magnets.  So too small for the load makes it inefficient and will get hotter with less load and it also has less mass to begin with where that heat could disipate to. Bigger is better.  An easy test to see if ur motor is at MAXIMUM efficiency would be to drag the motor around unpowered at the speeds u intend to do. It will get warm even unpowered. It will still experience almost all its same iron losses as it would powered. When you get half the temp increase from these switching losses, iron losses, as you get at the same speeds when self powered, then you losses are balanced between iron and copper and you'll likely have as an efficient size as the motor design will allow.
```

---
## \#6 Posted by: IsTalo Posted at: 2017-02-26T15:03:57.141Z Reads: 149

```
Man, but I wanna know, Does a Small motor 42mm, will have troubles?
```

---
## \#7 Posted by: Sander Posted at: 2017-02-26T15:04:30.380Z Reads: 144

```
[quote="Hummie, post:5, topic:18271"]
Possibly too hot and damage the magnets.
[/quote]

Dont think so if he limits the amp the motor will be just fine. But bigger motors are better.
```

---
## \#8 Posted by: IsTalo Posted at: 2017-02-26T15:08:09.851Z Reads: 139

```
Understood, I'll give this motor a chance, especially because it was 39 pounds and more 29 pounds for shipping, when it blow I'll change for your hub motors, theyre great
```

---
## \#9 Posted by: Hummie Posted at: 2017-02-26T15:13:48.285Z Reads: 136

```
4260 size depends on the brand and it could be a 52mm motor if scorpion maybe or as small as a 42mm diameter of measured differently. 
Power or amp ratings are not a reliable indicator of power ability. They doesn't incorporate ambient temperature but instead likely assume you're flying a plane with the motor on some freezing day. 60amps continuously to the motor and it will die. At what temps will the motor magnets die: The Currie number.  Who knows as most motor sellers of cheaper motors don't want to tell u the magnet's max temp ability as the higher heat mags are more expensive.  Probably the most important number for a motor to survive.
```

---
## \#10 Posted by: Hummie Posted at: 2017-02-26T15:25:05.005Z Reads: 133

```
But u likely won't be hanging around doing 50 amps continuously, or 60, anyway and likely will be fine.  Temp decides it. So u can do many more amps and set your vesc higher than 60 battery amps if u want..as long as the motor doesn't get too hot (mystery temp but if u stay under the max for standard niodimium mags..forget what it is but search ) then you're fine. Also the vesc has a temp sensor in it to self shut down if it gets too hot as well which is nice 

Setting your vesc settings you could set the battery amp max to much higher than 60 really and the limit would be what ur cells could put out.  Forget what they are. But the motor amp limit...set it to 200!!! You'll be fine and there's a lot of confusion as to how it works. And max to 200 as well.  Really u should research a bit to find the math to get u an even acceleration or u could just start at 200 motor amps and maybe 40 battery and work the battery number up as u like.  This will give u the most slow speed acceleration and least amount of cogging and more
```

---
## \#11 Posted by: Iceni Posted at: 2017-02-26T18:34:59.408Z Reads: 105

```
That motor may be a bit on the small side.
It should work if geared down a bit and used mainly on flats/light hills though.
Bigger hills might be problematic.

With 6s and 13/36 gearing with 76mm wheels will still get you up to around 30km/h on flats.
```

---
## \#12 Posted by: IsTalo Posted at: 2017-02-26T18:43:27.028Z Reads: 102

```
[quote="Iceni, post:11, topic:18271"]
13/3
[/quote]

I use a 16/36 with 71mm wheels, But I will change for Hummies Hub motor in the future
```

---
## \#13 Posted by: Iceni Posted at: 2017-02-26T18:54:20.343Z Reads: 96

```
Cool.
Didn't know you already had it assembled.
If the motor gets too hot to touch during a ride, try gearing it down and it'll have an easier time. 
If you have a smaller pulley that is :)

Might not even be worth it if you plan on switching to hubs anyway.
```

---
## \#14 Posted by: IsTalo Posted at: 2017-02-26T19:06:07.647Z Reads: 89

```
Yeah, I'll use this 42mm motor until july, that I'm going to NYC and will buy another Vesc and a Hub motor
```

---
## \#15 Posted by: Dornacht Posted at: 2017-02-26T22:35:22.633Z Reads: 80

```
The biggest problem will be braking because of the reduced gearing and the small size , have a scorpion 5030 single and excels at everything except braking, witch is hard for belts anyways especially on inclines
```

---
## \#16 Posted by: IsTalo Posted at: 2017-02-26T23:03:34.645Z Reads: 77

```
But it is not a great problem, I just afraid of my motor don't get me where I want..,
```

---
## \#17 Posted by: tonystark Posted at: 2017-02-27T02:05:23.694Z Reads: 73

```
[quote="IsTalo, post:1, topic:18271"]
Great Scott)
[/quote]

hey man. i also have alien motor. does your have colored wires? mine has 3 black wires and no markings. i have no idea how to connect. can you help please?
```

---
## \#18 Posted by: IsTalo Posted at: 2017-02-27T02:22:53.549Z Reads: 70

```
Hi Sir, first, Mine are Colored, But On Esc you can conect with the order you want, it don't matter, and if the motor spins in the wrong way you just change two wires, fine?
```

---
## \#19 Posted by: Namasaki Posted at: 2017-02-27T22:56:58.550Z Reads: 71

```
[quote="Hummie, post:5, topic:18271"]
Bigger is better
[/quote]


I believe this is a good rule of thumb for e-board motors.
Size matters because torque matters.
```

---
## \#20 Posted by: saul Posted at: 2017-02-28T23:24:22.308Z Reads: 64

```
I think i've seen someone use a 42mm motor a long time ago.
it will work for a while, but it will have much much less torque. probably no hills. but i'm sure it could keep you rolling on flat....

my very first attempt i used a tiny 50mm. I think 50/50. the stator was a 4020. about half as long as the usual 5065.
it did fine up to 15mph. but it was a custom 85kv on 12s!

larger motor diameter increases torque more than length. 6355 motors are probably the best all around motors right now because of vesc power limits. 50's are cool for duals but can handle some hills pretty well on  single...

the real thing with smaller motors is the shaft is usually 6mm or less. easy to bend :head_bandage:
```

---
## \#21 Posted by: IsTalo Posted at: 2017-02-28T23:26:37.196Z Reads: 62

```
True again, I will test mine, In Brasilia (Brasil capital) we don't have hills, is a planned city so everything is flat... But I think I'm going to buy Hummies Hub Motor, do you think they work good with 6s?
```

---
## \#22 Posted by: saul Posted at: 2017-02-28T23:42:29.763Z Reads: 55

```
most hubs are setup for 12s. to keep current/heat down.
torque is addictive. just leave room to grow. its crazy how fast you can get used to this stuff.:sunglasses:
```

---
## \#23 Posted by: IsTalo Posted at: 2017-03-01T00:09:49.026Z Reads: 55

```
[quote="saul, post:22, topic:18271"]
torque is addictive. just leave room to grow. its crazy how fast you can get used to this stuff
[/quote]

Oh, fine, I will need to buy another 6s pack, I have one that is 6300 mah, do I need buy one with 6300 mah too?
```

---
## \#24 Posted by: Iceni Posted at: 2017-03-01T14:36:54.831Z Reads: 53

```
Yes, you'll want to use the same type of battery as the other one.
```

---

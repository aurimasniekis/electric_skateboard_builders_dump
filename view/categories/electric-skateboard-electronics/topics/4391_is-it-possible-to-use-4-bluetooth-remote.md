# Is it possible to use 4$ bluetooth remote?

### Replies: 20 Views: 1593

## \#1 Posted by: Hillso Posted at: 2016-06-07T13:37:17.119Z Reads: 211

```
Is it possible to use this 4$ bluetooth [joystick](http://www.aliexpress.com/item/2016-Universal-Bluetooth-Remote-Controller-wireless-Gamepad-Mouse-Mini-Wireless-joystick-For-Samsung-Android-iOS-VR/32610332492.html?spm=2114.10010108.1000014.3.tGxH0s&scm=1007.13338.33346.0&pvid=87165ef8-9980-4445-9640-4ddc59c5e488&tpp=1) with this bluetooth [receiver](http://www.aliexpress.com/item/HC-06-Bluetooth-serial-pass-through-module-wireless-serial-communication-from-machine-Wireless-HC06-for-arduino/32284764842.html?spm=2114.30010308.3.10.V56ZuZ&ws_ab_test=searchweb201556_7,searchweb201602_4_10037_10017_507_10032_401,searchweb201603_3&btsid=abb0dce2-c31e-44ec-961c-8e9e5c2b4ec9) and [Arduino nano](http://www.aliexpress.com/item/free-shipping-for-Arduino-Nano-V3-0-controller-ATMEGA328P-ATMEGA328-original-CH340-USB-cable/32595285450.html?spm=2114.30010308.3.11.i5jrqb&ws_ab_test=searchweb201556_7,searchweb201602_4_10037_10017_507_10032_401,searchweb201603_3&btsid=fbcba2dd-4f4d-4e0a-941a-6a93b5c1a41a)?
or with different configuration.
Thanks.
```

---
## \#2 Posted by: Karmannghiagirl Posted at: 2016-06-07T13:37:56.257Z Reads: 211

```
technically, anything is possible :grin:
```

---
## \#3 Posted by: Hillso Posted at: 2016-06-07T13:42:19.418Z Reads: 209

```
I don't like your answer :slight_smile: 
are you suggesting it is not practical?
thanks.
```

---
## \#4 Posted by: Maxid Posted at: 2016-06-07T13:44:21.946Z Reads: 204

```
if you actually want to do an arduino project with digital signal to PWM conversion why don't you just check out the wii nunchuck and try to modify its receiver signal to output a suitable PWM signal? That would be a real contribution.
```

---
## \#5 Posted by: Karmannghiagirl Posted at: 2016-06-07T13:48:39.882Z Reads: 195

```
You asked if it was possible, i said it is :smile:
 
For real though, you could make a sweet controller if you did that. you could add in an lcd like the new evolve one. maybe add in some additional features. It would be a good project.

Now, if you want something that just works, either get an RC controller, a nyko wii nunchuck and modify it, or get the steeze (i think thats what its called) remote from enertion or some other place online.
```

---
## \#6 Posted by: trbt555 Posted at: 2016-06-07T15:02:18.248Z Reads: 172

```
I tried exactly that. 
There is a phletora of similar remotes available from China.
I ordered a few and connected them to my Arduino and generated a pwm output that could be read by a (V)ESC.
Conclusion: all units I tried suck bigtime. The joysticks basically act as on/of switches, there is no way you can gradually accelerate or gently brake.
They are now at the bottom of my junk drawer.
```

---
## \#7 Posted by: Maxid Posted at: 2016-06-07T15:13:17.196Z Reads: 157

```
did you try nunchucks as well? Can you post a link to your code - I want to try it with a nunchuck and could need a sample of how to do the digital to PWM conversion.
```

---
## \#8 Posted by: Hillso Posted at: 2016-06-07T15:17:33.088Z Reads: 153

```
The stick does not move a potentiometer? wow that's disappointing. Thanks though.
```

---
## \#9 Posted by: trbt555 Posted at: 2016-06-07T15:19:02.471Z Reads: 150

```
They do, but the ouput range was just abysmal.
```

---
## \#10 Posted by: trbt555 Posted at: 2016-06-07T15:21:03.737Z Reads: 142

```
What you descibe is basically the Wiiceiver. As far as I know that code is open source and available to all.
```

---
## \#11 Posted by: Maxid Posted at: 2016-06-07T15:32:59.785Z Reads: 130

```
Yeah i just don't get why you need special hardware for that. Hook up an Arduino Mini Pro to the Receiver cables of a nunchuck then read the digital values and output a PWM servo signal. Could be done for 5$ with any nunchuck.
Maybe someone tried already and found a problem - but right now it actually sounds too simple to be true.
```

---
## \#12 Posted by: trbt555 Posted at: 2016-06-07T15:56:55.236Z Reads: 120

```
You are aware that the Wiiceiver is just an Arduino on breadboard, right ?
```

---
## \#13 Posted by: Maxid Posted at: 2016-06-07T16:01:55.548Z Reads: 122

```
The chip is the same yes (ATmega328P) - but I thought there is more to it. Why are people paying 40-50$ for this when they could just use a 2$ arduino?

Also what does "due to the lack of good wireless nunchucks available" mean on Austin David's site? Don't all nunchuks use the same I2C protocol? has anyone ever tried to see what the differences in the output signal are to a kama?
```

---
## \#14 Posted by: trbt555 Posted at: 2016-06-07T16:43:45.821Z Reads: 110

```
It's as simple as that. Look at his code, it's not complicated if you're familiar with Arduino coding.

Though the protocol is the same, there are differences in handshaking/encryption. The Nyko Kama nunchuck is slowly going extinct and there arent any good alternatives.
```

---
## \#15 Posted by: Maxid Posted at: 2016-06-07T16:47:46.499Z Reads: 106

```
[quote="trbt555, post:14, topic:4391, full:true"]
Though the protocol is the same, there are differences in handshaking/encryption.
[/quote]
How can there be differences? That would mean the wii handset is capable of negotiating with different protocols or encryptions or whatever - can that really be? People a lot more intelligent than me have probably tried this already and apparently failed for a reason but I can not find any information on this. When the wii handset is capable of connecting to different nunchuks we should be too...
```

---
## \#16 Posted by: trbt555 Posted at: 2016-06-07T17:47:55.571Z Reads: 92

```
There are actually posts about this on ES.
Sorry but I'm too wasted to search just now.
```

---
## \#17 Posted by: trbt555 Posted at: 2016-06-08T10:26:14.868Z Reads: 82

```
Ok so I'm sobered up now, I found the post I was referencing:

http://vedder.se/forums/viewtopic.php?f=14&t=26
```

---
## \#18 Posted by: Maxid Posted at: 2016-06-08T10:39:08.151Z Reads: 82

```
Thanks - but it just seems like one line of code could fix this. But there is no feedback since February. This could have been solved long ago but seems to not be in focus anymore for whatever reason.
```

---
## \#19 Posted by: Hillso Posted at: 2016-06-08T10:44:49.498Z Reads: 82

```
output range means bluetooth connectivity range, or ppm range (or something like that). thanks.
```

---
## \#20 Posted by: Dutch Posted at: 2016-06-17T01:30:07.006Z Reads: 67

```
After i saw the 3 part tutorial of GreatScott on youtube how to make a e-board,

I was actually searching to see if it was possible to use one of those bluetooth remotes and stumbled across this topic.
I wanted to build my own eletric board and was coming up with idea's. I liked the idea of using a nunchuck of a wii.
But i don't really like those. Don't really fit my hands well. I mean, i don't have big hands or anything but i really hate small controllers or anything like that. I rather have it a little bit bigger. I was looking at this one [Bluetooth Mouse Joystick Controller](http://www.aliexpress.com/item/VR-BOX-Bluetooth-Gamepad-Mini-wireless-Mouse-Joystick-For-Samsung-S5-IOS-Ebook-3D-Games-Bluetooth/32659316532.html?spm=2114.30010308.3.82.AM02i2&ws_ab_test=searchweb201556_0,searchweb201602_4_10017_507_10040,searchweb201603_3&btsid=a0918f81-21e3-4c4e-bcf4-6162b5aa62a5)

Also i wanted something else then the nunchuck because i wanted some more buttons. Mainly because i wanted to add a head/tail light on it for when i'm cruising when it's dark. Being able to control them from the remote is nice and convenient. Was also thinking of adding in turning signals of some kind. Don't ask me why, just because.

Also i'm from the netherlands so we have weird laws and the boards are technically banned because they are unsafe or something? So yeah, would be nice to tweak it a bit to make it. "safer".
```

---

# Wii nunchuck doesn&rsquo;t work as planned \[SOLVED\] thanks for help

### Replies: 19 Views: 1670

## \#1 Posted by: Benja_man Posted at: 2017-03-19T19:50:55.477Z Reads: 128

```
Hello there esk8 builders! :) I decided to do an electric longboard as a project for a school grade. I wanted to do my control system by myself, but I've ran in to some problems. I went with a cheap setup. I have bought these parts:
-Motor:[turnigy-aerodrive-sk3-6374-192kv](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)
-ESC:[hobbyking YEP 120A](https://hobbyking.com/en_us/hobbyking-yep-120a-lv-2-6s-brushless-speed-controller-with-selectable-sbec.html) (my plan is to control it with arduino and wireless nunchuk)
-Battery (2):[ZIPPY Flightmax 5800mAh 3S 30C ] (https://hobbyking.com/en_us/zippy-flightmax-5800mah-3s1p-30c.html) (I realized later after some research that I should have used a higher voltage, but it will work)
-wireless Wii nunchuck:[Nintendo Wii Playfect Rechargeable Wirel...](http://www.ebay.com/itm/331847694924?ssPageName=STRK:MESINDXX:IT&_trksid=p3984.m1436.l2649)
-programming card [i don' have it yet but that's the one](https://hobbyking.com/en_us/hobbyking-yep-esc-programming-card.html) (this will help me setup brakes and everything)

I have some background knowledge about programming (arduino and C) (not much tho) (I study electro highschool engineering..)
I started doing prototype control with an original wii nunchuck, and a servo motor (as throttle) and it worked!  But whenever I plug the wireless nunchuk, the module and nunchuck bind, but there isn't any data going through. Only the indicator light on the module blinks when I press one of the buttons on the nunchuck.

Can anyone help me? Does anybody know where to direct me?  Maybe I need to change the Baudrate? If anyone has any comments on my setup feel free to help :) im still new to this.
Sorry for English mistakes there must be a ton.. I live in Europe by the way.
```

---
## \#2 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-19T20:07:09.873Z Reads: 118

```
[quote="Benja_man, post:1, topic:19305"]
But whenever I plug the wireless nunchuk, **the module** and nunchuck bind,
[/quote]

What module?

I have wiiciever I'm not using, I'd offer it to you but your whole project is about you doing this reciever by yourself?
```

---
## \#3 Posted by: rpn314 Posted at: 2017-03-19T20:24:12.382Z Reads: 114

```
What are you plugging the nunchuck receiver into? Maybe more specifically, what device would you be changing the baud rate on? I'm pretty familiar with the setup on the vesc, but it doesn't look like that's what you're using....
```

---
## \#4 Posted by: Benja_man Posted at: 2017-03-19T21:01:40.381Z Reads: 100

```
thank you for your offer :) i live in europe so i guess the shipping would be on me ;). But the point is that I resove problems by myself or with your help (thank god i found this website).

I plug the nunchuck reciever tho the I2C pins on the arduino (in my case analog 4 and 5 pins, 5V, and gnd). I use an old wii nunchuck library that works.
```

---
## \#5 Posted by: Benja_man Posted at: 2017-03-19T21:04:26.000Z Reads: 97

```
Correct, this is not a vesc setup, but I plan on programing the [ESC](https://hobbyking.com/en_us/hobbyking-yep-120a-lv-2-6s-brushless-speed-controller-with-selectable-sbec.html) with a prog. card and arduino (hopefully I will get the brake going).
```

---
## \#6 Posted by: rpn314 Posted at: 2017-03-19T21:08:20.489Z Reads: 93

```
Got it. Just trying to get the whole visual. Sounds like you're going to use the Arduino to turn the nunchuck's signal into a pwm signal for the speed controller. Good for you!

My gut says try the baud at 9600. Can you link the Arduino library you're using?
```

---
## \#7 Posted by: Benja_man Posted at: 2017-03-19T21:13:20.685Z Reads: 85

```
Sure! It's [this one](https://github.com/coopermaa/Wiichuck)
```

---
## \#8 Posted by: Benja_man Posted at: 2017-03-19T21:36:43.839Z Reads: 83

```
Just to make things clear, wii nunchuck works on an actual wii, it just doesn't work on my prototype setup yet..
```

---
## \#9 Posted by: lowGuido Posted at: 2017-03-19T21:45:38.929Z Reads: 85

```
As far as im aware only the nyko kama or memorex brand wireless nunchucks work. It was something to do with the code i think.. someone on here found it once but i didnt hear much back from them.
```

---
## \#10 Posted by: Benja_man Posted at: 2017-03-19T21:52:02.523Z Reads: 84

```
[quote="lowGuido, post:9, topic:19305"]
nyko kama or memorex brand wireless nunchucks work
[/quote]

do you mean work on wiiciever? 

I found this post, really usefull for me haha [wiiceiver controller](http://www.electric-skateboard.builders/t/wiiceiver-controller/3057/34)
```

---
## \#11 Posted by: lowGuido Posted at: 2017-03-19T21:55:40.112Z Reads: 81

```
Ah yeah that was the thread i was thinking of. And he references that nunchuck you got.
Hmm i dont know then.
```

---
## \#12 Posted by: UniqueSnowflakeN27 Posted at: 2017-03-19T21:56:10.792Z Reads: 80

```
I live in Europe too, so it shouldn't be too expensive.
```

---
## \#13 Posted by: Benja_man Posted at: 2017-03-19T21:57:32.945Z Reads: 73

```
All I need is the code he wrote, I'm going to write him a message soon.
```

---
## \#14 Posted by: rpn314 Posted at: 2017-03-19T22:00:40.926Z Reads: 72

```
What are you using to connect the receiver to the Arduino? Something like the board referenced in this post?
https://todbot.com/blog/2008/02/18/wiichuck-wii-nunchuck-adapter-available/#more-224
```

---
## \#15 Posted by: Benja_man Posted at: 2017-03-19T22:01:01.826Z Reads: 72

```
Really? That would be awsome! Always good to have a backup if anything goes wrong. Like I said this project is still all about me making the thing because I'm being graded a month later, I have to report what I've done..
```

---
## \#16 Posted by: Benja_man Posted at: 2017-03-19T22:18:56.624Z Reads: 75

```
Yes I saw that post, I am using a cheap little adapter from [ebay](http://www.ebay.com/itm/I2C-Wii-WiiChuck-Nunchuck-Adapter-shield-Module-Board-for-Arduino-/400522866870?hash=item5d4105f0b6:g:4YYAAOSw9a5XPtQ1). However the code provided there doesn't work, or I don't understand it or how to use it..
```

---
## \#17 Posted by: landonkun Posted at: 2017-03-20T05:57:29.339Z Reads: 70

```
I know this is different than the way you're trying to go about it, but this is a video I saw before about using a regular Wii remote:

https://www.youtube.com/watch?v=MZfOWmmXbdc
```

---
## \#18 Posted by: Benja_man Posted at: 2017-03-26T14:17:36.303Z Reads: 63

```
Found the original Austin David code, I seems to work fine, (I havent motor tested it yet, but the motor works) I love to code, and I will most likely use it all the time. I have a little problem though, my nunchuck isn't calibrated (the neutral joystick position is not zero,  serial monitor says 0.1667). If I plug the classic wired nunchuck, the neutral position is 0.1200. so I guess It's fine?
```

---
## \#19 Posted by: Benja_man Posted at: 2017-04-01T15:54:07.922Z Reads: 53

```
Everything is fine now, figured the calibration. The board is runnig and I absolutely love it.
```

---

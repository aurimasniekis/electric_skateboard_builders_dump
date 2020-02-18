# Accessible DIY Remote: No 3D Printing, all parts available through Amazon.. and will leave you with minty-fresh breath:)

### Replies: 8 Views: 1640

## \#1 Posted by: tomiboi Posted at: 2019-03-09T04:52:59.490Z Reads: 205

```
![remoteproject|666x500](upload://rt9njD6GsZMQ3FGaXlrE07bhl9T.jpeg) 

Hi! I think that every DIY esk8er should be able to make their very own remote. So I have started to work on a project with the hope of making that possible... but I'm going to need a little help to move things along. 

For accessibilities sake I took my 3D printer and threw it out the window (just kidding, I don't own a 3D printer), I found a way around printed circuit boards, and also, all of the parts can be found on Amazon or through Adafruit.com. Lastly, it's adorable:)

The only thing that some folks might find intimidating is learning about Arduino, but don't worry. Arduino is designed so that we can all copy the work of smarter people and look brilliant, ourselves. It's easy. Don't let it intimidate you. This is a great project to get your chops up so that you can employ this technology elsewhere on your esk8.

Many Arduino projects use mint-tin style containers as project boxes and, quite honestly, they seem like they could make a good remote enclosure as well. They are functional, discrete and available at every corner store (they are also available empty, in-bulk and in all shapes and sizes at Amazon). Conveniently, Adafruit Industries also sells proto-boards shaped just like common mint-tins. They're kind of cute, make wiring easier and mitigate the need for PCBs. Although, you could make custom PCBs for yours, of course... or an enclosure made from legos for that matter:) 

Many of the remote projects that I looked at involved 3D printed thumbwheels. For this project prefabricated thumb-sticks seemed like the best fit. The large thumbstick pictured above is a very common Arduino sensor with a lot of documentation. It would work well for a larger remote, is easy to wire and would be a good choice for those of you with large, meaty hands :) The small thumbstick is from the Nintendo Switch. These replacement thumb-sticks can be found everywhere and would make for a nice mini-remote.

The Arduino board that I have chosen is the Adafruit Feather M0. There are a lot of reasons for this. For one, it is a great board and Adafruit makes cool toys. But also, @StephanMe has done a lot of ground work with this board based on @solidgeek's Firefly remote. So why reinvent the wheel. Additonally, though I'm leaving out the OLED is the basic project, you could get spicey and throw one in. The code is already there.

To get this project done before someone actually invents a hoverboard, I'll need some help. First, the sketch code for the Arduino board needs to be adapted for a thumb joystick instead of a hall-sensored thumbwheel. Second, I haven't a clue how to interface the small thumbstick with the Arduino. What on Earth is that little ribbon connector called?

Well, that's that. I'll report back with any progress. Any help from the community would be appreciated. Oh... by the way, the dorky antenna in in the picture is kind of a joke... kind of:)
```

---
## \#2 Posted by: skatardude10 Posted at: 2019-03-09T05:02:05.079Z Reads: 186

```
As much as I appreciate your initiative to design a non-3d printed remote... I suspect it's going to be similar to the arguments people have as to why you should just buy a spot welder if you intend to make more than one battery.

Secondly, a spot welder is great for batteries, but a 3d printer is great for so much more beyond what you would think you will end up using it for. I'd advocate for just diving into purchasing one of the good $200 3D printers, and end up with infinitely more flexibility with whatever you end up using it for.

Finally, regardless of what I advocate, this is cool AF. I don't have any Arduino experience, but I'll be following this thread for sure.
```

---
## \#3 Posted by: Virol Posted at: 2019-03-09T07:18:33.899Z Reads: 161

```
This looks interesting, I'll be keeping an eye
```

---
## \#4 Posted by: tomiboi Posted at: 2019-03-09T14:54:39.241Z Reads: 128

```
@skatardude10
It's all about accessibility and a good learning project :) I'll release a super high-end remote project later in the spring using the Feather M0, an aviation-grade thumb-wheel and a CNC milled enclosure. It will all be based on the same premises. You could certainly make a 3D printed mint-tin if you'd like :) I bet it would turn out really cool.
```

---
## \#5 Posted by: tomiboi Posted at: 2019-03-09T14:58:53.402Z Reads: 120

```
@Virol Thank you. I'll try not to disappoint :) If you know any codemeisters, direct them toward the thread.
```

---
## \#6 Posted by: tomiboi Posted at: 2019-03-09T15:27:52.092Z Reads: 112

```
Also, in my opinion 3D printing is for poodle-whippers and I'm standing firm on that opinion until I figure out which 3D printer I'd like to buy :)
```

---
## \#7 Posted by: Fissh02 Posted at: 2019-03-09T17:53:39.147Z Reads: 97

```
Wouldn't the metal ruin the signal?
```

---
## \#8 Posted by: tomiboi Posted at: 2019-03-09T20:28:50.630Z Reads: 84

```
@Fissh02 Solder a wire from the antenna pad to the mint-tin itself and the tin acts as an antenna. You could also install an external antenna like the dorky yet suave one pictured above. I would worry more shorting connections with the tin. I have some 1/16" adhesive-backed neoprene that I intend to insulate the inner front and back of the tin with to help prevent these problems. 
I hope to have the project ready for code within a week or two. Still need help with the code. Then it will be time for road-tests:)
```

---

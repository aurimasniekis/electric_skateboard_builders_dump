# An EE&rsquo;s ideas for improving the typical control system of ESK8

### Replies: 5 Views: 175

## \#1 Posted by: zbrown Posted at: 2019-07-05T17:47:35.194Z Reads: 83

```
Hey, 

I'm a student currently studying Electrical Engineering and I've done a lot of longboarding, skiing, and mountain biking in my life, but haven't actually ridden ESK8 much, I'm looking forward to building my first board.

The electrical engineer in me has been thinking about how we can make boards more intelligent in whats going on around them. There seems to be a big disconnect in how we control our boards, with a remote being the most prominent option (and really only option). I like the way the guys at Z Boards have integrated load cells into their boards to use shifting your weight as a control method, but it seems hard to learn and frankly dangerous on its own. 

So, here are my ideas.

 First off, load cells in between the trucks of the board and the deck. With a proper microcontroller (I've been thinking about prototyping with the teensy becuase of it's CAN bus support), you can effectively use this to arm and disarm your board when you're standing on it. You could also put a long strain gauge on the top of the deck and sense flex if you wanted to, although I don't know what purpose that would serve. 

My second idea is differential steering assist. Basically in a two motor board, you would use the aforementioned load cells and maybe also an IMU to measure the way the board is leaning and have a microcontroller give one side of the board more or less power. This could be a big deal because not only would it increase your turning radius, it would also allow you to theoretically drive your board around like an R/C car (I just thought that was fun lol).

Third, LoRa remotes. LoRa, while a pretty new wireless protocol, has proven to be very powerful and good enough for realtime applications. The current RF/Zigbee/Bluetooth solutions are good, but the range, customizability, and relatively low power of LoRa all seem to make it well suited for this kind of application. Imaging bailing on a hill (something even us non-esk8 longboarders hate) and just being able to drive your longboard back up it....

Finally, better encoders. I know that the VESC and many other platforms support encoders for better performance but developing a system like that of the ODrive's where you can use it for more advanced closed loop control (trajectory planning etc) would be really cool. Plus you could also use it for better coasting performance and belt life estimation if you have one at the wheel and one at the motor.

Thats about it for my initial post, but I have some projects in the works. Right know I don't really have any money (student life) but KiCAD is free so I might work on a concept of a board that integrates all of these ideas into one almost plug and play platform.
```

---
## \#2 Posted by: BooYA Posted at: 2019-07-05T19:14:05.703Z Reads: 73

```
I think these ideas night be good options for more mainstream EVs, but for esk8 I personally like to move a lot on my board while riding.
Also the gradient of the road would affect the way the load is distributed between the trucks. So you'd need an IMU to sense the incline.
I do like the remote because it makes the control independent from the way you ride.
Maybe some pressure measurement plates in the shoes, to sense when you push your back / front foot to accelerate / brake
```

---
## \#3 Posted by: meesie Posted at: 2019-07-06T14:23:31.015Z Reads: 44

```
i always move my feet and change my stance depending on the way and speed that i ride. in all honesty i think pressurepad controlls are a really bad idea for esk8.
```

---
## \#4 Posted by: zbrown Posted at: 2019-07-06T16:21:11.812Z Reads: 26

```
The beauty of the load cells is that the bumps and grade of the road will affect the reading proportionally equally on both sides, so you can effectively just subtract them from eachother. It's the same principle that differential communication protocols rely on.
```

---
## \#5 Posted by: zbrown Posted at: 2019-07-06T16:24:54.345Z Reads: 23

```
I totally see this, which is why I'm thinking about a hybrid design. Everything is up to you and mostly just serves as data for the microcontroller. And actually, based on the way it is currently sensing, shifting your stance wouldn't throw off the computer that much in the real world. The beauty of the system is that it's differential, so your forward/backward weight wouldn't affect the way the system responds to control. It's just doing subtraction to determine how the board is tilted left or right, and my guess is your changes of stance don't tilt the board because then you'd be turning anyways.
```

---

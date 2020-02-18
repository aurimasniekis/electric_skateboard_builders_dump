# Third party VESC devices developpers playground

### Replies: 9 Views: 382

## \#1 Posted by: Pimousse Posted at: 2019-02-27T12:00:54.069Z Reads: 132

```
Hi everyone,

We are now a lot of crazy guys who created amazing stuffs communicating with VESC.
Everyone knows @rpasichnyk, @Ackmaniac, @twan or @emmaanuel  for their apps.
But also @solidgeek who built a [remote](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543?u=pimousse), @janpom who built also an [embedded display](https://www.electric-skateboard.builders/t/davega-battery-monitor-odometer-speedometer/71509?u=pimousse), and many other people.

I also designed some toys (such as the [SmartRing](https://www.youtube.com/watch?v=94tGvjmw-p8) I love to play with).

Recently, we had a huge update of VESC FW and lot's of things moved.
Unfortunately, VESC project is really bad documented, so each time, we have to dig into source code and reverse-engineer stuffs to check/repair compatibility with our products.

Due to this lack of documentation, I started to build some personal tools.
I realized that they would be even more useful if they were shared ! :slight_smile: 

So I put them here : https://drive.google.com/open?id=1cz4vvPLa9w7otzsrnxXuGm6yhv0MWV9E
(some need to be updated such as VT and FW compatibiliy)

Feel free to grab them and add more stuffs. :+1: 
Share them back to me,I'll update the folder.
This way, we keep a common place.

What do you dev friends think ?
```

---
## \#2 Posted by: janpom Posted at: 2019-02-27T12:29:28.563Z Reads: 114

```
Hi @Pimousse, thanks for sharing those resources! Useful stuff.

It would be really nice to have a well maintained open source VESC communication library. I personally would be happy to contribute. I imagine that each of us would have different requirements and the question is if we can find enough overlap such that we could collaboratively create something that each of us could benefit from.

For me, the requirement would be that it compiles from the Arduino IDE since that's what I mostly use. I would also need to be able to compile it such that its footprint is small when I use only a small part of available functionality. I currently don't have a use case for writing into the VESC. I only read from VESC.

For some (@rpasichnyk?), the GPL license would likely be a stopper. It would have to be something less restrictive (MIT, BSD, Apache). I guess that would imply we start from scratch since the existing resources I know of (@solidgeek's [`VescUart`](https://github.com/SolidGeek/VescUart), RollingGecko's  [`VescUartControl`](https://github.com/RollingGecko/VescUartControl)) are GPL.

To start, I guess it would be best if everyone could say (1) whether and how much they would be willing to contribute to the project and (2) what their expectations/requirements would be.
```

---
## \#3 Posted by: chocol4te Posted at: 2019-02-27T12:48:41.011Z Reads: 99

```
I've been working on one here: https://crates.io/crates/vesc-comm.

It's very basic right now, but adding more features really shouldn't be too hard. It is, however, written in Rust and the major drawback is that using it from a C/C++ project isn't simple, but it is definitely doable.
```

---
## \#4 Posted by: Pimousse Posted at: 2019-02-27T12:56:09.881Z Reads: 95

```
Yeah, you're right.
Having an official Arduino library that can be updated directly in the IDE would be very useful !
I think @solidgeek 's one is a real candidate as it embbeds examples, readme, and so on.
```

---
## \#5 Posted by: Pedrodemio Posted at: 2019-02-27T23:39:54.132Z Reads: 72

```
Great idea @Pimousse, as @janpom said a universal communication library would be awesome, I stopped updating the firmware since while ago since it may mean a few hours cross checking everything and a lot of headache to make it work
```

---
## \#6 Posted by: evoheyax Posted at: 2019-02-28T01:54:45.763Z Reads: 61

```
Ah I neee to learn rust lol. I took 2 c++ classes back in the early days of college, but I’ve never really found a good use for it. I usually end up using java or python these days (mostly python). Though I am studying machine learning, so... lol.

Love the work of putting these all together. I did drastically improve the original implementation for Bluetooth communication and it’s updated for the latest firmwares. Though I need to push the latest code, you can find it on my GitHub.

[Github](Http://www.github.com/lukebelz)
```

---
## \#7 Posted by: solidgeek Posted at: 2019-03-06T16:23:50.381Z Reads: 40

```
I do not see why the GPL (GNU) license is an issue? I guess you refer to the "Disclose source" part, however, this does not mean that one is forced to release his software open source, only that if he does, it has to be under the same license as the library. That is at least how I understand GPL.

I would love to expand the VescUart library, however, I am not sure what features are needed/wanted.
```

---
## \#8 Posted by: janpom Posted at: 2019-03-06T16:53:24.077Z Reads: 40

```
I don't think so. GPL is a viral license. If you use any GPL code in your project, you're obliged to make your code open source under GPL as well.

This wouldn't work for Metr.at, for example.
```

---
## \#9 Posted by: solidgeek Posted at: 2019-03-06T19:29:22.329Z Reads: 31

```
Yeah, you are right, I have misunderstood how GPL works :) Unfortunately, I cannot change the license of the library, as some files are borrowed directly from the VESC bldc firmware (GPL).
```

---

# Making an Arduino controlled skateboard - senior project

### Replies: 5 Views: 2383

## \#1 Posted by: Spencer Posted at: 2016-11-22T14:46:17.326Z Reads: 138

```
Hi all,

I'm very new to the electric skateboard community, and I've been doing a good amount of research. I am making an electric skateboard for a senior project for school, and I want to use an Arduino to control it from my phone. I'm aiming to keep this sort of cheap (but I don't think that's gonna happen) and I was hoping that I could find some advice on choosing parts, compatibility, and utilization.

Here are my parts so far:
Motor: diy-electric-skateboard-kits-parts/motor-6374-190kv-3150w/
VESC: diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/
Drive train: http://www.enertionboards.com/diy-electric-skateboard-kits/mono-drive-mechanical-kit
Arduino UNO
Battery: https://hobbyking.com/en_us/zippy-flightmax-8000mah-3s1p-30c-lipo-pack.html

My questions are:
-what am I missing?
-is there anything glaringly wrong with this configuration?
-is there anywhere I can go to find a tutorial on how to implement the Arduino and use my iPhone as a controller?

Thanks!
```

---
## \#2 Posted by: domw95 Posted at: 2016-11-22T15:06:27.645Z Reads: 129

```
Hey i am doing something not too dissimilar at the moment, although I am using another arduino instead of a phone as the controller as I felt that would be more suitable, although i did look at using my phone.

As far as I know the only option to communicate between the two is via bluetooth which is possible using an arduino bluetooth module and then either using an App like [this](https://itunes.apple.com/gb/app/lightblue-explorer-bluetooth/id557428110?mt=8) or by writing your own in Xcode.  Example insructables [here](http://www.instructables.com/id/Iphone-bluetooth-control-arduino/).

From what I have seen this is slightly easier to implement with Android but still not easy.

Personally I didnt fancy using a touchscreen to control the board as it seems a bit risky not having actual buttons in your hands
```

---
## \#3 Posted by: jamesw Posted at: 2016-11-22T15:08:50.452Z Reads: 119

```
you're getting at least 2 of them batteries right?

this guy controls his with android; https://youtu.be/bOMJYJlmIfc

and this is his website; http://currentcontrolsystems.com/

good luck and keep us updated with the progress
```

---
## \#4 Posted by: DougM Posted at: 2016-11-22T16:19:11.678Z Reads: 104

```
2 things you may want to consider - 

If you use your phone as a controller and you crash there's a good likelihood that you'll damage your phone.

You won't be able to shoot video of your elongboarding shenanigans.

I went down this path using android and MIT App Inventor and it worked pretty well but in the end I decided a dedicated controller was better.
```

---
## \#5 Posted by: Spencer Posted at: 2016-11-22T19:35:37.545Z Reads: 78

```
[quote="jamesw, post:3, topic:13466"]
you're getting at least 2 of them batteries right?
[/quote]


I was planning on getting two, yeah, but it would be ideal to find one battery for cheaper than the two.
```

---

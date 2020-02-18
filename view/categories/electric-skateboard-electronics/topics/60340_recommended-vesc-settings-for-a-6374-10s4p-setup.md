# Recommended VESC settings for a 6374 10s4p setup

### Replies: 15 Views: 828

## \#1 Posted by: bplatoff Posted at: 2018-06-28T18:18:56.564Z Reads: 153

```
Hello, I know that this topic has been discussed a lot before but I could not find anything for my specific situation. I have already blown my VESC once and would prefer not to do it again. My setup is a single 6374 motor, a 10s4p 25r pack with a diyelectricskateboards VESC. I also have an anti spark switch that is supposed to be able to handle 40a. What settings would you recommend for this setup so that I have performance but do not risk my VESC again. Thanks for the help.
```

---
## \#2 Posted by: Benjamin899 Posted at: 2018-06-28T18:47:57.696Z Reads: 147

```
Ok that is the TB Vesc right? As far as i understand they can handle 28A continuous, since they have no direct FET cooling. Other than that, don't go over 60k erpm.
```

---
## \#3 Posted by: bplatoff Posted at: 2018-06-28T19:15:26.471Z Reads: 143

```
it is the torque boards one, I had heard that they couldn't handle very much so I didn't want to push to much, but I had the amperage low and could barely move, so I don't know what setting I should use because I don't think it would be pulling above 28 for an extended period of time.
```

---
## \#4 Posted by: Hannes Posted at: 2018-06-28T19:19:29.944Z Reads: 140

```
So their information on their site is incorrect?

"Current: Up to 240A for a few seconds or 50A continuous"
collections/featured-items/products/torque-esc-bldc-electronic-speed-controller
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-06-28T19:29:39.519Z Reads: 129

```
https://www.electric-skateboard.builders/t/new-vesc-user-read-this-complete-walktrough-of-the-vesc/2980
```

---
## \#6 Posted by: mixedcreation Posted at: 2018-06-28T20:15:20.690Z Reads: 119

```
Myself along with others run TB VESC above 28a.  I do understand, as I have read Evo's thread from 2016, but I know I am not the only person running higher than 28amps.

The only thing I stay away from is FOC on their VESC.  @torqueboards can shine some light on this subject.
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-06-28T20:24:28.888Z Reads: 112

```
i guess it is no problem since most don't run continuous 28amps, so the vesc can handle it but if you ride up a longer incline and you are heavier, you could cook it.
```

---
## \#8 Posted by: bplatoff Posted at: 2018-06-28T20:41:44.215Z Reads: 110

```
I’m definitely not gunning foc but for now I’m going to stick with 50a and hope it doesn’t blow I’ll post my setting later just to make sure nothing is too wrong
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-06-28T20:46:59.206Z Reads: 106

```
lol i’ve run more than 50a through my TB vesc got uphill runs. you just risk thermal throttling which isn’t really a big deal
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-06-28T20:53:14.147Z Reads: 102

```
yeah but do you want to risk it? i dont want to be the dude who said you can crank it up ^^ and later it is a pile of garbage
```

---
## \#11 Posted by: GrecoMan Posted at: 2018-06-28T20:58:15.451Z Reads: 97

```
risk what? thermal throttling? that just means the vesc will slightly tone down the performance until it cools down...
```

---
## \#12 Posted by: bplatoff Posted at: 2018-06-28T21:12:09.374Z Reads: 92

```
I also have heat sinks that I’m going to use on mine so hopefully that helps, they have some adhesive on them so I’m hoping that is thermally conductive
```

---
## \#13 Posted by: Benjamin899 Posted at: 2018-06-28T21:16:20.260Z Reads: 92

```
i am no expert, but i guess constant thermal throttling isnt good for electronics. i like to use my stuff conservatively
```

---
## \#14 Posted by: GrecoMan Posted at: 2018-06-28T21:59:48.371Z Reads: 88

```
lol constant thermal throttling does literally nothing long term to electronics
```

---
## \#15 Posted by: Benjamin899 Posted at: 2018-06-28T22:03:16.226Z Reads: 85

```
@GrecoMan good to know thanks
```

---

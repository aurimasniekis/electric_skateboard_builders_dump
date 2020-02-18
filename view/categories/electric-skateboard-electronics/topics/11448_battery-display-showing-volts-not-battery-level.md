# Battery Display Showing Volts Not Battery Level

### Replies: 6 Views: 945

## \#1 Posted by: GeorgeKing Posted at: 2016-10-19T14:02:52.658Z Reads: 157

```
Please could someone provide some assistance.

The battery level on my board is showing volts instead of the actual battery level. It seems to have affected the actual board itself as the brake no longer works and when you push off the motor stutters. I have checked the VESC to make sure the pins haven't punctured into the cables, which they haven't, but I've added some insulation to them as well as some glue just to make sure.

Not sure what to do here or how or why the braking has been affected so badly so any help would be appreciated.

I have the board open and everything seems to be working at first glance. 

Up until now, everything has worked flawlessly, the day before I went on a massive 30km ride and not a single thing went wrong, even with the Winning remote which is both amazing and surprising.

I have included an image for reference.

<img src="/uploads/db1493/original/3X/4/2/4201da4302ca15738172be7619f082bfdc00af7c.jpg" width="281" height="500">
```

---
## \#2 Posted by: Maxid Posted at: 2016-10-19T14:14:59.994Z Reads: 149

```
The battery meter should be hooked up in parallel to the rest of your system - so this can't be the reason for your braking. 
Battery meter wise I would actually prefer to have the voltage shown instead of percentage - this way you have at least hard numbers you can rely on - the percentage is not as accurate.
To solve this you need to look at your other parts and VESC configuration.
```

---
## \#3 Posted by: treenutter Posted at: 2016-10-19T14:39:58.572Z Reads: 140

```
[quote="GeorgeKing, post:1, topic:11448"]
The battery level on my board is showing volts instead of the actual battery level.
[/quote]

@GeorgeKing This is how these battery meters work, unfortunately. It is only marginally useful, since the discharge curve of our batteries is not linear. You'll be at "full" charge i.e. 42V for a short time, then at 3.7 for a long time, and then it will drop quickly again. 

Someone needs to develop a smart battery indicator that accounts for capacity and average discharge, to even out the curve and provide useful information (like a mobile phone's battery meter).
```

---
## \#4 Posted by: GeorgeKing Posted at: 2016-10-19T17:04:11.975Z Reads: 120

```
So at which voltage do I start to worry? Let's say, for example, that the battery level would read 10%, what would be the equivalent in voltage? Or is that not how these things work?

Also, that doesn't really explain why the board started stuttering and stalling and slamming on brakes. Any ideas on that?

My setup is pretty much a mono drive raptor but I have a Fulbag deck.

Enertion Space CELL Pro 4
Enertion drive train
Enertion 5374 motor
Enertion VESC
Winning Remote

<img src="/uploads/db1493/original/3X/7/2/7266cfab4302ace1c8b58ef4a9a50f3ba0fc77e8.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/8/3/838db6a78e735d0c330316fcd5de4f4c700a5d81.jpeg" width="281" height="500"><img src="/uploads/db1493/original/3X/2/d/2dedbd9f08ee42b61c03a69261baae62281a0081.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/8/8/88f13f2945a6da1c436240ffa4f5beb8d92b4067.jpeg" width="281" height="500"><img src="/uploads/db1493/original/3X/a/2/a2b4ffe7dd2e796fd439095d01ef027e552a1e19.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/c/c/ccacf753b3eb866f520d5db37b1f105bfa3d2207.jpeg" width="292" height="500"><img src="/uploads/db1493/original/3X/a/a/aa838cd6ae769888aeeeda98395dfcf5a15b83de.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/4/2/4201da4302ca15738172be7619f082bfdc00af7c.jpg" width="281" height="500"><img src="/uploads/db1493/original/3X/6/f/6fd1b5d37ed5667961cd5bc5b01cfe83cec1e0f3.jpg" width="690" height="388">
```

---
## \#5 Posted by: SageTX Posted at: 2016-10-19T17:37:53.242Z Reads: 100

```
Wrapped up and insulated like that, your VESC could be tripping a heat sensor maximum.

I know this was an attempt at a solution, but it can't be helping.
```

---
## \#6 Posted by: Blasto Posted at: 2016-10-19T18:36:36.024Z Reads: 94

```
There's a button at the back of the LCD, just press the button once while the board is on to switch from % to Volts, IMO prefer Volts

Isolate those motor leads, you will blow your DRV if they touch
```

---

# Decent setup for under $300?

### Replies: 8 Views: 1155

## \#1 Posted by: potatowarrior13 Posted at: 2017-04-24T01:19:41.454Z Reads: 113

```
So I have a custom built longboard that I want to convert to electric for <$300 and I think I have a relatively decent parts list, but since this is my first eSk8 I don't want to make a newbie mistake. The longboard has 70mm wheels and quite a bit of clearance underneath. It is not my first time dealing with RC electronics however so I know about battery C rating, capacity, motor kv, etc. 

So for the motor I am considering this one - http://www.ebay.com/itm/332121977591
Motor mount + pulleys and belt is here - http://www.ebay.com/itm/262844276187
ESC is this one - http://www.ebay.com/itm/262914773417
For the control I want to use an arduino nano connected to a Bluetooth module, and I made an android app so I can control the throttle by tilting my phone, I think this will be cool, but I'm not sure how practical haha
Then for power I want to use two 3s 10,000mah lipo batteries in series for a 6s voltage.

I have access to a 3d printer for making a custom enclosure underneath the board.
Does all this look OK, is there anything I am forgetting or missing on component selection?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-24T02:56:23.701Z Reads: 93

```
I hate to be the bringer of bad news but:
Your wheels have to be big enough to give ample ground clearance for the motor and pulley and belt.
80mm is pretty much the minimum that is used.
83mm and 90mm is more common.
400kv is much too high for an E-board.
245kv to 280kv for 6s voltage is more appropriate.
The motor mounts you listed are designed to be cheap but they're not designed to work well and will not keep your motor and wheel pulley alligned. And if you can get it to work at all, it will likely work loose and drop your motor on the ground while your riding.
The FVT ESC works but I've heard that it doesn't last long.
Your batteries need to be a minimum of 25C and 5000mah.
The multi rotor 10C high capacity batteries have been tried and it is reported that they are not so good for this application.
```

---
## \#3 Posted by: potatowarrior13 Posted at: 2017-04-24T03:30:45.285Z Reads: 83

```
Meh, I kindof figured as much, will look at redesigning my setup haha
```

---
## \#4 Posted by: wmj259 Posted at: 2017-04-24T03:38:47.360Z Reads: 78

```
Based on @Namasaki 's points: 
-If you spend $20 more for the motor you can get a decent KV one. Also in the groupbuy. 

-If you want a vesc I would recommend you participate in the group-buy that I started. The are about $65 and well built. 

-Don't go cheap on the motor mounts as it will wear down your pulleys and the belts much quicker.
```

---
## \#5 Posted by: Namasaki Posted at: 2017-04-24T03:44:14.821Z Reads: 73

```
[quote="wmj259, post:4, topic:21652"]
-If you want a vesc I would recommend you participate in the group-buy that I started. The are about $65 and well built.
[/quote]


That's a really good bargain.
@potatowarrior13 I would jump on this deal if I where you because if you don't get a vesc now, you will later and the money you spend on a car esc will just be money wasted.
```

---
## \#6 Posted by: potatowarrior13 Posted at: 2017-04-24T03:46:41.703Z Reads: 68

```
link for the vesc groupbuy? I can't seem to find it
```

---
## \#7 Posted by: wmj259 Posted at: 2017-04-24T04:07:15.627Z Reads: 63

```
It's made by the same company as the motors group buy.
```

---
## \#8 Posted by: wmj259 Posted at: 2017-04-24T04:08:38.832Z Reads: 64

```
I am unsure if the price is still the same:
https://www.electric-skateboard.builders/t/sk3s-big-size-motor-group-buy-3-6354-260kv-left/13540/230
That groupbuy closed but theres another one going on:

https://www.electric-skateboard.builders/t/sk3-small-dual-motor-groupbuy/16671/75
```

---

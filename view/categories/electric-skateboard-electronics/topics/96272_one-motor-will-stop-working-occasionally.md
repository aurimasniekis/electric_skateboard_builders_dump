# One motor will stop working occasionally

### Replies: 7 Views: 164

## \#1 Posted by: ualsteve94 Posted at: 2019-06-10T07:24:11.050Z Reads: 52

```
So I have a duel setup, Focbox’s, slave connected over can-bus.   Configured using BLDC TOOL, firmware 2.18.     One motor will stop working when the remote is not used.   Sometimes in a matter of seconds and sometimes it will take several minutes of not using the remote before it stops working.  It’s the Slave Focbox.  And the Focbox doesn’t actually shut off when this happens.  I made a video I’ll try and post right now.  Thanks.  Oh, and it worked fine for a whole day on one particular ride.   But then today it now keeps shutting off.   Any ideas?   

Here are pictures of the app config.


MASTER FOCBOX PICS 
![image|666x500](upload://v83ZHh5S5myuz8qCJnDgA32lLDd.jpeg) ![image|666x500](upload://3reIAX9yTlI6ptxg3MltLQ8SWSl.jpeg) 

SLAVE FOCBOX PICS 
![image|666x500](upload://6ueCm6jjPxpCDpbCg6tIb8gignu.jpeg) ![image|666x500](upload://t5QKwEwUZB8LaaB9LQQYE1shLFU.jpeg)
```

---
## \#2 Posted by: ricardo Posted at: 2019-06-10T08:04:22.170Z Reads: 30

```
Same thing happens to me, interested in this thread. Which remote are you using?

I'm using a Photon, btw.


Cheers,
Ricardo
```

---
## \#3 Posted by: ualsteve94 Posted at: 2019-06-10T08:13:45.904Z Reads: 29

```
Im using the nano V2
```

---
## \#4 Posted by: ualsteve94 Posted at: 2019-06-10T08:33:34.285Z Reads: 27

```
I think I got it!  You still there ?
```

---
## \#5 Posted by: ricardo Posted at: 2019-06-10T08:41:33.296Z Reads: 27

```
yeah! So how did you solve it?
```

---
## \#6 Posted by: ualsteve94 Posted at: 2019-06-10T08:50:50.809Z Reads: 27

```
So the Focboxes where confused as to which one is suppose to pickup the signal... I had both Focboxes controller ID set to 0,  and both set to “current no reverse with brakes”.. so they where both trying to pick up a signal. 

 So here’s what fixed it.   Make sure the master Focbox , the one plugged into your receiver, make sure that one , in the app configuration, general tab, the controller iD is 0
Then in the slave Focbox , make sure the controller id is 1
And then also in the slave settings, app configuration, ppm tab, hit disabled.  (if your remote is a ppm remote)   
Then write configuration and celebrate like I did 😁

This way only the master (the one named 0 ) is the only one trying to pick up a signal and then sending that info via can-bus to the slave. 

My motors work fine now.  THANK YOU TEDDY TOBOGGAN!
```

---
## \#7 Posted by: ualsteve94 Posted at: 2019-06-11T09:47:42.187Z Reads: 17

```
I was also told to UNcheck the box “send status over can” inside the master ESC.   Then inside the slave ESC select UART only. 

  I did both of these things as well as the other stuff previously mentioned and everything seems to be working perfect.
```

---

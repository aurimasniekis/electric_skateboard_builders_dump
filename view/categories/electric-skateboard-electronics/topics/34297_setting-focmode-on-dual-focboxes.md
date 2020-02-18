# Setting focmode on dual focboxes

### Replies: 7 Views: 730

## \#1 Posted by: Bloop Posted at: 2017-09-29T17:10:31.836Z Reads: 160

```
Hey i know this was discussed so many times and i.ve read so many posts about this.

Today i did the setup for my dual vesc over can. 

I did the motor detectinon for foc mode but only 1 motor spins.. so do i need to connect the slave vesc and do the motor detection on that one too ??? 

Thank you.
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2017-09-29T17:41:02.169Z Reads: 151

```
Yes you need to complete motor detection on both. Be cautious and double check everything. Do not connect or disconnect anything while any power is on/live. Even the USB connector. It's bad practice.

Good luck.
```

---
## \#3 Posted by: Bloop Posted at: 2017-09-29T18:06:22.325Z Reads: 143

```
Thank you for quick confirmation. i asked someone else and told me that i only need to do it from master .. but is working now that i did the setup on both 

I hope ill get it out on the streets tomorrow :D
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2017-09-29T19:58:27.416Z Reads: 131

```
I did have a second thought to what you first asked too. I'm using ackmaniacs firmware. I have never used the original vesc firmware. I don't know if they differ. On mine you can setup up the slave through can forwarding from the master. Maybe the person you asked had the same thought as me. What I am not sure about is doing motor detection through can forwarding. If anyone sees this and can Corcoran I would love an expert opinion. Anyway can fwd is right under the connect, disconnect and reboot buttons on the bldc tool. You check can fwd and choose #1 for the slave if that's how you have it numbered. I did the detections separately because I was setting up sensored foc and wanted no mistakes.

You did it the correct way. Congrats
```

---
## \#5 Posted by: karma Posted at: 2017-09-30T09:49:33.589Z Reads: 113

```
I just set up my dual focboxes with can and FOC last night. I set up each FOCBOX with it's own motor. Did motor detection separetly and then set up the CAN. I also used the ackmaniacs firmware.
How do you set up the slave through the master? I thought you had to change settings in both so that they match?
```

---
## \#6 Posted by: i2oadsweepei2 Posted at: 2017-09-30T11:29:13.965Z Reads: 105

```
You can change settings on the slave using "can fwd" on the master. So you would check the box in the pic below then choose #1 beside it. Your master should be set to #0 and the slave to #1. If you had four wheel drive they would be nice breed 0, 1, 2, 3. What I was curious about and never even thought to try was motor detection through "can fwd"

The reality is that I do set each vesc through its own USB port. This is just a cool feature. Many people have had a lot of problems with their vesc and some reported on the focbox too. I think the focbox/vesc-x are a solid choice. I've setup my two duals boards many different times in foc and now sensored foc. They really are set it and forget it as long as there aren't any heat issues or binding, arcing, other shorts, bad settings from rushing to get on the road etc... Just my opinion and not necessarily anyone else's.

<img src="/uploads/db1493/original/3X/2/a/2ae9537a67abfa31f39613e8471b0e54e810f5ee.jpg" width="666" height="500">
```

---
## \#7 Posted by: Bloop Posted at: 2017-09-30T13:59:21.332Z Reads: 90

```
In the end i did detection. on each vesc independent .

Tonight i will install ackmaniac fw and do all the settings once again . for that watt controll. :D And also i need to play with settimgs a bit.

Right now is not going too fast.. but it has lots of power when i start from still i almost get down. Wish i can get the top speed higher a bit.. i will have to measure the top speed tho
```

---

# When I turn off my remote, my motor goes full throttle. Anyone know what the cause it?

### Replies: 6 Views: 779

## \#1 Posted by: mgertner Posted at: 2017-12-14T03:03:18.162Z Reads: 118

```
So I will link a video of my problem,  when I turn off my remote while its still connected to the vesc/board, it goes close to full speed. Its not that big of a deal as I can just turn off my board first, but I am worried that ill be riding at like 5mph and then the remote will die and the board will go like 23mph and well, rip. So hopefully someone can help me out with this. Thanks.

Link to the video:
https://youtu.be/eGBoAygC9TY
```

---
## \#2 Posted by: mmaner Posted at: 2017-12-14T03:04:15.772Z Reads: 118

```
Search for 'fail safe'. There is literally a dozen threads about it.
```

---
## \#3 Posted by: mgertner Posted at: 2017-12-14T03:12:15.667Z Reads: 122

```
Do you know if there is a fail safe setting in the BLDC tool?
```

---
## \#4 Posted by: Namasaki Posted at: 2017-12-14T03:14:47.608Z Reads: 118

```
You need to re-bind you remote with the receiver.
Pull the jumper after the binding is complete and before turning off the board or remote.
Then test the remote throttle and brake, then turn the remote off with the board on to test fail safe.
Fail safe is set during the bind process, not in the bldc tool.
https://youtu.be/ywUfqtKF8Zg
Once you have successfully completed the bind process, you need to calibrate your Vesc and Remote in the bldc tool.
https://youtu.be/OtuofrQr3F8
```

---
## \#5 Posted by: mgertner Posted at: 2017-12-14T03:21:45.581Z Reads: 97

```
Ok I figured what I did wrong. I turned the board off before I pulled the jumper out. Thanks for your help!
```

---
## \#6 Posted by: Namasaki Posted at: 2017-12-14T03:30:36.311Z Reads: 94

```
Your welcome.
Also check out the second video on setting up your receiver in the bldc tool. Very important.
```

---

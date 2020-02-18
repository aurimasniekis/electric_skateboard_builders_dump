# Wheels spinning at different rates?

### Replies: 11 Views: 521

## \#1 Posted by: Dogman1247 Posted at: 2017-09-12T02:41:17.536Z Reads: 91

```
https://youtu.be/f9skZ4jTRSU

Here is a link to the video that should help show the issue,

I was also wondering if I went into bldc tool if that could help effect it at all?

I went into bldc and ran start detection, but it only ran for one wheel and I clicked apply, did I mess it up there? If so how do I run the other wheel on bldc?
```

---
## \#2 Posted by: Bloop Posted at: 2017-09-12T05:20:07.857Z Reads: 77

```
you need to run detection for each vesc individually.
```

---
## \#3 Posted by: Dogman1247 Posted at: 2017-09-12T07:08:21.107Z Reads: 71

```
but how do I do that? There is only one micro USB Port?
```

---
## \#4 Posted by: Bloop Posted at: 2017-09-12T07:41:58.308Z Reads: 66

```
each vesc has his own micro usb port. what do you mean by only one ?? can you describe more your setup ? vesc and connection to your motors?
```

---
## \#5 Posted by: Dogman1247 Posted at: 2017-09-12T07:50:52.130Z Reads: 59

```
there is only one micro usb port on the board, Its a kaly.nyc setup
```

---
## \#6 Posted by: TarzanHBK Posted at: 2017-09-12T08:01:23.119Z Reads: 52

```
Then it should be 2 Vescs connected over CAN bus, so you can connect to the usb port and choose CAN forward to ID 1:
<img src="/uploads/db1493/original/3X/0/f/0f987f3ecc31d4427465d4e1cc1080822911e709.jpg" width="525" height="262">
Then you are connected with your slave (second) Vesc and you can do all your settings there.
If you have further questions, i´m sure @Kaly will help you out ;)
```

---
## \#7 Posted by: Dogman1247 Posted at: 2017-09-12T22:34:41.656Z Reads: 36

```
this is so annoying, im about ready to burn this thing in a pit of gasoline...

so I got the second vesc on bldc BUT NOW MY REMOTE IS NOT WORKING.... any ideas? did I fuck something up in app confirguartion?
```

---
## \#8 Posted by: cwazy1 Posted at: 2017-09-12T22:42:36.488Z Reads: 32

```
guys, I would be careful telling him to mess with the can settings. The OP doesn't seem to know much about vesc configs. Worst thing that can happen to him right now is that he blows a drv because of a can setting.
```

---
## \#9 Posted by: Dogman1247 Posted at: 2017-09-12T22:43:34.695Z Reads: 32

```
how do I get my remote to work again?
```

---
## \#10 Posted by: cwazy1 Posted at: 2017-09-12T22:49:22.303Z Reads: 30

```
take screenshots of your BLDC config tabs.
```

---
## \#11 Posted by: Dogman1247 Posted at: 2017-09-12T22:50:22.023Z Reads: 29

```
got it fixed had it on the wrong app config and needed to reboot!
```

---

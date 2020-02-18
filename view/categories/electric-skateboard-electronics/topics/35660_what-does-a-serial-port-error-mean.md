# What does a &ldquo;serial port error&rdquo; mean?

### Replies: 8 Views: 406

## \#1 Posted by: evoheyax Posted at: 2017-10-16T14:38:03.836Z Reads: 80

```
chaka quad vesc v4.12

Was able to connect to it fine a week ago when I configured hummies new hubs with it. Now, I can't connect to any of the 4 vescs. One is missing the usb port (my fault) and the other 3 all give this error. It detects the firmware, connects, and immediately gives the serial port error and disconnects.

Any ideas what could cause this? The vescs all run fine other wise. Can't check for fault codes, since I just get an error when I try to connect. But I doubt I have any, since they are working normally otherwise.


This is using @Ackmaniac's 2.54 firmware. It's weird to me that I can connect to the 2.18 tool in limited mode without this error. 

@JTAG @chaka @Blasto
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-10-16T14:39:15.460Z Reads: 80

```
Are you using a Mac ?
```

---
## \#3 Posted by: evoheyax Posted at: 2017-10-16T14:43:24.949Z Reads: 74

```
yes 10 char
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-10-16T14:50:26.680Z Reads: 70

```
Yeah... I think it's how the tool as been compiled, I had the same issue so I switch back to the windows version, I haven't go any issue since.
```

---
## \#5 Posted by: evoheyax Posted at: 2017-10-16T15:07:34.228Z Reads: 66

```
It's weird though that it worked fine a week ago. I'll try the windows version and see I guess.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-10-16T15:34:58.323Z Reads: 63

```
Maybe a Mac update caused the issue. 
Do you have automatic updates?
```

---
## \#7 Posted by: evoheyax Posted at: 2017-10-16T15:36:04.142Z Reads: 63

```
ahhh... maybe. I don't have auto updates, but its been buggin me update for weeks, and I told it to f** off until the night, at which it can update, so it probably updated, lol.
```

---
## \#8 Posted by: evoheyax Posted at: 2017-10-16T16:19:19.164Z Reads: 47

```
So tried it on windows and all is good. Seems like the mac version no longer works...
```

---

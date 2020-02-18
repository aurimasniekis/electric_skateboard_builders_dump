# Setting up VESC

### Replies: 10 Views: 1251

## \#1 Posted by: Bensaida Posted at: 2017-07-21T21:58:57.760Z Reads: 107

```
I dont really understand how to correctly setup a VESC. Is there somewhere that shows exactly what settings to do, and really explains it?
```

---
## \#2 Posted by: mmaner Posted at: 2017-07-21T22:00:24.973Z Reads: 106

```
http://www.electric-skateboard.builders/t/vesc-faq-easy-vesc-configuration-in-windows-mac-for-noob/2963
http://www.electric-skateboard.builders/t/vesc-faq-easy-to-follow-vesc-getting-started-playlist/5560
```

---
## \#3 Posted by: lowGuido Posted at: 2017-07-21T22:22:47.054Z Reads: 97

```
you dont need to start new threads asking the same thing you can keep it all here.
```

---
## \#4 Posted by: Bensaida Posted at: 2017-07-21T22:26:18.857Z Reads: 88

```
Sorry. Ok ill condense it.
```

---
## \#5 Posted by: Bensaida Posted at: 2017-07-21T22:27:05.835Z Reads: 80

```
If the TB vesc is preconfigured for a 6355 motor is it okay fir a 6374 motor or do i have to change it?
```

---
## \#6 Posted by: darkkevind Posted at: 2017-07-21T22:27:29.474Z Reads: 75

```
You need to re-detect the motor...
```

---
## \#7 Posted by: Bensaida Posted at: 2017-07-21T22:28:06.792Z Reads: 72

```
Okay. And what if the battery has a 40 amp fuse, but the vesc is configured for a 80amp fuse? Will it detect/scan the battery as well?
```

---
## \#8 Posted by: darkkevind Posted at: 2017-07-21T22:29:24.075Z Reads: 71

```
[quote="Bensaida, post:7, topic:28226"]
but the vesc is configured for a 80amp fuse?
[/quote]

What is? . . . .
```

---
## \#9 Posted by: Bensaida Posted at: 2017-07-21T22:29:52.931Z Reads: 70

```
Edited the comment
```

---
## \#10 Posted by: darkkevind Posted at: 2017-07-21T22:33:07.514Z Reads: 69

```
You mean the max motor current?

That's for the VESC to automatically cut out if it tries to pull more than that amount of current. The battery will only go to 40A so there's no problem there, its the battery that will just get real hot, real fast running at max capacity.

What you don't want to do though is put too many amps to your motor, so if it's rated for 60A, don't put any more than 60 in that field...
```

---

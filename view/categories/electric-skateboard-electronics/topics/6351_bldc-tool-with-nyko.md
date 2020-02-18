# BLDC Tool with Nyko

### Replies: 5 Views: 709

## \#1 Posted by: arpitdave Posted at: 2016-07-19T22:18:29.513Z Reads: 52

```
Hello I got the Nyko Wirless  controller and soldered it to a JST and connected that to the VESC. I am struggling with having the motor activated with the remote. Currently my VESC is connected to the BLDC tool. The remote is on and light from both my remote and receiver are on. when i press C the light on the receiver starts flashing. So i know they are connected properly. However, when I press accelerate nothing happens. I have already read/write configurations for the Motor and App. Any help would be appreciated.
```

---
## \#2 Posted by: lowGuido Posted at: 2016-07-19T22:28:18.303Z Reads: 49

```
you will have to enable nunchuck and current control in the BLDC tool.
```

---
## \#3 Posted by: arpitdave Posted at: 2016-07-19T22:29:27.013Z Reads: 49

```
Yeah I did that already :confused:
```

---
## \#4 Posted by: arpitdave Posted at: 2016-07-19T22:30:45.087Z Reads: 44

```
So I go the remote connected. And it accelerates but the reverse function is not working. Any ideas about why? I have the bldc tool on current and reverse. Are there any other parameters I need to change to make it go in reverse?
```

---
## \#5 Posted by: Bender Posted at: 2016-07-19T22:37:12.512Z Reads: 39

```
tap the Z button once to go to reverse mode. you still push forward on the remote, back is always break for both forward and reverse mode.
```

---

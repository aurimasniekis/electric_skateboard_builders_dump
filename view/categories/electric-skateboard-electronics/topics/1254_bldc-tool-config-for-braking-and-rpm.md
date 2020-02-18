# BLDC tool config for braking and RPM

### Replies: 8 Views: 2460

## \#1 Posted by: Dedbny Posted at: 2016-02-07T10:19:49.792Z Reads: 170

```
Need some input on what I'm not doing right with the setting up of VESC through BLDC 1.10.
Running Dual R-spec 6355 motors 2x 4.7 VESC, Set up with HK-GTE transmitter and receiver.

Have the motors running, but the braking is not constant. At the moment its trigger down to accelerate and push trigger forward for braking. When using braking it wont hold the braking for much longer than about 5-10 sec(guess) not long anyway. Not long enough to come to a full stop I don't think at speed.  Need to push the trigger forward again to make it brake again.  Is there a setting I need to change on the BLDC tool to make the braking HOLD, so it keeps in braking mode.

I'm setting this board up for my son so need this to work to make it safer.

Also whats the best way to reduce the RPM or max speed, so we can get through a learning curve on the board. Son has never had an E-board before, and we are wanting to reduce top speed till he's use to it. 

At the moment its very easy to go very fast with the transmitter. Tried just reducing the RPM fig on the motor config connection menu on RHS, but that didn't seem to reduce the speed.

Thanking you all in advance. Found some good info on the site, but  now a little stumped. I'm sure its a simple setting thing. Hoping someone can help as I have a very eager kid who's very keen to get out on this board.

Screen shops of motor and app config.

<img src="/uploads/db1493/original/2X/6/6950098cc64548226fdf29b412423b74fadcedd4.jpg" width="335" height="500">

<img src="/uploads/db1493/original/2X/7/74e698e93c3bbc72d077737f179dfa813bab103b.jpg" width="335" height="500">
```

---
## \#2 Posted by: NIK Posted at: 2016-02-07T10:29:01.087Z Reads: 151

```
How you make the screenshot looks so tiny. Tbh, I doubt if anyone can see the details.
```

---
## \#3 Posted by: Dedbny Posted at: 2016-02-07T10:40:58.910Z Reads: 155

```
Appolagies. If you click the image and download it youll be able to read it better. Couldnt work out page set up in paint. Useless. Hope someone can help.
```

---
## \#5 Posted by: onloop Posted at: 2016-02-07T10:45:40.349Z Reads: 157

```
Check all the switches on the hand controller itself. There is a chance you have the throttle reversed due to the switch in the wrong place. This may also explain the braking issues. Check the trimming on the hand controller too.

To limit max speed you need to limit erpm.

Erpm is motor rpm x motor poles.
```

---
## \#6 Posted by: onloop Posted at: 2016-02-07T10:48:39.469Z Reads: 153

```
I wrote more about it here:

http://www.electric-skateboard.builders/t/stealth-hi5ber-zenith-caliber-2-single-r-spec-190kv-custom-carbon-enclosure-spacecell-vesc/249/53?u=onloop
```

---
## \#7 Posted by: Dedbny Posted at: 2016-02-07T10:52:36.172Z Reads: 145

```
Thks Jason, What would we do without you, Will have another look at the controller, and do some more research on the link.
```

---
## \#8 Posted by: Nasty Posted at: 2016-02-09T00:54:02.892Z Reads: 132

```
Click on "soft rpm limit" , and under "rpm limit end" enter value "60,000.00". Smooth and safe throttle my friend.
```

---
## \#9 Posted by: PDXroses Posted at: 2017-05-18T20:41:02.897Z Reads: 60

```
That's just what I needed to know. Thanks Nasty. Is this correct?

ERPM limit start = controls the acceleration from zero

ERPM limit stop = controls the top speed

What do you recommend if I want a safe acceleration from a standing position?  60K?
```

---

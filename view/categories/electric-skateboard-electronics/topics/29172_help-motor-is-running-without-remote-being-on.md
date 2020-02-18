# Help! Motor is running without remote being on

### Replies: 11 Views: 734

## \#1 Posted by: bluetree70 Posted at: 2017-07-31T01:17:07.402Z Reads: 108

```
Enertion Space Pro 3 Battery
Vescx
6374 190kv Sealed Motor
 FS-GT2B receiver and remote

I have ridden around 150-200 miles on this setup with no problems. Recently, I took apart all the connections to do some maintenance. This resulted in my setup having erratic behavior at times when I riding it. Nothing too dramatic when I'm accelerating or decelerating, but noticeable "jerky" motion that was never there before at random times. The setup simply does not respond as smoothly at some points in my ride. Today, as I put my board down, the motor started running all by itself! The remote wasn't even on! As I turned on my remote, it went back to normal, but I am at a loss as to why this is happening. My best guess is perhaps the connection between the receiver and the Vescx is damaged. Hopefully neither receiver nor Vescx is damaged. Any suggestions?
```

---
## \#2 Posted by: Sander Posted at: 2017-07-31T23:24:14.630Z Reads: 85

```
You could go in the PPM setting and enable the signal display to see how it acts and if it stays in the middle(the progress bar) when you have it in idle?
```

---
## \#3 Posted by: Eboosted Posted at: 2017-07-31T23:26:29.766Z Reads: 90

```
Your PPM settings are wrong and if you are using the Mini remote you need to turn the second wheel until it does not go forward when disconnected
```

---
## \#4 Posted by: DilatedPupils Posted at: 2017-07-31T23:54:57.131Z Reads: 88

```
You need to activate the fail safe on the remote
```

---
## \#5 Posted by: lrdesigns Posted at: 2017-08-01T06:15:49.285Z Reads: 85

```
GT2B has a weird bug where if you turn on the board but not the remote, after a couple minutes it will go full throttle. :rage: pretty dangerous.

But if you turn on the remote first, then the board. Then turn off the remote it will set the fail safe and you can leave the board on indefinitely with the remote off and nothing will happen. (Provided your fail safe is correctly set) Test if for your self and see.

Edit; Well at least mine has this bug I would like others to confirm?

As to the jerky-ness not sure could be many things.
```

---
## \#6 Posted by: krloz Posted at: 2017-08-01T07:26:01.755Z Reads: 72

```
Didn't ever have that issue with mine. Turned board and remote on and off in all possible orders plenty of times.  
Mine did come with the failsafe set to quite a big amount of breaking but I reset the fail safe to centre and no issues since
```

---
## \#7 Posted by: WARMAN Posted at: 2017-08-01T07:45:20.103Z Reads: 68

```
I don't remember setting a failsafe on mine and have no problems,I always turn my board on then the remote with no issues.
I did program my vesc's a long time ago though so not sure if a failsafe is set,why open it up when everything's been running smooth..if it ain't broke...
```

---
## \#8 Posted by: lrdesigns Posted at: 2018-08-27T08:57:39.082Z Reads: 38

```
[quote="lrdesigns, post:5, topic:29172"]
Edit; Well at least mine has this bug I would like others to confirm?
[/quote]

I finally found out why my board goes full throttle if you turn it on but do not turn on the remote. 

The receiver will automatically after a minute or so if it has had no signal from the remote go to a failsafe of 1500 ppm.  If when you set up the end points in BLDC tool and your mid point is not 1500 then you have trouble. 

This is in built to the receiver and seperate from the "fail safe" which is set with the remote and receiver.  

This only happens if the remote is never turned on. If you turn the remote on then the board, then remote off it gets your set fail safe. 

To fix the issue, go back into BLDC tool and make sure your mid point is at 1500 by adjusting the trim pots. You may even need to adjust the internal pots if you cant get it to 1500 with the externa trim pot. 

Then also re-set your regular fail safe with the button on the receiver. 

This way you have your fail safe from the remote at 1500, and the receivers remote never on fail safe is also 1500, and the midpoint in BLDC tool is 1500 then you should have no issues no matter the order you turn on your remote or board.
```

---
## \#9 Posted by: danielz Posted at: 2018-08-27T09:08:01.088Z Reads: 32

```
Yep, i documented this too a few months ago. The gt2b is weird, two different failsafes, one cant be changed.
```

---
## \#10 Posted by: Rotko Posted at: 2019-05-27T10:36:43.159Z Reads: 14

```
Hi, sorry to resurrect this old converstion but I couldn't find anything more helpful than this. 

In order to solve the a.m. problem
 I have to:

1) Set Pulselenght center @ 1500 in Ackmaniac vesc tool.
2) Adjust the middle Trim (Th. Trim) of the GT2B in order to get closer to 1500.

![immagine|375x500](upload://7zHavxZ0MMcF6txO1PCyA7FPOWY.jpeg) 

If necessary trim the internal pots, Which one? 1 or 2? (my assumption, these seem the only adjustable components on the pcb)

![3ae3e5438e387fc4dd54cf6f75bbbf7e291d0d8b|231x357](upload://oAnPXwWQvlvad9XT9wgnaGo7O8P.jpeg) 

thanks in advance for any help
```

---
## \#11 Posted by: captclearleft Posted at: 2019-05-27T13:13:26.942Z Reads: 9

```
Not sure that I will be of help here as I am not familiar with your remote, and I am not sure what hardware you are using.   You should first post more details...  What hardware are you using...?

Most RC tx/rx setups are similar... But each can be unique (you would need to look at your Transmitter(tx), Receiver(rx), and ESC documentation.  Here is what I mean.

Application 1:
When the transmitter(tx) and the Receiver(rx) are paired.  The center position of the transmitter motor channel is learned and stored.  

Application 2:
When the Receiver is turned on it waits for the transmitter to turn on.  It then waits to learn the Min/Max position for throttle (mostly rc airplanes).  

Application 3 (VESC):
With a VESC you must setup the VESC using the VESC software.  (Or whatever hardware VESC you are using).  This is where you might say: "duh, I know that"....  again, I don't know what hardware you are using...

So. Your trim pots...initially when the tx and rx are paired - They should be set to 0 to start (neutral).  

WARNING!!!! - - - Make Sure - - - 
SKATEBOARD IN A POSITION WHERE WHEELS CAN TURN FREELY AT FULL SPEED WITHOUT DOING ANY DAMAGE...

Turn on Remote.
Turn on Receiver.
Transmitter and Receiver should be paired.  If they are not paired, Pair them.

{{{NOTE: These are basic statements...  There are more steps to this. This is not a tutorial.  Following these steps could brick your system.}}}

Somehow your VESC should be connected to a computer, and you should be able to access it through some VESC software.  
In the APP, or remote settings you should see the PPM signal.  You should also have a "Setup Wizard" of some sort that walks you through your remote setup...

For most VESC's you can simply use the software to define center on the VESC.  Once the VESC knows where "YOUR" center is - Then you run through the wizard and define the min/max...  

If this incorrect, or someone has more input - Please correct me.   Thanks.
```

---

# VESC DRV8032 Problems new soldered

### Replies: 21 Views: 932

## \#1 Posted by: Blackmuffin Posted at: 2018-03-14T12:21:06.961Z Reads: 126

```
Hi guys, I buyed my VESC from Torque Boards and in the beginning it worked just fine (I just ran the motor dry without chain or something). Then I received my servo male to male cable and wanted to try out the motor with my RC Remote. Well, I don´t know how but the DRV8032 blew up. The motor didn´t spin at all and the error code said DRV8032. So I buyed a new DRV and let a friend solder it on to the VESC. Now the Motor is spinning when I´m using the arrow keys. But when I try to detect the motor it just stutter and says "detection failed". Same for when I´m using my RC Remote. But there are no error reports in the terminal at all. I hope someone can help me, because otherwise I have to buy another ESC. The biggest battery I connected was a 6s 2700mah and the motor I´m using is the APS 6384 130kv 4000w. I apreciate any help.
```

---
## \#2 Posted by: Ishayc Posted at: 2018-03-14T12:27:42.730Z Reads: 122

```
Can you upload a pic of the new soldered DRV?
```

---
## \#3 Posted by: banjaxxed Posted at: 2018-03-14T12:40:09.449Z Reads: 113

```
Is is essential to bridge 2 pair of pins per diagram on vedders schematic?
```

---
## \#4 Posted by: Ishayc Posted at: 2018-03-14T12:46:26.997Z Reads: 109

```
I'm not sure since I never went through the schematics but all vescs I saw had those 2 pins soldered together.

Edit: According to schematics it should be soldered together.
Look at 50,51 and 53,54 from Benjamin's schematic.

![Captu1re|448x500](upload://1vnpzmlo1ERI7JPJ0Cj82i4Cz2p.JPG)
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-03-14T12:50:53.012Z Reads: 96

```
yea they gotta be bridged
```

---
## \#6 Posted by: linsus Posted at: 2018-03-14T12:52:00.816Z Reads: 96

```
Did you use a hot air station when you soldered? Poor Connection to the gnd pad can do funny things. Also Visual inspection of each pin in a stereoscope does help alot. And then theres always the heat test where you Place the tip of your finger on the top of the componenets to see if anything runns abnormally hot. 

And yes, there are two pairs on one side of the DRV that are wired together. See schematic on vedders github if you want to know which ones.
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2018-03-14T12:52:52.970Z Reads: 96

```
[quote="Blackmuffin, post:1, topic:49082"]
The biggest battery I connected was a 6s 2700mah and the motor I´m using is the APS 6384 130kv 4000w.
[/quote]

Hi, 

Was the Battery fully Charge? and did you change the value of the battery voltage? Also, If you don't want to fry it again I highly suggest to not play with the Arrow is you didn't run a proper motor, it might easily blow your DRV again. 

PS. It will be easier for everyone to help you, if you add screenshots and picture

Regards
JF
```

---
## \#8 Posted by: Blackmuffin Posted at: 2018-03-14T13:14:01.221Z Reads: 93

```
![IMG_20180314_140736|375x500](upload://p9wGP3Nf5n0NvSqgZnA5kcZ4JlN.jpg) That´s the best picture I could get.
```

---
## \#9 Posted by: Blackmuffin Posted at: 2018-03-14T13:15:04.359Z Reads: 89

```
Yes he used a hot air station and checked the pins under a stereoscope. It seemed alright.
```

---
## \#10 Posted by: Blackmuffin Posted at: 2018-03-14T13:15:55.616Z Reads: 85

```
So you mean I have to bridge them directly on the chip? Or do you mean on the board? Because Vedder constructed the board, so I think the board already has the bridge connection in it.
```

---
## \#11 Posted by: linsus Posted at: 2018-03-14T13:27:30.412Z Reads: 83

```
they're connected on the board. but since heat is transfered easly thru the pins since they share the same pad they get cross soldered easly. So no, you dont need to bridge them with solder, but its not a big deal if they get bridged
```

---
## \#12 Posted by: Ishayc Posted at: 2018-03-14T13:49:21.301Z Reads: 80

```
Take a voltmeter and check if they are bridged to make sure.
If they are not there you go, otherwise, you got one less thing to check to spot the problem.
```

---
## \#13 Posted by: Blackmuffin Posted at: 2018-03-14T14:36:02.366Z Reads: 74

```
Thanks for the help. But now it blew up. I think i accidentally touched another component. So we won´t found out what the problem was.
```

---
## \#14 Posted by: linsus Posted at: 2018-03-14T15:32:48.861Z Reads: 70

```
Always probe stuff when Power is off, to make sure you dont short anything on your way there. 
What blew? the DRV? or circuitpaths?
```

---
## \#15 Posted by: Blackmuffin Posted at: 2018-03-14T16:06:38.940Z Reads: 65

```
Clearly the DRV. ![IMG_20180314_162744|282x500](upload://x3UEOCIspBMW8w0nN9usoUptQSP.jpg) But this time for real.
```

---
## \#16 Posted by: linsus Posted at: 2018-03-14T16:20:29.127Z Reads: 60

```
holy crap! it got nuked :joy:
Be careful when removing now so you dont rip DRV pads with you. See if there was any damage to the pcb and other Components, if not then you can try again!
```

---
## \#17 Posted by: b264 Posted at: 2018-03-14T16:27:05.491Z Reads: 60

```
Are you sure the DRV is blown?  Try checking the console for faults.  You wouldn't want to replace a good DRV chip

`/s`
```

---
## \#18 Posted by: banjaxxed Posted at: 2018-03-14T16:36:31.304Z Reads: 60

```
That will clean up ok with isopropol
```

---
## \#19 Posted by: Blackmuffin Posted at: 2018-03-14T17:09:41.385Z Reads: 58

```
Well I just cleaned it with isopropol and the DRV is clearly destroyed. So I´m gonna desolder it and see what´s left. I already bought a normal ESC from APS, so I can drive atleast. When I´m in the mood to try to repair the vesc I´m gonna go for it and buy another DRV chip. I still have the old one that doesn´t blew up but showed the DRV fault code whne built in. ![IMG_20180314_180842|282x500](upload://pZd1NCbDpnMBLOxyXS9qKKpfRhp.jpg)![IMG_20180314_181106|375x500](upload://2pWT3bOOngb7LszQc2VR7zIvBmC.jpg)
```

---
## \#20 Posted by: linsus Posted at: 2018-03-15T13:48:07.595Z Reads: 48

```
Think the cleanup was meant to be sarcastic :smiley:

Think there still are some that offer repair service if you dont want to put energy and time on it. Try look around abit :)
```

---
## \#21 Posted by: ThermalM16 Posted at: 2018-04-09T14:30:56.818Z Reads: 39

```
@Blackmuffin Hi, if you’re in North America, either @JohnnyMeduse or I can repair it
```

---

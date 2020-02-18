# \[solved\] I think :D - Unity problems&hellip;.. Please help

### Replies: 34 Views: 348

## \#1 Posted by: SynteX Posted at: 2019-04-03T19:27:43.952Z Reads: 117

```
I'm having insanly anoying problems with the Unity.

Please check out these 2 vids and I hope someone can help?
My trampa worked perfectly with 2 normal focboxes and I'm trying to replace them with a Unity.
But that just won't work?
Sensorless motors.

https://youtu.be/TiO-kDvFRgw

https://youtu.be/5-4x74GrHc8
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-04-03T19:31:03.688Z Reads: 112

```
@Deodand @CarlCollins those are the right people to ask. :smile:
```

---
## \#3 Posted by: Jinra Posted at: 2019-04-03T19:42:12.812Z Reads: 110

```
Did you program them and run through detection? or did you just try to plug and play? It'd be helpful if you included more information and what problems you're having and what you've tried doing.
```

---
## \#4 Posted by: pookybear Posted at: 2019-04-03T19:43:13.995Z Reads: 108

```
Did you use PC or app to configure this?
```

---
## \#5 Posted by: barajabali Posted at: 2019-04-03T19:44:04.075Z Reads: 103

```

Use the focbox tool program and up your Sensorless erpm to 5000 or so. That should solve your stuttering  problem @SynteX

Other things to check
Rerun detections
Rerun sensor detections
Make sure all bullets are plugged in
```

---
## \#6 Posted by: SynteX Posted at: 2019-04-03T19:46:07.945Z Reads: 95

```
This is my second esk8.
I do exactly know how to program them

I've connected a:
30q 12s5p And got the following settings:
80A bat max
Both motors 60A max

I'll do some things @barajabali just said.

Let me try that.
```

---
## \#7 Posted by: SynteX Posted at: 2019-04-03T19:51:57.729Z Reads: 91

```
![Screenshot_20190403-215114|243x500](upload://jdG4EP0OBGeVTOuiaN0jntKTc6l.jpeg) 

Didnt solve the issue
```

---
## \#8 Posted by: SynteX Posted at: 2019-04-03T19:53:16.169Z Reads: 84

```
![Screenshot_20190403-215249|243x500](upload://e3Q1Qfv9gBkpFikRJqxIcXleedf.jpeg)
```

---
## \#9 Posted by: barajabali Posted at: 2019-04-03T19:53:30.666Z Reads: 81

```
Did you do what I said about changing the sensorless erpm?
```

---
## \#10 Posted by: SynteX Posted at: 2019-04-03T19:57:18.736Z Reads: 79

```
Using the focbox tool?
```

---
## \#11 Posted by: barajabali Posted at: 2019-04-03T19:57:29.775Z Reads: 78

```
Yes 

10 char
```

---
## \#12 Posted by: Jinra Posted at: 2019-04-03T19:58:45.974Z Reads: 76

```
why would sensorless eRPM affect anything if he's running sensorless to begin with. Assuming he correctly set the mode to run sensorless...
```

---
## \#13 Posted by: SynteX Posted at: 2019-04-03T20:00:08.268Z Reads: 75

```
Like this?

![unity1|690x387](upload://xDpGCTGP9K3KPti9PwgSfQ18YMs.png)
```

---
## \#14 Posted by: Jinra Posted at: 2019-04-03T20:00:54.705Z Reads: 70

```
no that's `openloop erpm`. There's a section in "hall sensors" for "sensorless eRPM" but you shouldn't need to touch that if you set it to "sensorless" in the "general" tab.
```

---
## \#15 Posted by: SynteX Posted at: 2019-04-03T20:01:23.622Z Reads: 69

```
Hahah than i won't write these settings let me change that other setting :stuck_out_tongue:
```

---
## \#16 Posted by: Blasto Posted at: 2019-04-03T20:01:24.938Z Reads: 69

```
for the stuttering, go grab the focboxtool.exe

https://github.com/EnertionBoards/FOCBOX_UI/tree/FOCBOX_UI/windows_build


go to motor settings -> FOC -> sensorless tab

crank up the openloop erpm in increments of 100

![image|690x303](upload://iiCDQ0jrehFx5XnMes89d3PSOon.png)
```

---
## \#17 Posted by: SynteX Posted at: 2019-04-03T20:05:36.470Z Reads: 68

```
@barajabali 
Changed sensorless ERPM to 5000 under the hall sensor tab. Seemed to fix 1 motor?

https://youtu.be/q6dLH8N3IEk

Let me add a note:
My motors have 3 diffrent colored cables
Red, black and yellow

They are connected to the focbox like this:
Motor1: red black yellow, motor2: yellow black red.

This should be the problem since this is only the direction of the motor?
```

---
## \#18 Posted by: Jinra Posted at: 2019-04-03T20:13:17.723Z Reads: 60

```
Yea phase wire order only affects direction
```

---
## \#19 Posted by: SynteX Posted at: 2019-04-03T20:14:05.547Z Reads: 61

```
Wel the right motor seems to work now. But the left one still doesn't

Another note:

Checking the duty cycle in the focbox tool:
duty 1 is not changing on acceleration.
duty 2 is now
```

---
## \#20 Posted by: Jinra Posted at: 2019-04-03T20:16:19.724Z Reads: 59

```
Could you confirm your set it to senseless in the general tab? There's two "General > sensor port" and "FOC > General > sensorless"
```

---
## \#21 Posted by: SynteX Posted at: 2019-04-03T20:19:31.950Z Reads: 57

```
Sensor ports don't have an option for none " General &gt; sensor port"
I can however confirm is is set to sensorless at "Foc > General"


![unity3|571x500](upload://xldkg6YRb84O0OUwXRN4Q2wwSar.png)

Duty 2 keeps chaging from -0.1 to 0.0 and 0.1
Duty 1 is 0.0 all the time.
```

---
## \#22 Posted by: Jinra Posted at: 2019-04-03T20:22:07.879Z Reads: 53

```
Which one is the working one
```

---
## \#23 Posted by: SynteX Posted at: 2019-04-03T20:22:55.112Z Reads: 52

```
duty 2. Because that is the right motor i can see him increasing % when I accelerate.
```

---
## \#24 Posted by: barajabali Posted at: 2019-04-03T20:25:35.855Z Reads: 52

```
Increase it more, increments of 500.
```

---
## \#25 Posted by: Jinra Posted at: 2019-04-03T20:26:10.282Z Reads: 56

```
Did you detect lambda as well? I only ask because i see that's missing on your picture
```

---
## \#26 Posted by: SynteX Posted at: 2019-04-03T20:27:18.338Z Reads: 57

```
They rarely work together:
https://youtu.be/4csR36f26xc

After I did a brake they didn't work anymore.

So I need to increment the "Foc -> Hall sensor -> Sensorless ERPM with 500 until it works?"
```

---
## \#27 Posted by: barajabali Posted at: 2019-04-03T20:39:18.876Z Reads: 55

```
Lets get on a team viewer. I can likely fix whatever problem you are having. PM with your details
```

---
## \#28 Posted by: barajabali Posted at: 2019-04-03T20:40:02.593Z Reads: 51

```
Your motors dont have sensors, Right? If not the openloop erpm needs to be adjusted
```

---
## \#29 Posted by: SynteX Posted at: 2019-04-03T20:40:46.021Z Reads: 50

```
Nope they are indeed sensorless i'll pm you my teamviewer info right now.
```

---
## \#30 Posted by: barajabali Posted at: 2019-04-03T20:41:16.014Z Reads: 52

```
Okay I have experience getting sensorless motors working well with the Unity. Not as easy as with the Focbox
```

---
## \#31 Posted by: barajabali Posted at: 2019-04-03T20:50:37.919Z Reads: 52

```
Problem solved: Increase openloop ERPM, increase stator saturation. Took multiple trys to get Lambda to detect but it worked in the end.
```

---
## \#32 Posted by: SynteX Posted at: 2019-04-03T20:53:12.532Z Reads: 52

```
Thanks for the help man!!!

I'm going to do some test rides tomorrow :smiley:
```

---
## \#33 Posted by: barajabali Posted at: 2019-04-03T20:53:48.255Z Reads: 52

```
My pleasure
```

---
## \#34 Posted by: SynteX Posted at: 2019-04-04T19:38:13.385Z Reads: 29

```
Just had a little night ride. My board is working perfectly!!! Thanks again @barajabali .
```

---

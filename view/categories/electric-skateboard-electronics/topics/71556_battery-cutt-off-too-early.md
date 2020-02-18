# Battery Cutt Off too early

### Replies: 20 Views: 407

## \#1 Posted by: silvor11 Posted at: 2018-10-17T17:28:05.593Z Reads: 140

```
Hello fellow electric skateboarders,

I have encountered a issue and I hope someone can point me in the right direction. I use Vesc Tool 0.95 and have set my cutt off  start voltage at 34V and my cutt off end voltage at 31V. My BMS has the cutt off at 31V. When I ride my skateboard it shuts down when I have completed 20-25km. When I check the voltage level the voltage is still at 36.7V. I don't understand why it shuts down because I didn't reach my cutt off settings. Is it because of the lower voltage, more amps has to push trough too reach the same watts and therefore too much amps are pushing trough which shuts down any of my components?

-I use a flipsky vesc 4.12, Battery Max at 50.
-I have a 10s5p LG MF1 cells from diyeboard (I know, not the best battery please don't judge me ghehe)
-I use the flipsky anti-spark switch with on/off button
-Turnigy sk8 6364, 245kv unsensored

I hope someone is able to help me. Thanks in advance.
```

---
## \#2 Posted by: Battosaii Posted at: 2018-10-17T17:36:22.699Z Reads: 128

```
That's weird a 10s5p shouldn't have enough voltage sag to drop from 36.7 to 31v.  Maybe there is an issue with the battery. Do you have a Bluetooth module to datalog and see what's going on in the Vesc when it cuts power.
```

---
## \#3 Posted by: Benjamin899 Posted at: 2018-10-17T17:44:46.803Z Reads: 121

```
i disagree. The MF1 sags hard. 
@silvor11 Battery max 50A is 100% of the continous rating of the Battery. Meaning at 50% asking 100% of the possible pushes the battery fast down to the cutoff.
https://lygte-info.dk/review/batteries2012/LG%2018650%20MF1%202200mAh%20(Purple)%20UK.html
```

---
## \#4 Posted by: Sender Posted at: 2018-10-17T17:47:46.599Z Reads: 112

```
I think this is sag causing the cut out
```

---
## \#5 Posted by: silvor11 Posted at: 2018-10-17T18:40:29.611Z Reads: 101

```
Don't have a bluetooth module yet, so it's difficult too see what really happens. But a drop of 5 volt seems like a big drop. Things that I notice as well is that the breaks aren't working accordingly after 15/16km.  The braking power isn't as strong as a fully charged pack.
```

---
## \#6 Posted by: Benjamin899 Posted at: 2018-10-17T20:24:19.084Z Reads: 89

```
post all your settings from the vesc pls.
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-10-17T20:32:59.299Z Reads: 85

```
3v (34-31v) sag for a 10s pack means .3v sag per cell. very likely sag. 

start soft cutoff higher so vescs has a chance to limit current draw before bms does a hard cutout.
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-10-17T20:40:55.474Z Reads: 82

```
exactly what faceplanted me. the battery was already around 30% and i gave it full power, no chance for the for vesc to regulate it down.
```

---
## \#9 Posted by: silvor11 Posted at: 2018-10-17T20:42:46.467Z Reads: 84

```
![Vesc%20Settings|690x388](upload://sYH8eI1VDPnQiw3UuYTIFAjpJ57.jpeg) ![Vesc%20Settings%202|690x388](upload://mvw1twoVLdKN62P8vIrBzlmVJhI.jpeg)
```

---
## \#10 Posted by: silvor11 Posted at: 2018-10-17T20:48:56.320Z Reads: 78

```
So setting "voltage cutt off start" higher will draw less amps when reached, less amps will create less voltage sag so it won't reach the 31V cutt off immediately like before? Did I understand this correctly.
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-10-17T21:08:07.817Z Reads: 74

```
that is the idea, yes.

and then also get into the habit of not gunning it when pack % gets below like 40%, that helps too.

this is not an issue when bms is bypassed.
```

---
## \#12 Posted by: Benjamin899 Posted at: 2018-10-17T21:17:03.460Z Reads: 70

```
i would lower that battery max, down to 30A. Still enough and it doesnt kill your pack.
@thisguyhere is the hardcutoff of the bms the same as from the vesc?
```

---
## \#13 Posted by: silvor11 Posted at: 2018-10-17T21:17:12.728Z Reads: 67

```
Thanks. I will try new settings with cutt off start at 36V. The issue with the brakes is it related? Brakes aren't as strong at low volts vs fully charged (42V)
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-10-17T21:19:57.150Z Reads: 64

```
i wouldnt set the cutoff that high. 
you can set the Battery Regen to -12.
```

---
## \#15 Posted by: silvor11 Posted at: 2018-10-18T15:07:24.362Z Reads: 55

```
Thanks for all the ideas. I will try those new settings. Will report back if it's succesfull.
```

---
## \#16 Posted by: briman05 Posted at: 2018-10-18T16:14:22.783Z Reads: 52

```
The amps for that pack are 50A that isnt that much depending on the power your motors are putting out  not sure how much the MF1 cells are but you can get HG2 for 6.00 a cell and double your amps for your pack and have longer battery range Or the Samsung 25R for 3.50 a cell.  I would contact @psychotiller and replace the battery because he doesnt use crappy cells for his packs
```

---
## \#17 Posted by: silvor11 Posted at: 2018-10-18T17:39:54.663Z Reads: 52

```
[quote="briman05, post:16, topic:71556"]
the MF1 cells are but you can g
[/quote]

I totally agree with you those MF1 aren't the best cells but at the moment it's all I have and want the most out of it. So I'm happy that people are taking the time for answering my questions and have possibles solutions to make the best of a worst case (battery pack) scenario. In the future I will definetly take it into considerating to buy or create a better battery pack.
```

---
## \#18 Posted by: briman05 Posted at: 2018-10-18T18:43:54.110Z Reads: 48

```
No problem with trying to get the most out of what you got.  But do what they stated above and you should be good to go.  And when you are ready to upgrade your batteries I'm sure there will be a groupbuy for some 30Q or something @thisguyhere has done a few and you get some great batteries for pretty cheap because it is such a large quantity orders
```

---
## \#19 Posted by: thisguyhere Posted at: 2018-10-18T18:50:27.170Z Reads: 44

```
funny you mention it, i've got an ass load on the way on a boat from nkon.

details to follow, sometime in november.
```

---
## \#20 Posted by: humanisticnick Posted at: 2019-03-13T18:45:31.839Z Reads: 25

```
Were you able to find the battery settings that worked for you? I have the same DIYEboard pack and was considering hooking it up to a VESC.
```

---

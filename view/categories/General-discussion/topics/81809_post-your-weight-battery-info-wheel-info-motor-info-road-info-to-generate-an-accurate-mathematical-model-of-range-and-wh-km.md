# Post your weight, battery info, wheel info, motor info, road info to generate an accurate mathematical model of range and wh/km

### Replies: 9 Views: 369

## \#1 Posted by: mishrasubhransu Posted at: 2019-01-23T11:08:57.963Z Reads: 121

```
In my work I create mathematical models(using machine learning) for explaining complex vehicle dynamics given the control commands and velocity of the vehicle. I plan to employ some of those methods to generate an accurate model to predict the range of your vehicle. To do so, the more the data points the better. Please don't be afraid to post whatever information have. To start off please enter data in the format below, later I can create a webpage to get the data from you. The same webpage will include a calculator for people who want to get their prediction too. 

**Please let me know if you think of any other important variable or if you notice any mistake**

if you don't have a field, or don't feel like answering then just say "none". Also you don't have to include "#" or anything after that. It would be treated as a comment.
format:
++++
weight: 90 # rider+board in kg
cell_min: 3.2 # min cell voltage
cell_max: 4.1 # max cell voltage
cell_capacity: 2.5 # advertised cell capacity in Ah(not mAh)
cell_name: 25R # 30Q, HG2... Whatever name you know. Could be "none".
batt_size: 10S4P #cells in series and parallel
batt_capacity: 370 # in watt-hour.  calculated as nominal_voltage X cell_capacity X total number of cells
range: 20  # Full range you get based on your cell_min and cell_max
whperkm: 20 # watt-hour/km if you have already calculated it
wheel_width(mm): 50 # wheel width
wheel_dia(mm): 150  # wheel diameter
wheel_duro: none #shore hardness 
wheel_psi: 70 # pressure if pneumatic wheel else none
wheel_type: pneumatic # options are: pneumatic, thane
motor_can_dia: 63 # in mm
motor_can_len: 74 # in mm
motor_type: outrunner# options: hub or outrunner
motor_brand: flipsky # options: flipsky, maytech, hummie, enertion, ...
drive_type: belt15 #options: belt9, belt12, belt15, belt20, geared, direct
terrain_type: asphalt2 # options: asphalt0(best),..., asphalt5(like cobble stone), dirt
++++

**In addition if you have the metr pro log files that would be awesome.** 


As per the best of my knowledge, existing [calculators](http://esk8.today/2016/12/28/how-far-can-i-ride/#rc) don't take several important factors into account. Interface of such a calculator found in one of the threads show that. 
![image|281x500](upload://xm6gwRjaxjsRbOzcdeSi4Cp6qhm.jpeg)
```

---
## \#2 Posted by: Sebike Posted at: 2019-01-23T11:24:19.816Z Reads: 114

```
I believe almost this same exact data was collected for a (similar?) project about a year ago. 

You can probably find it using the search function and maybe he's willing to share the data with you?
```

---
## \#3 Posted by: mishrasubhransu Posted at: 2019-01-23T11:47:53.736Z Reads: 113

```
Oh thanks, I think I found it(unless you are talking about a different one). I won't be able to use the data there because it is missing out a lot of useful information(wheel type, wheel_size, cell_min, cell_max ....) and not very easy parsable. In that thread,  I also found a link to the [calculator]( http://esk8.today/2016/12/28/how-far-can-i-ride/#rc) but it doesn't seem to be online. Also that calculator doesn't take into account a lot of the influencing factors. 
![image|281x500](upload://pX3lwEXxIrLCxdJ1Y0lMofjdSXC.png) 

https://www.electric-skateboard.builders/t/whats-your-range-list-the-following-battery-size-wh-xsyp-lipo-li-ion-brand-drivetrain-hubs-belt-single-duo-quad-kv-ratio-vesc-y-n-regen-braking-y-n-average-payload-user-gear-bags-etc-range-miles-or-km-wh-km-or-wh-mile/14832/8
```

---
## \#4 Posted by: Bor.inc Posted at: 2019-01-23T11:58:54.352Z Reads: 91

```
I thought @bevilacqua also did a project about eakate stats but not sure
```

---
## \#5 Posted by: bevilacqua Posted at: 2019-01-23T12:31:11.550Z Reads: 79

```
Its still ongoing, plenty of data to use.But im skeptical about a Range Calculator, too many variables
```

---
## \#6 Posted by: mishrasubhransu Posted at: 2019-01-23T12:39:26.573Z Reads: 74

```
[quote="bevilacqua, post:5, topic:81809"]
Its still ongoing, plenty of data to use
[/quote]
Link?

[quote="bevilacqua, post:5, topic:81809"]
too many variables
[/quote]

Are you saying that I am asking for too many variables or are you saying that real world has too many variables to consider and we can't use all of them?

But anyway, that will be reflected in the accuracy of the model on the validation dataset. The idea is to get the best estimate we can, so that our build matches our expectation.
```

---
## \#7 Posted by: bevilacqua Posted at: 2019-01-23T13:04:30.821Z Reads: 62

```
Sorry, maybe I dind't use the right words, yes simplifying some of the parameters it would work. 

[quote="bevilacqua, post:1, topic:73454"]
Open Database Files: [Link](https://drive.google.com/drive/folders/1V5F6_CeHETD8KmOQ9URazU5k292Xgf0R?usp=sharing)
[/quote]

I'll update the list this evening. They are saved/converted to VDLA format. Distance in km (miles were converted) and timpestamp on the left side in unix format. Only numbers to facilitate csvread. Cell (1,17) is the vesc-count.
```

---
## \#8 Posted by: mishrasubhransu Posted at: 2019-01-23T13:13:18.112Z Reads: 60

```
Oh wow! This is precisely what I had in mind. The data collection part is nicely done. Even after your theseis is done, maybe you can keep it open so that addition data keeps coming in.
```

---
## \#9 Posted by: bevilacqua Posted at: 2019-01-23T13:15:58.035Z Reads: 58

```
of course, I didn't have time for any deep analysis of the data, but I'll post the finished work with some cool histograms and maybe a representative Esk8-Driving Cycle (similar to a FTP-75 or WLTP  DC)

The preprocessing step is completely automated (well, I have to open matlab manually, but thats it), the rest is done by the google apps script cloud
```

---

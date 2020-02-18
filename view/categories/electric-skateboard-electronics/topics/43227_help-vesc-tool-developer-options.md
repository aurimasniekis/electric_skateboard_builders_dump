# \[HELP\] Vesc Tool developer options

### Replies: 20 Views: 808

## \#1 Posted by: XIII Posted at: 2018-01-08T22:07:37.076Z Reads: 120

```
Hi,

Today all of a sudden my Slave Vesc went into OVER_TEMP_FET. 
I'm reading 120 degree Celsius and am not able to run the vesc anymore because I'm hitting the cutoff. 
In Vesc Tool you cannot go over 120 degree and since I am idling at 120-130 atm I cannot even do BLDC or FOC motor setup. 
In developer mode you can overwrite the limits, so I'm planning to just overwrite them and try to work with this. Never ever hit the cutoff Temp of the vesc so I'm pretty safe of running it this way with my settings.

The thermistor is reading 9800 Ohms.
Reflashed the firmware
Used Vesc Tool and BLDC Tool
Vesc from Esk8.de. Less than a year old. 
4.12 VESC

Somoene could help me fix my Vesc or helps me with a looparound for the Vesc Tool?
I don't manage to write these new limits which I write in the developer mode.
```

---
## \#2 Posted by: evoheyax Posted at: 2018-01-08T22:25:27.228Z Reads: 109

```
If you think your VESC is broken, you should get it fixed, not just override the firmware values. Vedder did select that number for a reason and not make it easy to override.

Depending on where you are located, the drv wizard @JohnnyMeduse should be able to help you if you can't find someone locally.
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2018-01-08T22:41:34.908Z Reads: 103

```
[quote="XIII, post:1, topic:43227"]
9800 Ohms
[/quote]

The Termistor seem alright, but maybe you could look into R2 to see if it is 10k (it should not give you 10k but around 8 if I remember correctly)

<img src="/uploads/db1493/original/3X/9/8/98eb048b3e512f136b3ea7174a3b7fe37efaa131.jpg" width="374" height="500">
```

---
## \#4 Posted by: Pimousse Posted at: 2018-01-09T09:33:11.080Z Reads: 75

```
A french guy has the same issue after a run under wet conditions, same value in VESC Tool (around 120°C).
We think that water made a short between MOSFET and R1 (measured at 0.5Ohm).

Check the resistance as @JohnnyMeduse suggested.
Changing a single SMD resistance is not such a big deal if you do it carefully.
```

---
## \#5 Posted by: XIII Posted at: 2018-01-09T16:24:55.863Z Reads: 66

```
Located in EU Belgium ,

R2 is 9kOhm 

@Pimousse did you find a fix ? This could be true in my case aswell. Eu is pretty wet at the moment. Try to cover my vescs with shrink tube and glue gun as much as possible but always a chance water gets in. 

So If I understand correctly my Vesc has a short over the thermistor. The thermistor isn't broken because it still reads 8-9 kOhm. 
Should I try to remove the thermistor and check if there is something shorting the thermistor underneath  ?

Thanks
```

---
## \#6 Posted by: XIII Posted at: 2018-01-09T16:34:34.501Z Reads: 62

```
one extra thing I notice is that my Motor Temp ( no temp sensor installed) is reading -80 degree Celsius. Don't know if this is a correct value.
```

---
## \#7 Posted by: Pimousse Posted at: 2018-01-09T17:10:00.393Z Reads: 56

```
If you don't have motor temp sensor connected, it's normal that you get -80.
On VESC Tool, displaying live value, is the temperature a steady line or does it moe a bit (in other words, is there any "life" on the signal) ?

If the thermistor is 8-9k, you should have something like your ambiant temperature (I hope it's not the ADC which dies...).

Check the pictures of measures on respectively R2 and R1 of the French guy :
http://e-sk8.fr/forum/viewtopic.php?f=25&t=2901&start=10
```

---
## \#8 Posted by: XIII Posted at: 2018-01-10T15:26:34.728Z Reads: 52

```
Can somoene explain me how I can overwrite the settings in developer mode in the new vesc tool? , If I would like to go the path of overwriting the max values

![image|690x351](upload://NQ8KdqXU4N8LPrAkc78KAehdLJ.png)
```

---
## \#9 Posted by: Pimousse Posted at: 2018-01-10T15:37:27.383Z Reads: 51

```
Use the "no limits" FW (available if you display non-standard FW in the list).
```

---
## \#10 Posted by: XIII Posted at: 2018-01-10T15:40:17.273Z Reads: 52

```
.I read your thread on the ESK.FR forum, 
The guy is going to buy a new thermistor. But this will not resolve the problem since the values is stil good.. The problem is that the pcb shorted somewhere... no?
```

---
## \#11 Posted by: Pimousse Posted at: 2018-01-10T15:45:07.529Z Reads: 50

```
He DOES have a fried thermistor (R1) which is 0.5k instead of around 10k (see second picture [here](http://e-sk8.fr/forum/viewtopic.php?f=25&t=2901&start=10#p64682)).
```

---
## \#12 Posted by: XIII Posted at: 2018-01-10T16:59:08.800Z Reads: 43

```
I just uploaded the new firmware default_with_no_hw_limits.
But this only let's me change the current above 100A for Motor max , etc but not the Mosfet Temp.
When I go into the "parameter editor MCConfig"  under developer, I can change the l_temp_fet_start
and l_temp_fet_end.
I can save this as a XML file but how can I insert this into the vesc tool? 
Regards
```

---
## \#13 Posted by: Pimousse Posted at: 2018-01-11T12:53:06.296Z Reads: 38

```
FYI, the french guy (@Toleg , don't know why I didn't mention him before ;) ) solved his OVER_TEMP issue by changing R1 resistor (like a master).
I would not recommend to overpass the temperature limit as it may result in simply disable the temperature protection and thus fry your VESC under load.
```

---
## \#14 Posted by: XIII Posted at: 2018-01-11T13:52:09.207Z Reads: 33

```
But my r1 resistor is Reading 8-9kOhm...
And I have never hit the max temp restriction with my current setup
```

---
## \#15 Posted by: Pimousse Posted at: 2018-01-11T13:53:52.173Z Reads: 34

```
If R2 and R1 are ok, I'm afraid that your issue comes from a dead ADC on the MCU... :neutral_face:
```

---
## \#16 Posted by: Toleg Posted at: 2018-01-17T23:53:20.088Z Reads: 35

```
hi, i'm the guy with the problem :slight_smile:
Can you send a screen capture of your temparature live feed on vesc tool ?
Are your mosfet hot (when you touche them) even when your have just your vesc power on ?
```

---
## \#17 Posted by: XIII Posted at: 2018-01-23T17:43:09.884Z Reads: 35

```
I fixed the problem ! I removed the R1 resistor, and it works now without a temperature reading. Should try to find a new thermistor tho
```

---
## \#18 Posted by: Toleg Posted at: 2018-01-24T13:13:46.914Z Reads: 33

```
https://www.mouser.fr/productdetail/81-ncp18xh103f03rb
```

---
## \#19 Posted by: XIII Posted at: 2018-01-24T20:29:17.644Z Reads: 29

```
you have a spare one? or did you buy just one?
```

---
## \#20 Posted by: Toleg Posted at: 2018-01-25T08:44:11.957Z Reads: 26

```
Have a few spare, can send you one. PM :)
```

---

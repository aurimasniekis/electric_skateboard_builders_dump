# Help with translating hall sensor values from BLDC to FOC

### Replies: 8 Views: 299

## \#1 Posted by: theviith Posted at: 2018-10-10T02:58:35.676Z Reads: 84

```
Hi guys,
Does anyone know how to translate hall sensor values from BLDC to FOC? 
For example, my current hall sensor values under BLDC is: -1, -1, -1, -1, 1, 3, 6, 4 and I want to input this value into the hall sensor table under FOC mode in such a way that it would understand. Based off of some research, I know that a -1 or 0 value in BLDC is equivalent to 255 in FOC. But what about for other values like 3, 6, 4, etc?? Is there a conversion table available to show which values in BLDC corresponds to values in FOC?

My apologies in advance if this is confusing but reason why I am asking is because for some reason, I am able to get sensored mode to work in BLDC by plugging in the hall sensor values directly. But when switched to FOC, the hall sensor detection comes out failed and no values is generated for me to plug in directly like in BLDC. This is why I am asking to see if the hall sensor values from BLDC can be translated to values used in FOC so I can run it in sensored mode in FOC. 

here's some screenshots of what I'm referring to
![12|690x387](upload://yucUTjIvf3Wq30uadiNTbYrXyf2.png)  
this is under BLDC mode. The hall sensor detection shows "failed" but I was able to plug in the values from the generated value and got it to work


![10|690x387](upload://g9OhHJgNk9bcSWosMV0lnygByCx.png)  
this is under FOC mode. Again the hall sensor detection "failed" and this time, there weren't any values generated so I was wondering if I could use the equivalent values from BLDC to plug in to the FOC hall sensor table to get it to work. Does anyone know how to translate the values?
```

---
## \#2 Posted by: threebysix Posted at: 2018-10-10T04:31:36.632Z Reads: 70

```
does the same error still appear if the hall sensor is selected in the Foc mode? Because sensorless is currently selected in your screenshot of FOC mode.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-10-10T04:43:47.374Z Reads: 70

```
Definitely select first HALL instead of sensorless.
Than try if it’s working.
```

---
## \#4 Posted by: theviith Posted at: 2018-10-10T06:47:33.591Z Reads: 63

```
still same results with or without hall selected in FOC. When I click on "measure" under "detect hall sensors" I still get the same error of "bad detection results" with no values given.

here's another screenshot showing exactly just that.
![48|690x388](upload://rE3OMPDlvoeiz1DYrEiQHjVyRCk.png)
```

---
## \#5 Posted by: theviith Posted at: 2018-10-10T07:01:23.894Z Reads: 53

```
I should mention that I'm running on a pair of OM 170kv 5065. The sensor wires have been connected exactly as instructed on a post from other people on this forum with the same motors. I've also tried all combinations of the Hall 1, 2, 3 wires to see if I can get a successful detection in FOC but all with no avail. At this point, I'm inclined to say that it's the motors themselves that's at fault. Then again, it makes no sense how the sensored/hybrid works in BLDC but not in FOC. So if anyone knows a solution to this or has information on how to translate the hall sensor table values from BLDC to FOC, please let me know
thanks!
```

---
## \#6 Posted by: b264 Posted at: 2018-10-10T07:07:52.960Z Reads: 49

```
Have you looked through the source code to try to see what the numbers mean?
```

---
## \#7 Posted by: theviith Posted at: 2018-10-10T07:23:32.627Z Reads: 46

```
source code?
```

---
## \#8 Posted by: b264 Posted at: 2018-10-10T17:57:26.152Z Reads: 38

```
https://github.com/vedderb/bldc
```

---

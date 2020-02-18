# Battery percentage checker

### Replies: 21 Views: 1404

## \#1 Posted by: Jammeslu Posted at: 2017-04-15T13:46:44.298Z Reads: 164

```
going to run 8s3p cells so question is, the voltage indicators on eBay ( cheap ones ) rated between 3s to 15s only do 12v 24v 36v them 48v but my setup is 33,6v so how do I do? will it work or what?
```

---
## \#2 Posted by: mmaner Posted at: 2017-04-15T13:54:50.020Z Reads: 162

```
The volt value will still be correct, only the percentage will be off by a small amount.
```

---
## \#3 Posted by: Jammeslu Posted at: 2017-04-15T13:56:20.200Z Reads: 159

```
so if I buy one I should put it at 36v?
```

---
## \#4 Posted by: mmaner Posted at: 2017-04-15T13:59:41.706Z Reads: 150

```
Correct, 36v.
```

---
## \#5 Posted by: Jammeslu Posted at: 2017-04-15T14:45:32.620Z Reads: 134

```
yeah do you know how many percent the difference will be? I assume silmillar to like 95% is 10%?
```

---
## \#6 Posted by: mmaner Posted at: 2017-04-15T15:04:12.878Z Reads: 126

```
100%/x%=36/33.6
(100/x)*x=(36/33.6)*x       - we multiply both sides of the equation by x
100=1.0714285714286*x       - we divide both sides of the equation by (1.0714285714286) to get x
100/1.0714285714286=x 
93.333333333333=x 
x=93.333333333333

now we have: 
33.6 is 93.333333333333% of 36
```

---
## \#7 Posted by: Jammeslu Posted at: 2017-04-15T15:20:41.295Z Reads: 120

```
thanks alot
```

---
## \#8 Posted by: mmaner Posted at: 2017-04-15T16:13:52.645Z Reads: 122

```
No worries.
```

---
## \#9 Posted by: PXSS Posted at: 2017-04-16T03:27:50.605Z Reads: 101

```
Jesus. 
You could've just done 
33.6/36 = 0.9333

E: BTDubs, thats not how those percentage meters work. Your battery capacity does not correlate linearly between 36V and 0V. 
There is a discharge curve between 42V and 30V for a 10S (36V) display. The percentage is mapped to voltage based on this curve. 36V is ~50% in this curve and 33.6V is ~10% so your display will almost always show 0% if you get that. 

Look up LY6N or LY6W battery display. Those work for 8S too.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-04-16T03:36:34.732Z Reads: 104

```
Yeah Jesus don't worry.... cause he came back to life this weekend
```

---
## \#11 Posted by: PXSS Posted at: 2017-04-16T03:40:16.070Z Reads: 110

```
Completely forgot it was Easter...
```

---
## \#12 Posted by: Namasaki Posted at: 2017-04-16T06:38:21.421Z Reads: 105

```
I think most of those meters do 12,24,36 and 48 with lead acid batteries but they also do 3s to 15s lithium batteries.
This one does both:
http://www.ebay.com/itm/12V-24v-36V-48V-Lead-acid-Lithium-Indicator-Battery-capacity-Tester-volt-meter/172018886570?_trksid=p2047675.c100005.m1851&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D40130%26meid%3Dd113753123854c1a95c8a63e1d5535d4%26pid%3D100005%26rk%3D5%26rkt%3D6%26mehot%3Dpp%26sd%3D331810603701

<img src="/uploads/db1493/original/3X/6/0/606fff106ccf401a3fe0f1b294230bf78ec301d7.png" width="677" height="500">
```

---
## \#13 Posted by: Jammeslu Posted at: 2017-04-16T08:47:48.639Z Reads: 93

```
Yeah so What do i do for A 8s setup?
```

---
## \#14 Posted by: PXSS Posted at: 2017-04-16T12:04:56.476Z Reads: 85

```
He literally just pasted the instructions above...
```

---
## \#15 Posted by: Jammeslu Posted at: 2017-04-16T13:43:06.408Z Reads: 78

```
yeah for 12,24,36 and 48V 8s is 33.6 literally...
```

---
## \#16 Posted by: PXSS Posted at: 2017-04-16T16:25:26.485Z Reads: 72

```
If you're not willing to read then I cannot help you
```

---
## \#17 Posted by: Jammeslu Posted at: 2017-04-16T17:18:49.626Z Reads: 70

```
I have already looked at the ly6n and w and its the same, supports 8s but only 12,24,36,48v
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2017-04-16T17:19:52.210Z Reads: 70

```
put it in **L8** mode..... it's made for 8s battery.... :confused:
```

---
## \#19 Posted by: Jammeslu Posted at: 2017-04-16T17:20:33.350Z Reads: 67

```
And What volt setting?
```

---
## \#20 Posted by: JohnnyMeduse Posted at: 2017-04-16T17:21:55.418Z Reads: 70

```
It's automatic..... the setting is L8... like 8s = 8string battery
<img src="/uploads/db1493/original/3X/0/5/0563e494d1313cc7526ccdd1a7dd6038121925fb.png" width="677" height="500">
```

---
## \#21 Posted by: Jammeslu Posted at: 2017-04-16T18:14:17.219Z Reads: 65

```
Oh now i get it
```

---

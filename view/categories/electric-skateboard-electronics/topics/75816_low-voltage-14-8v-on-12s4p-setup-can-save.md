# Low voltage 14.8v on 12s4p setup can save?

### Replies: 21 Views: 642

## \#1 Posted by: huzaini Posted at: 2018-11-24T08:14:03.661Z Reads: 117

```
hi guys i have problem with my battery, i probably accidentally set a wrong setting thrue vesc tool setting. i have 12s4p battery now on low voltage which is 14.8v , 1.3v per pack, the problem is i set my battery to 12 cells on voltage without pressing apply button on vesc tool. my setup is 
flipsky dual fsesc 6.6 
12s4p sony vtc6
flipsky 190kv 6374 motor
and trampa hollipro hs11
bluetooth module from flipsky. 
smart switch
and bms

1) is it possible to save my battery from 1.3v per cells /pack ? 
2) what's the risk? 
3) can i just charge using normal 50.4v 12s 4a charger?(still on shipping)

![2|690x459](upload://A916BNHQrEWIvKJBTj7bJNocVpg.jpeg) ![1|690x459](upload://2bp2Y8JwdY7JwGlGz3JIGdgQt1Q.jpeg)![3|690x378](upload://mtWj0JmVO9ISzxKBfqBNIYZ7jeK.jpeg)
```

---
## \#2 Posted by: visnu777 Posted at: 2018-11-24T08:21:08.343Z Reads: 108

```
Are you sure every P pack is at 1.4? Did you measure them? AFAIK the default values for cutoff are for at least 10s?

edit: oh, I see its way lower :(
```

---
## \#3 Posted by: taz Posted at: 2018-11-24T08:23:03.749Z Reads: 105

```
1.Yes you can. However you have caused some damage to your battery.
2.No risk as long as you monitor the voltages as it is charging.
3. Probably not. You can do it with a hobby charger set to Nimh or Once and charge each p group through the balance leads. Use a low current per p group (1A would be ok) until it reaches 3.1-3.2V. Once all the p groups are at this voltage continue with your normal charger.
```

---
## \#4 Posted by: huzaini Posted at: 2018-11-24T08:23:41.593Z Reads: 99

```
yeah m8, but i havent ride at all, just setting thrue vesc tool. from 39.39 drop to 14.8 :frowning:
```

---
## \#5 Posted by: huzaini Posted at: 2018-11-24T08:26:50.281Z Reads: 96

```
that's really convincing, gotta try that out, because i not even ride it even once before. just bench test and there my battery goes. but how it possible to drop that much just from bench test , 2 days figureit out using vesc tool.
```

---
## \#6 Posted by: taz Posted at: 2018-11-24T08:30:28.663Z Reads: 90

```
3.2V per cell is only 5-10% charge.
Li-ion cells drop in voltage very fast after that.
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-11-24T13:01:41.299Z Reads: 80

```
When you try to breathe life back into the battery, do you have anywhere safe to put it?

Lipo bag.... Outside.....

Be safe :0
```

---
## \#8 Posted by: Livid Posted at: 2018-11-24T13:04:17.574Z Reads: 81

```
I recovered a 10s2p from 10v using a normal 10s charger. used it for 3 years after that
```

---
## \#9 Posted by: huzaini Posted at: 2018-11-24T13:53:56.960Z Reads: 77

```
My friends also suggest me to charge it first using normal charger. Since I don't have the charger now gonna have to wait for shipping. Hopefully bms would help and can be charged.
```

---
## \#10 Posted by: huzaini Posted at: 2018-11-24T13:54:34.673Z Reads: 78

```
Sound dangerous things. Some friend said Can be charge hmm
```

---
## \#11 Posted by: Sn4pz Posted at: 2018-11-24T14:28:10.847Z Reads: 69

```
It can be done, it's just that reviving a battery (depending on it's composition) can sometimes be dangerous


Also it should be said that when cells are revived, sometimes they lose.... Capacity (? Not sure how to explain it, but just know that your range might take a hit.)

Additionally, internal resistance *may* increase. 

Alot of forums talk about how panasonic, sanyo and some Samsung cells can be revived with ease, just proceed with caution!
```

---
## \#12 Posted by: huzaini Posted at: 2018-11-24T16:01:09.129Z Reads: 64

```
thanks m8 im gonna try to charging it using normal charger first
```

---
## \#13 Posted by: Sn4pz Posted at: 2018-11-24T16:02:54.655Z Reads: 64

```
alright, just make sure that if your charger is rated for any more than 2 amps that youre checking the temperature of the cells/ the pack occasionally. 

The same thing happened to my space cell, as and I was trying to recharge it with its original (2a) charger, the pack became VERY hot. 

It took a ride to the disposal center later that day :/
```

---
## \#14 Posted by: huzaini Posted at: 2018-11-24T16:10:26.182Z Reads: 61

```
That's what I'm worried about. Need adjustable charger maybe? So I should start charging from normal charging port using 1a isn't?
```

---
## \#15 Posted by: Sn4pz Posted at: 2018-11-24T16:12:25.174Z Reads: 59

```
the amperage is dictated by your charger. maybe take a picture and show? :) 

1a, or even .#a is fine, 2a generates heat in battery packs regardless, so staying lower is better in this circumstance
```

---
## \#16 Posted by: huzaini Posted at: 2018-11-24T16:16:46.261Z Reads: 58

```
i dont have the charger right now. because i just order this week probably next week i can get it. the one i order is 50.4v 4a , or i need to find exactly 1a to play safe?
```

---
## \#17 Posted by: Sn4pz Posted at: 2018-11-24T16:21:36.806Z Reads: 57

```
4a would almost certainly cause a malfunction.

lower a is the way to go, 1a or less would be my reccomendation
```

---
## \#18 Posted by: jmasta Posted at: 2018-11-24T17:34:47.715Z Reads: 47

```
This is how lithium battery fires start....
```

---
## \#19 Posted by: Hummie Posted at: 2018-11-24T18:10:53.346Z Reads: 49

```
4a for a 4p battery not low enough current?  One amp rate too slow for reviving?
```

---
## \#20 Posted by: thisguyhere Posted at: 2018-11-24T18:11:22.164Z Reads: 49

```
Read pack voltage directly from battery, if it's really 15v, batteries are dead. 

That makes each P group 1.2v, way below the 2.5v threshhold. It means you've altered the internal resistance of every cell in your pack that can lead to all kinds of issues, premature heating is for sure one of them. 

To make sure, measure each P group voltage. Stick voltmeter positive to pack positive, then read each balance lead voltage. Write it down and when complete, take voltage difference in each subsequent P number, that'll give u each P group voltage. 

Kind of silly to not have set the cutoff correctly, not sure where u learned to program your controller but now it's going to cost you.
```

---
## \#21 Posted by: PXSS Posted at: 2018-11-24T19:21:22.060Z Reads: 35

```
The longer you wait, the more damage you cause to the cells since they're not meant to be in that state. So try to get them charging as soon as possible. 


Check individual cell voltages!!!!!!!!
---
This is the most important thing you need to do. You need to verify that all the cells are above 1V. If any of them is below 1V, do not charge the battery. This is explicitly stated in the datasheet of the cells. Charging a battery under 1V has a high risk of fire. 

Keep the cells cold. Between 5C and 15C ideally.
Between 0C and 20C is ok. 
Charge cells slow. 0.5A per cell or lower. (2A or less for a 4P)
Keep an eye on temperature when charging. Anything above 35C and you should let the cells rest before continuing. 
Do not use a BMS when recovering cells from under 2.5V. 
Check voltages constantly with a multimeter, making sure they are charging evenly. 
Charge to at least 3.6V before connecting BMS. 
Charge outside on concrete surface in case of fire. 
After you charge to 3.6V let battery sit for an hour or two at room temperature. 
Plug in BMS and charge normally to 4.2V. 
Check that cells are balanced to 50mV at worst. 

If you do not follow all of these steps exactly how I wrote them, you are risking your battery and surroundings to a very serious fire. 

VTC6s are some of the most resilient cells out there but you must be extremely careful still.
```

---

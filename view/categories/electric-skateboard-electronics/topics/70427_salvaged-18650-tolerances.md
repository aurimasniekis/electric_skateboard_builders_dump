# Salvaged 18650 tolerances

### Replies: 12 Views: 249

## \#1 Posted by: ramon Posted at: 2018-10-07T11:16:52.510Z Reads: 108

```
Hi,

Right now Im testing the capacity of some 18650 cells I salvaged from old laptops. 

My idea was to build for a battery pack for a personal project with cells arround 2500mah and for the moment I have 7 of them with that capacity (I expect to reach 12 once I finish to test all my cells and this way I will be able to build a 3s4p battery pack). 

My problem is that those cells which are arround 2500mah are not the exact same capacity, they range from 2359 to 2565 mah and I was wondering if this difference in capacity, which represents a 9% from one cell to another in some cases, would damage my battery pack on the long run.

Obviously it would always be better to have new batterys with exactly 2500 mah each, but since its not the case and I dont have a lot of money to spend on this project, I would like to know if ithat 9% difference in capacity would really make a difference.

Thanks in advance
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-07T11:24:29.801Z Reads: 103

```
What you need to do is put them into groups that will add to a similar capacity. For example if you have 3x 4ah, 3x 2ah and 3x 3ah you want to put one 2ah with a 3ah and 4ah in parallel. That way you will get 3 groups of parallel packs with a total of 9ah then connect them into series for a 3s3p. 

I know this will be harder to work out as you will be working in smaller integers but this is the best way to do it. The main thing is to have the same capacity in each parallel pack +- about 100mah. I would also not push these cells at more than 2c and have the cut off voltage set to 3.2v per cell.

Btw what sort of project is this for?
```

---
## \#3 Posted by: Fiori Posted at: 2018-10-07T11:33:40.395Z Reads: 90

```
Were you able to salvage these batteries for free or something? Because hover board battery packs that are 10s2p preassembled with a BMS already installed are around $40. They may not be the best cells, but at least they are all new and of the same capacity.

You wont have very much fun with a 3s battery. Unless this personal project isn't an esk8?
```

---
## \#4 Posted by: ramon Posted at: 2018-10-07T12:10:47.824Z Reads: 85

```
Thanks for your heIp. I wanna build a "diy nintendo switch" with a raspberry pi zero with retropie, a laptop screen, a driver for the laptop screen, 3d printed enclosure, some cheap usb controllers, usb ports, bms, etc... So power draw will not be a problem since it will be arround 2/3 amps. So the important thing is to have same capacity on the packs which are in series but I can have different capacity on the ones which are on paralel right??
```

---
## \#5 Posted by: ramon Posted at: 2018-10-07T12:13:23.796Z Reads: 75

```
Thank you for answering :smile:. Its for another project, and I got those cells for free :slight_smile: I only need a 12v input since its what the electronics Im using require, and I dont need a huge discharge capacity since it will only be drawing arround 2/3 amps.
```

---
## \#6 Posted by: Eboosted Posted at: 2018-10-07T12:42:11.245Z Reads: 65

```
What's your method to meassure the capacity in such an exact way?
```

---
## \#8 Posted by: ramon Posted at: 2018-10-07T13:21:17.955Z Reads: 53

```
I use my balance charger to do a full charge to 4,2 v, then a full discharge to 3v where I write down the mah drawn, and finally a storage charge (for each cell individually). Im sure there are faster ways to do it, but Im not in a hurry :slight_smile:
```

---
## \#9 Posted by: pat.speed Posted at: 2018-10-07T20:56:30.893Z Reads: 35

```
Yep that’s right. You will end up with 3 lots of 4 cells grouped together. Those 4 cells can have different capacities but you want the 3 groups to have a similar capacity. That way you might have a 7.5ah 7.6ah and 7.4ah and then connect them into series
```

---
## \#10 Posted by: Kug3lis Posted at: 2018-10-07T20:57:23.113Z Reads: 34

```
P.S. Laptop cells will sweat as fck if you pull more than 10A iirc
```

---
## \#11 Posted by: ramon Posted at: 2018-10-07T21:26:51.562Z Reads: 31

```
Dont worry, its for powering a screen and a raspberry pi which combined pull less than 3A, but thanks for the advice :slight_smile:
```

---
## \#12 Posted by: spesh Posted at: 2018-10-07T22:56:20.062Z Reads: 22

```
http://repackr.com
```

---
## \#13 Posted by: ramon Posted at: 2018-10-08T07:20:13.429Z Reads: 16

```
Thanks!!! That will be very useful once I finish testing all my cells!
```

---

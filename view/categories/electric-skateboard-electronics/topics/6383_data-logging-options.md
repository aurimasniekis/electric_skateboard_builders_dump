# Data logging options

### Replies: 11 Views: 1641

## \#1 Posted by: kaspars Posted at: 2016-07-20T18:28:13.163Z Reads: 119

```
Continuing the discussion from [The nicest hub motors! For sale cheaper than anywhere!](http://www.electric-skateboard.builders/t/the-nicest-hub-motors-for-sale-cheaper-than-anywhere/1002/873):

So what do you use for data logging and analysis?

At the beginning of last year I discovered the [Speedict](http://www.speedict.com/index.jsp) ebike computers. I got myself the Speedict Mercury for comparing the efficiency/performance of various ebike controllers. It measures voltage, current, temperature and speed (both from a sensor and from the GPS data on the phone). All of the data is stored on the device and can be viewed real-time on an Android device (no iOS support) or downloaded as a CSV file. There is also an option to upload the data to their online viewer -- here is a [sample output](https://www.flickr.com/photos/speedict/5863042469) from the time when the Google Maps integration was still working:

![](https://c2.staticflickr.com/4/3160/5863042469_f4355b31d3_o_d.png)

and here is my latest ride: http://chart.speedict.com/?weblogid=14O05v057212111

The [Android app](https://play.google.com/store/apps/details?id=com.speedict.client.mercury&hl=en) was last updated on December 11, 2014 and has a few bugs so I feel like they have shifted their focus to either their [BMS solution](http://speedict.com/) or something entirely different. Luckily the CSV export works fine and Google Sheets does its magic -- here is the [same ride on Google Sheets](https://docs.google.com/spreadsheets/d/1vkZ-jQeM24SSwWPWIu-X-8dAZqcYbyWDF7JQso06cT0/edit):

![](https://c2.staticflickr.com/8/7704/28225977422_3058d474ba_o.png)
```

---
## \#2 Posted by: sl33py Posted at: 2016-07-20T18:52:16.140Z Reads: 114

```
Very cool.  I saw those a while back, but didn't see (maybe wasn't developed yet) the bt integration w/ the phone.

I have an Eagletree v4 logger (uninstalled) - which can do some of the same, but not quite as smooth of an interface.
```

---
## \#3 Posted by: Hummie Posted at: 2016-07-20T23:03:38.933Z Reads: 96

```
how bout the vesc?  how hard is it to set up some recording of what's going on?  it's all in there already if it could just be recorded
```

---
## \#4 Posted by: kaspars Posted at: 2016-07-21T08:12:52.230Z Reads: 81

```
Looks like VESC has [an UART interface](http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/). I found [this sample project on GitHub](https://github.com/RollingGecko/VescUartControl) for Arduino. We could attach one of those cheap [UART to Bluetooth modules](http://www.ebay.com/sch/i.html?_nkw=UART+bluetooth) to VESC and do all the communication via Bluetooth on any device. Too bad I don't have a VESC.
```

---
## \#5 Posted by: Hummie Posted at: 2016-07-22T19:30:37.457Z Reads: 70

```
Is hat the simplest way to simply record?  Id like to see the realtime graph of my riding later.
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-07-22T19:37:23.603Z Reads: 65

```
I just sent somebody one of my VESCs, he's working on an iphone app to give RPM based speed in mph and kph, as well as data stuff. works over blue tooth. I'm looking forward to testing prototypes. It would be nice to see realtime current draw and all of that stuff on there too, i'm hoping he can work it in.
```

---
## \#7 Posted by: kaspars Posted at: 2016-07-23T05:14:29.068Z Reads: 53

```
Are you referring to VESC and UART? It seems to be the easiest from what I understand.

@longhairedboy Is that how your app will work -- via the UART data stream?
```

---
## \#8 Posted by: kaspars Posted at: 2016-09-01T20:24:23.977Z Reads: 46

```
@longhairedboy Do you have an update on the data logger project? I'm wondering if he managed to get the necessary data out of VESC.
```

---
## \#9 Posted by: Hummie Posted at: 2016-09-01T21:46:57.621Z Reads: 44

```
its now done I believe.  slowturtle or something is the app.  if you search here you'll find it.  cant do everything in the bldc tool but some and records
```

---
## \#10 Posted by: kaspars Posted at: 2016-09-02T06:56:29.220Z Reads: 41

```
Thank you! Here it is http://www.electric-skateboard.builders/t/ultimate-vesc-controller/6014/
```

---
## \#11 Posted by: PB1 Posted at: 2016-09-02T07:35:11.734Z Reads: 39

```
think @hummie is reffering to the android solarturtle Vedder ESC app
https://endless-sphere.com/forums/viewtopic.php?f=35&t=68975&start=100#p1211940 

@makevoid is also working on data logging
```

---

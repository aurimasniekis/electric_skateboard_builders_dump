# Capacitors to increase Max Current output

### Replies: 6 Views: 396

## \#1 Posted by: NilsS Posted at: 2017-05-04T12:58:34.150Z Reads: 80

```
Hi, i am using 18650 with a Max current output of 5,6Amps. I have 7 in Paralel so i am loking for a way to increase it. So I found the idea of using Caps. The two I have are each 50V 4700uF how long do you think they could run at 60a? My pack is 7S
```

---
## \#2 Posted by: B4Me Posted at: 2017-05-04T13:00:48.226Z Reads: 80

```
some milliseconds if not micro seconds
```

---
## \#3 Posted by: JohnA Posted at: 2017-05-04T13:04:09.222Z Reads: 78

```
You could make a pack of maxwell boost caps, those would do something. But they are 2.7v each so it wouldnt be cost efficient for how many you would need. 

Caps themselves: http://www.ebay.com/itm/Maxwell-310-Farad-2-7V-Ultracapacitor-Supercapacitor-D-Cell-Boostcap-X-2-pieces-/132177696865?hash=item1ec6679861:g:pNYAAOSwq7JUEc8I

Pre made battery pack: http://www.ebay.com/itm/12V-super-capacitor-module-6x-350-farad-caps-300A-engine-starting-car-audio-/112204472039?hash=item1a1fe85ee7:g:wxEAAOSwg3FUovjv
```

---
## \#4 Posted by: NilsS Posted at: 2017-05-04T13:15:40.230Z Reads: 70

```
I am just gonna 2 cells in parallel so it's 45A instead of 35A 9P7S. -_-
```

---
## \#5 Posted by: JohnA Posted at: 2017-05-04T13:33:44.187Z Reads: 69

```
That works. Something to consider though is the higher the voltage of the system the less amps needed. 
This is because to reach 1000 watt at 25.2v (7s) requires 40 amps, but in a 36v (10s) it would only need 27 amps. (W=V*I)
May be worth thinking about a higher voltage battery, cells that have more amp output, or using a vesc where you can limit the amps pulled from the battery.
```

---
## \#6 Posted by: NilsS Posted at: 2017-05-04T15:00:33.532Z Reads: 54

```
Yeah thought of that, but I didn't have enough cells for 10S5P I had 49?!? ikr, but I will beg my Computer Teacher for some more so I could make an insane 10S7P battery. That would be INSANE considering I already have 500wh
```

---

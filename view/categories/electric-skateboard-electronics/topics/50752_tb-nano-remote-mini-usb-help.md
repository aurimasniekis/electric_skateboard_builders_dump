# TB Nano remote mini USB help

### Replies: 7 Views: 444

## \#1 Posted by: TheFluffiest Posted at: 2018-03-31T06:39:25.741Z Reads: 72

```
Hi all,

Today the mini USB port that charged the tiny lipo battery in the TB Nano remote fell off. I think this was due to a crash, an then repeated yanking of the usb cord out. 

Does anyone know how to fix this, or how to install a different charger? It just needs 5v right?

Some pictures of what I mean:
!mlTS2XtpvfKmQ7P2ucKHkuD7los[20180330_234754|374x500](upload://.jpg)

![20180330_234808|374x500](upload://A0q1KYYAOQJ5t3Pq29nxL1L08lv.jpg)
```

---
## \#2 Posted by: ARetardedPillow Posted at: 2018-03-31T10:20:36.114Z Reads: 63

```
Correct me if I'm wrong, I'm not an expert at micro usb ports lol.

I think you only need to solder the port back to the 2 big pads on the remote since all it takes to charge a battery is a positive and a negative pole. 

I have no idea what the middle lines between those 2 pads are though. If anyone is more experienced in this field please correct me if I'm wrong
```

---
## \#3 Posted by: Aleks Posted at: 2018-03-31T10:29:44.002Z Reads: 59

```
the 2 big ones are just anchor pads.  the inbetween are the actual usb connection lanes, 2 of which would be +/- and the others are normally for actual data transfer on usb, which are not used in this remote.
```

---
## \#4 Posted by: TheFluffiest Posted at: 2018-03-31T13:47:13.474Z Reads: 49

```
@ARetardedPillow @Aleks  

I'm pretty sure the copper on the anchor pads came up completely, so I will have to glue those down. I'm guessing by the pictures, the left two pads are the +and-. Anyone have confirmation on this?
```

---
## \#5 Posted by: Meche Posted at: 2018-03-31T18:20:05.486Z Reads: 39

```
![Inkedfc5a6959afb5fbf88c3c6a1975c6b3253b864465_1_374x500_LI|374x500](upload://sEQ9P8GjmkDHUHUhmN08p1wGh26.jpg)

Like this if you understand my drawing :slight_smile:

You need to anchor the micro usb first also and you need to scrape of the soldermask(green) off to get to the copper so that you could solder. Be careful with that as it tends to get loose...

Insted of scraping off you could also bridge the powerline with that cap C8 if im reading correct

You also need to solder in GND as you ripped the big pads off... easy way is also to solder on the housing of the micro usb to any GND or if you are lucky the pad that is there is till in good condition
```

---
## \#6 Posted by: TheFluffiest Posted at: 2018-03-31T19:48:32.769Z Reads: 29

```
@Meche 
I understand the drawing. Could I glue the mini USB in order to anchor it? Or can I "restore" the copper on the pads? How would I solder to the C8 cap? I see what that is, I'm just not entirely sure where on it :joy:  

Where is the closest ground I can solder to? 

Thank you for your help!
```

---
## \#7 Posted by: TheFluffiest Posted at: 2018-04-01T05:57:41.661Z Reads: 20

```
Didn't seem to work. I will have to try it with a different battery and see if it works better
```

---

# VESC 4.12 Broken, dim blue &amp; red light on, usb not recognised

### Replies: 5 Views: 267

## \#1 Posted by: adrianlee Posted at: 2018-06-12T20:18:35.784Z Reads: 51

```
Soo I tried to replace DRV module without solder paste or proper tools and the results are not great. Just putting this here if someone would notice on the pictures if I missed something obvious, or if the board is just fried.

* dim red and blue lights on when powered
* USB connection not working
* DRV module changed
* I might have overheated the board with my 350c superblower
* Yes those plastic ports melted even though I was using keplan tape

![19|500x500](upload://a7Qr7Mwux5bHwhHMe96meEMP28n.jpg)![38|500x500](upload://opqLOepeVwnNdEDJUjdRfGl4oP8.jpg)![14|500x500](upload://8RIo9eTJNhcKTkEKJmHRuwUpOF3.jpg)![05|500x500](upload://ayBO2pgcV3Kueof4DI5tIqtcF6b.jpg)
```

---
## \#2 Posted by: Ishayc Posted at: 2018-06-13T08:03:23.916Z Reads: 35

```
After you replace the drv chip you need to flash a bootloader if i'm not mistaken otherwise the PC will not recognize it.
```

---
## \#3 Posted by: adrianlee Posted at: 2018-06-13T11:23:40.208Z Reads: 29

```
I couldnt find any info about that, for my understanding you only need to flash if you change the MCU?
```

---
## \#4 Posted by: Kug3lis Posted at: 2018-06-13T11:24:58.246Z Reads: 30

```
drv has nothing todo with bootloader
```

---
## \#5 Posted by: Ishayc Posted at: 2018-06-13T12:06:00.418Z Reads: 27

```
Yup my bad. Mixed up between MCU and drv.
```

---

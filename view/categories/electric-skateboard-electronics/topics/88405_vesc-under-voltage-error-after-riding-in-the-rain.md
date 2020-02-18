# VESC Under Voltage Error after riding in the rain

### Replies: 4 Views: 135

## \#1 Posted by: Chupacabra Posted at: 2019-03-26T20:16:23.226Z Reads: 39

```
Hi Guys,

I am using the Flipsky dual VESC 6.6 plus. Yesterday i was riding in the rain and on the way back I found that my motors were cutting off. The motors kept stuttering and I barely made it back because slowly the vesc completely stopped responding. 

Today when i opened the enclosure and dried it out, I see that I am getting a fault code of Under Voltage.  Also there is a red light that keeps flashing on the VESC.

![Capture|690x407](upload://lHRSEJLtohzhuizzjPtICAmMpIT.png) 

I have the maytech motors 6374 190 KV and I'm using these settings. 

![Capture4|690x358](upload://8toBAEp6HsRqQStm1CXZWw8z47A.png) ![Capture3|690x376](upload://rHMN53OlCjTpqCUFfHEr2xrLdxL.png) ![Capture2|690x319](upload://oxHLeoSr6WmhN3guCQc6Ik2gHqT.png)

Here is a video of the vesc and the red light that keeps flashing on the master. Any help will be appreciated!

https://youtu.be/D0eXEWw7aQM
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-03-26T20:31:19.596Z Reads: 35

```
Looks like there's are shorts/corrosion between pins on the STM32F405RG, as well as surrounding passive components.

Wherever you see corrosion, lightly touch up the solder joints with generous amounts of flux and modest amounts of solder. 
Be careful not to create any solder bridges or knock off any passive components.

I highly recommend watching some of Louis Rossman's videos on youtube if you are unfamiliar with SMD soldering.
```

---
## \#3 Posted by: Chupacabra Posted at: 2019-03-26T20:35:41.690Z Reads: 35

```
Wow I cant believe it. I used about 5 coats of conformal coating all over the vesc. Could it just be that the conformal coating has scrapped off?

Also could you tell me what part you’re talking about ?

![image|375x500](upload://21EyiV6HFJuTMmjJNCCG6f0RE0E.jpeg) ![image|375x500](upload://d0ydDKCKv8YOmjJImLoD781XPDE.jpeg)
```

---
## \#4 Posted by: Gamer43 Posted at: 2019-03-26T20:37:46.569Z Reads: 33

```
Not sure, but one way or another, water made its way into the components and caused corrosion between components.

The top one actually looks like it's in pretty good shape, but there is definitely corrosion between pins and components of the bottom one, I'm guessing the conformal coating didn't spread evenly on the bottom one?
By corrosion, I mean the foggy white stuff that see on some components on the bottom one, it's on multiple components, from what I can see, many pins on the STM32 (the big square chip with 64 pins and the QC sticker) and the surrounding resistors and capacitors.
```

---

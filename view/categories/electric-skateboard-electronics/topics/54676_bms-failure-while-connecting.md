# BMS Failure while connecting

### Replies: 4 Views: 365

## \#1 Posted by: Acidfie Posted at: 2018-05-07T10:39:42.623Z Reads: 70

```
So i just finished my 12S batterypack and wanted to connect my BMS System. My BMS is the HCX D196 from Bestech. As soon i connected the JST Plug i've seen some little smoke plume, just really really tiny. I've checked everything twice but i still have no clue what was wrong. Maybe someone had the same experience like me here.. i don't want to let my battery die because of a stupid mistake..

This is the spot where i think the smoke leaked:

![IMG_0248|666x500](upload://e4mfLwv9FzcG2GZhVIbFLqvKFlA.JPG)

The JST plug with the balancing cables

![IMG_0245|666x500](upload://AcD22kAIGy6Jk0yGOdn3z0axIDj.JPG)

The B- port

![IMG_0247|666x500](upload://dbAGJAoTaHyZo76xTJLmOkXCKij.JPG)

The whole battery pack, i measured from the + to every balance lead, everything correct.

![IMG_0244|666x500](upload://9MGeIb1lsI1lA7JRgfEXMVCUQeU.JPG)

The BMS PCB, top left you see C- (Charging -)

![IMG_0246|666x500](upload://sCov02duOdL8wTwdBCw6n99x59B.JPG)

The plan i received with the BMS from Bestech.

![IMG_0249|557x500](upload://kYwL8Z9yPamaHQEKa0dAiVQKjhi.JPG)
```

---
## \#2 Posted by: sMATTEr Posted at: 2018-05-07T11:24:53.305Z Reads: 50

```
Where does your c- go?
```

---
## \#4 Posted by: Acidfie Posted at: 2018-05-07T14:39:46.816Z Reads: 40

```
C- is not connected/connected to the DC-Charging Port
```

---
## \#5 Posted by: Acidfie Posted at: 2018-05-07T14:45:12.305Z Reads: 38

```
nvm. i think i have it.

i chosed the wrong pin, i used the pin for the temp sensor, thats why i caused this to happen. 

The JST has 13 pins, one is not needed since its 12S, i started from the wrong way, thats why it burned down the temp sensor conduct
```

---

# Burned flipsky vesc, bldc and bms

### Replies: 1 Views: 135

## \#1 Posted by: Starymis Posted at: 2019-10-24T02:37:58.903Z Reads: 55

```
Hi, I would like to ask for help in locating the fault that results in burned bldc (sk3 6374) , vesc (flipsky 4.12) and bms (bestech) . A few days ago on the way home, constant speed, my board suddenly braked and fired me like a catapult. When I got up and walked to the board, no response to remote. Bldc resisted clearly. After a few seconds smoke started coming out and and stoped few seconds later. When I opened the enclosure almost everything was burned apart from the battery and receiver. At the moment, bms smell and always gives current - the switch does not work.  
I noticed then that the balance connector was a little bit loose (possible cause?).
![IMG_20191018_082256_HDR|666x500](upload://xpBZPozqCepW7bMR7KIdHTRGyWN.jpeg) 
![IMG_20191011_082419|666x500](upload://kM32osl7kgSqWuAdCB48PqRmYJD.jpeg) 
Then vesc has burnt drv and a loose cable from the capacitors loose (heatshrink melted along the entire length of the cable). During the extraction, I noticed that one of the vesc - motor cables was loose (possible cause). Was soldered over half a year ago and never caused problems. I know that full braking can occur with connection problems but could it burn everything? ![IMG_20191018_082309_HDR|666x500](upload://gRAjjNQF2upp31sXx6Q2UyE60vN.jpeg) ![IMG_20191018_082325_HDR|374x499](upload://7yC4YmLg2cqZRGx8Vl3gucv1OnD.jpeg) ![IMG_20191011_084351_HHT|666x500](upload://66eR3C9dfFy1FNtJcPgHEAMtrvL.jpeg) 
Bldc I did the A + B, B + C, A + C test. When the connection of all three wires together gives proper resistance, when I have them separated it gives a "different" resistance and each combination with wire B does not work. The winding in the motor is additionally covered with resin and despite the appearance of burns (resin and dust) underneath is pure copper.
![IMG_20191012_051917|375x500](upload://2Ojqo5WJGP5TejBNdZzQvI53x7A.jpeg) ![IMG_20191012_051914|375x500](upload://gFY45rsSVCK3yaxNtmiQUPcib7C.jpeg) ![IMG_20191018_082402_HDR|666x500](upload://ddvhvMAG8Skx4JyTEb7Wh2ox7XR.jpeg) 
The battery was the only one left unscathed. Gives correct voltage from the cells.
My setting was Motor max 50, batt max 40,
```

---

# Help needed with wiring Bestech 10s BMS

### Replies: 3 Views: 474

## \#1 Posted by: Pingo03 Posted at: 2018-04-13T21:26:21.625Z Reads: 110

```
Hello,

After getting my new Bestech BMS and focbox I was having troubles with the battery dying mearly instantly and don’t being able to charge it, I think my wiring is wrong!

My setup is a 10s3p battery 
Focbox (also new)
Bestech 60A 10s Bms 
Maytech 6355

Settings of the Vesc:
Foc mode
motor max 60amps, motor min -45a
Batt max 40amps min -12a
Erpm 60000 and -60000(changed on the 3rd ride)
1.My first ride was great no issues but I did not charge the battery as I charged it before with the old bms

After this I plugged in the charger for a few hours and took it for a ride, I did not check the light on the charger as I only presumed it would work even if the lcd immediatly showed 100% when plugging in the charger.
 This is what happend during the ride: 4 overvoltage faults and a dead battery afterwards. 
https://metr.at/r/e0yXE

While getting back home charging of the battery doesnt work as the charger only does show green light as if the battery was full.
Here the wires were soldered like in the sheme attached that I found on the internet so soldered onto the CHG-
Xt60-   - of charger and -of LCD


3. After this I knew something was wrong with the wiring amd somebody told me to just move all the 3 wires from CHG- to DSG-. This did work to charge the board at first I took it out for another ride and pretty soon got brake cut off and a dead battery after 2kms. Faults were overcurrent and after that overvoltage https://metr.at/r/KEKIC
Now when I want to charge the charger immediatly shows green and does not charge

Please can somebody help me Hoe to wirie this properly hopefully nothing broke

![image|281x500](upload://k2wYoRUC6y5Rf1bOziAOPzIr1mg.jpeg)![image|281x500](upload://uTAxZuALKupPjVNiWnTzQx3dkfm.jpeg)![image|281x500](upload://hA1GJjg2YFxyVJ6dzCFCrV1CyNK.jpeg)
```

---
## \#2 Posted by: Acido Posted at: 2018-04-13T22:02:40.978Z Reads: 97

```
I guess you have that ebay charger for 10$, 2a?
Small black brick?
On that green is not charging/full, red is charging also you need to turn on the board (bms) to charge
Also a drawing of your wiring would be helpfull
```

---
## \#3 Posted by: Pingo03 Posted at: 2018-04-13T22:29:41.967Z Reads: 92

```
My charger is a 10A and does show red while charginging and green when full

Here is an (ugly) drawing of the actual wiring

![image|375x500](upload://nMLwnqRYmNuzfBRm9QW4cfGLKof.jpeg)
```

---

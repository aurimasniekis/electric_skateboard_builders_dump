# Problem with Flipsky Dual 4.20

### Replies: 5 Views: 163

## \#1 Posted by: Oibu Posted at: 2019-08-09T17:53:24.448Z Reads: 48

```
Hi, I'm trying to configure my Dual VESC but as a complete noob I'm having some troubles: 
Whenever I complete the motor setup my motors spins weirdly even after the remote calibration. 


**Video here** : https://www.youtube.com/watch?v=yZyje_wKsf0
I've contacted Flipsky they are really trying to help and told me to use a more stable version (older) of VESC Tool 
I did it but I still have the same problem. My last hope is VESC Tool 1.09 I guess, or maybe I'm doing something wrong... 
I've noticed that I cannot change the firmware version of my main vesc at all, but I can do it on the second VESC, I don't know what to do. 
Any help would be highly appreciated. Thanks!
```

---
## \#2 Posted by: a13xr3 Posted at: 2019-08-09T20:33:40.310Z Reads: 42

```
First guess, are these unsensored motors? If so it's likely unable to orient the current start in order to begin the motor spinning. This is why unsensored boards typically say to kick start.
```

---
## \#3 Posted by: Oibu Posted at: 2019-08-10T07:22:12.650Z Reads: 29

```
Thanks for your response ! Yes they are unsensored ! So I just need to push the board to start and it will work ?
```

---
## \#4 Posted by: visnu777 Posted at: 2019-08-10T07:41:34.632Z Reads: 26

```
The motor assistant worked as it should? Detection is usually a sequence of a loud, MRI-like noise, some spinning and some slow turning. Unsensored motors don't need a kickpush on the bench ;)
```

---
## \#5 Posted by: Oibu Posted at: 2019-08-10T07:54:23.316Z Reads: 23

```
Yes it did and motors spin was very smooth during it
```

---

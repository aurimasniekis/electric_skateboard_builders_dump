# How connect Focbox Unity to Arduino by UART?

### Replies: 6 Views: 175

## \#1 Posted by: auveele Posted at: 2019-09-05T09:16:06.131Z Reads: 54

```
Hi forum!

I was trying to connect the focbox unity to the arduino by uart.
I wanna control the light and breaklight when the esk8 is breaking.

I check two libraries, but I can not connect to the focbox correctly.
https://github.com/SolidGeek/VescUart
https://github.com/RollingGecko/VescUartControl

Please, has anyone managed to connect the controller with arduino?
```

---
## \#2 Posted by: visnu777 Posted at: 2019-09-05T09:35:18.612Z Reads: 51

```
I think the Unity is the problem, they changed the original VESC Firmware quite a bit which might break compatibility with those libraries. Actually I did the same thing yesterday :D 
https://forum./t/grunstern-mov-e-shortboard-12s3p-nese-hummie-hubs-hammock-baseplates/2409/153
But with a FSESC 6.6 dual which is a "classic" VESC.
```

---
## \#3 Posted by: auveele Posted at: 2019-09-05T10:06:57.970Z Reads: 46

```
Jop!

I will try your code this afternoon, but if is a classic VESC, I think that the problem will persist.
I found another library for Focbox. I will try it too.

https://github.com/StefanMeGit/VescUartUnity
```

---
## \#4 Posted by: auveele Posted at: 2019-09-05T11:58:59.965Z Reads: 42

```
I can't undestand that if they modify the firmware of vesc, dont create a library or something to use the UART port. I think that without that this port in a little bit unuseful.

What is then its purpose? Only bluetooth controller?
```

---
## \#5 Posted by: visnu777 Posted at: 2019-09-05T12:36:30.767Z Reads: 38

```
Mhh, Stefans version is a fork of solidgeeks library where the PPM stuff is missing, but it should be easily doable to apply Stefans changes to @Pimousse fork :D I have no unity and therefore no need ;)
When you do please share it again so someone can easily do this in the future. Its quite easy with the normal VESC.
```

---
## \#6 Posted by: auveele Posted at: 2019-09-05T14:03:59.182Z Reads: 34

```
Yeah!

I was looking the structure of received data...

If I succeed, of course, I will publish the git.
```

---

# Will these batteries blow up my VESC?

### Replies: 5 Views: 243

## \#1 Posted by: dino15309 Posted at: 2018-06-29T22:20:47.661Z Reads: 84

```
So I am getting ready to buy everything for a build, (I might make a post about it) and I have found a great deal on some SUPER powerful LiPOs. They are rated for up to 200a discharge and 15c charge. I was going to put 8 of them in series for an 8s 1p 8000mah batery to drive 2 200kv racestar motors. They will be charged with a bypass bms at 2 amps (nothing fast or special). Anyway, will the high current blow up my VESCs? I am using these batteries: [https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F183036786061](https://rover.ebay.com/rover/0/0/0?mpre=https%3A%2F%2Fwww.ebay.com%2Fulk%2Fitm%2F183036786061)

Thanks!!
```

---
## \#2 Posted by: E1Allen Posted at: 2018-06-30T02:09:01.104Z Reads: 56

```
No, VESC are customizable.  You can limit current to whatever you want.
```

---
## \#3 Posted by: wafflejock Posted at: 2018-06-30T02:35:33.314Z Reads: 54

```
Max capacity for discharge is just that, an advertised maximum you can let flow before damaging the batteries.  The vesc is limited to about 12S in terms of voltage because of the components it uses but as previous post says you can limit max current the vesc will allow to flow to keep the vesc, motor, and batteries in safe limits.  Look up how to configure these things and spend time setting up/configuring the vesc before attempting to drive the motor at all.
```

---
## \#4 Posted by: dino15309 Posted at: 2018-06-30T03:08:43.417Z Reads: 36

```
Thank you Guys! This is only my second build and have self taught myself about batteries and all that. I thought what @wafflejock said about advertised maximum was the case, but I didn't want to assume and have some expensive parts fail.

Also, if you don't mind, do you think that 8s is enough to power 2 200kv motors?
```

---
## \#5 Posted by: E1Allen Posted at: 2018-06-30T03:11:52.359Z Reads: 31

```
Sounds good enough.
```

---

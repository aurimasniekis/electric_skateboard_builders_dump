# One last attempt at a BMS

### Replies: 13 Views: 274

## \#1 Posted by: TiMMaTTie Posted at: 2018-10-22T10:23:13.953Z Reads: 123

```
Hi guys,

I am trying to add a BMS to my two 4s lipo setup. I am using a cheap BMS to bypass for charge only, P- on my BMS is not connected. Links are below. I am measuring 4 untill 32 volts from b1 to b8, and 32.8v at the charger when unplugged. The problem I have is that the charger LED remains green, indicating it is not charging. Does anybody have any ideas? I am really close to removing the BMS and attaching my enclosure using clevis pins so I can more easily charge with a regular balance charger :)

[https://hobbyking.com/nl_nl/8s-li-ion-pcm-charge-4a-discharge-10a.html](https://hobbyking.com/nl_nl/8s-li-ion-pcm-charge-4a-discharge-10a.html)
[https://www.banggood.com/33_6V-2A-Smart-Battery-Charger-For-8S-28_8V-29_6V-Li-ion-Li-Po-Battery-p-1111782.html?cur_warehouse=CN](https://www.banggood.com/33_6V-2A-Smart-Battery-Charger-For-8S-28_8V-29_6V-Li-ion-Li-Po-Battery-p-1111782.html?cur_warehouse=CN)
![plaatje|543x500](upload://hLhEBbQcIiOqlunSUsoFbUVrJ77.jpeg)
```

---
## \#2 Posted by: pat.speed Posted at: 2018-10-22T10:41:51.016Z Reads: 92

```
Check the balance of the cells and make sure they are all similar. Also check connections and maybe even the charger plug.

Finally have you charged the battery up until this point or is this the first time you have plugged it into charge? You might be able to also try discharging it a bit and try again to rule out the charger output voltage being a bit low
```

---
## \#3 Posted by: Andy87 Posted at: 2018-10-22T10:47:59.415Z Reads: 86

```
did you check if you can charge your packs without bms?
just to be sure everything is good with your charger and your cells.
```

---
## \#4 Posted by: TiMMaTTie Posted at: 2018-10-22T11:01:30.060Z Reads: 80

```
all between 4.00 and 4.01. Connections seem fine, I will try discharging the batteries a bit. The batteries have been charged and discharged before using a balance charger, first time using a bms and cc cv charger
```

---
## \#5 Posted by: TiMMaTTie Posted at: 2018-10-22T11:02:19.428Z Reads: 72

```
DO you mean connecting the charger negative directly to battery negative?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-10-22T11:06:29.276Z Reads: 60

```
Yep, he means connecting the main power wires of the battery to the charger, this is a good method to rule out the bms
```

---
## \#7 Posted by: Andy87 Posted at: 2018-10-22T11:14:16.132Z Reads: 55

```
just hook your charger up to the pack without bms and look if the charger turns red and start charging.
```

---
## \#8 Posted by: TiMMaTTie Posted at: 2018-10-22T11:17:07.752Z Reads: 51

```
Thanks guys, will try
```

---
## \#9 Posted by: Namasaki Posted at: 2018-10-22T11:59:36.848Z Reads: 46

```
What charger are you using?
Did you check the output voltage of your charger while charging?
```

---
## \#10 Posted by: Andy87 Posted at: 2018-10-22T12:02:03.586Z Reads: 45

```
Link of the charger in the description 😉
```

---
## \#11 Posted by: Namasaki Posted at: 2018-10-22T15:08:25.871Z Reads: 30

```
The link is just giving me a blank page
```

---
## \#12 Posted by: TiMMaTTie Posted at: 2018-10-22T15:45:25.597Z Reads: 25

```
Thanks for the help guys, I found the issue. The female dc charge connector seemed to work when I used the beep function of the multimeter (sorry, not an electrical engineer), but I didnt measure anything when the charger was connected. Is it possible that the connection wasn't very solid, some resistance occured and the charger wouldn't start? Anyway, I switched to xt-60 and it's working fine now. 

Thanks again for your effort!
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-22T16:10:19.888Z Reads: 22

```
Now link isn’t working for me too.
Just to complete, it was a 2a Laptop brick style charger.

@TiMMaTTie good that you found the issue 👌
```

---

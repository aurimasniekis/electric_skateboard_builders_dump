# Vesc shutting off after i turn it on

### Replies: 19 Views: 732

## \#1 Posted by: Zimbombe Posted at: 2018-04-07T15:10:37.122Z Reads: 85

```
So this will hopefully not be another  "how i burned my vesc" thread.

But i wired up my new setup and and everthing themed to work fine, i connected it and updated the firmware, used very moderate settings

Motor current Max 25A
Max Brake -25A

Battery current max 25 A
max regen 2,5A

V shutoff at around 20,4V

until the Vesc Tool wanted to detect my motor and after the first beep it shut off all of the sudden.

Now the Vesc shows the blue light for a second when  i turn it on and then shuts off.

this is my wiring diagramm: (ofc there are 3 motor wires)

![Wiring sheme|551x500](upload://bFJdnP38Uazi6XGniqVt5IuVm21.png)


To give you some background this is my old setup where i added a esk8.de Vesc with an anti spark switch.
I also changed the old battery setup to a spot weldet one, same batteries tho, still 6s samsung 30q´s.

http://www.electric-skateboard.builders/t/human-instrumentality-project-6s3p-single-racerstar-140kv-5065-custom-deck-battery-box-holder-fvt-120a-esc/32737/26

would really appreciate any help, thx.
```

---
## \#2 Posted by: scepterr Posted at: 2018-04-07T15:18:56.831Z Reads: 78

```
Your vesc is wired to charge port negative? Not main battery negative?
```

---
## \#3 Posted by: Zimbombe Posted at: 2018-04-07T15:22:40.430Z Reads: 74

```
It´s wired to BMS C- and also Charging port - .

This BMS is different in some ways i think, anyway this is how it worked in my last setup.
```

---
## \#4 Posted by: scepterr Posted at: 2018-04-07T15:23:42.236Z Reads: 72

```
Negative on the vesc should be coming directly from battery if the bms is used for charging only
```

---
## \#5 Posted by: Zimbombe Posted at: 2018-04-07T15:25:17.133Z Reads: 70

```
This was the wiring of my old Setup which worked, as i said the BMS is kinda different.


![plan 3|690x261](upload://zUMtaWdgA8h5MlOLjRrfoJCk6q4.png)
```

---
## \#6 Posted by: scepterr Posted at: 2018-04-07T15:25:54.211Z Reads: 66

```
So you're using it for discharge?
```

---
## \#7 Posted by: Zimbombe Posted at: 2018-04-07T15:30:18.053Z Reads: 65

```
Both, yeah.
 ![1OXXXXXa0XXXXq6xXFXXX5|600x452](upload://oX1UWx0aTKKOn9Jcl7wz0WJxBrs.jpg)
```

---
## \#8 Posted by: scepterr Posted at: 2018-04-07T15:31:46.372Z Reads: 64

```
Seems like something is cooked on the bms then if it shuts off when the vesc tries to pull amps
```

---
## \#9 Posted by: Zimbombe Posted at: 2018-04-07T15:35:58.027Z Reads: 65

```
I thought about that too and you may probably be right, what would the vesc show if it broke ?
```

---
## \#10 Posted by: scepterr Posted at: 2018-04-07T15:38:30.989Z Reads: 61

```
Are you getting any errors or faults on the vesc?
```

---
## \#11 Posted by: Zimbombe Posted at: 2018-04-07T15:43:33.413Z Reads: 59

```
The only the it gives me is a short blue light, i´m not able to connect it via usb.
```

---
## \#12 Posted by: scepterr Posted at: 2018-04-07T15:45:18.786Z Reads: 59

```
Oh it doesn't stay on at all, I would inspect the vesc PCB, post some pics if you can
```

---
## \#13 Posted by: Zimbombe Posted at: 2018-04-07T16:58:51.297Z Reads: 51

```
![20180407_185536|281x500](upload://rf8eRHwyRBUXqTCg1CU6nbahTJG.jpg)![20180407_185531|281x500](upload://bxrY1TzXvV7WmKz1Fvgw14tzBFd.jpg)![20180407_185508|281x500](upload://96vvFuW48GYz7OrvAuo2nk77mG5.jpg)![20180407_185542|281x500](upload://zJaEWxELA4mbuBbEm19k8quQZys.jpg)
```

---
## \#14 Posted by: Orin635 Posted at: 2018-04-07T18:16:41.362Z Reads: 42

```
What BMS do you have?
```

---
## \#15 Posted by: Zimbombe Posted at: 2018-04-07T18:50:19.180Z Reads: 40

```
https://www.aliexpress.com/item/13S-100A-bms-2016-new-Li-ion-48V-100A-large-high-current-BMS-PCM-with-different/32759040792.html?spm=a2g0s.9042311.0.0.TLKPGu
```

---
## \#16 Posted by: Sebike Posted at: 2018-04-07T18:52:35.801Z Reads: 39

```
Is that a typo or did you set batt min to a positive value?
```

---
## \#17 Posted by: Zimbombe Posted at: 2018-04-07T19:00:16.302Z Reads: 38

```
![Unbenannt|665x499](upload://g6CVl3LRjWkQIi6EcLmz3UZUzla.png)

The

Absolute Maximum current Value was´nt there when in the Motor wizard, otherwise i would have set it down.
```

---
## \#18 Posted by: rich Posted at: 2018-04-07T19:08:41.740Z Reads: 37

```
[quote="Zimbombe, post:17, topic:51483"]
The Absolute Maximum current Value was´nt there when in the Motor wizard, otherwise i would have set it down.
[/quote]

It's not in the wizard because it should be 130A, that's default, if you set it lower you'll get faults..
You could increase Batt regen up to -12A with your 6s3p.
But this hints won't help if you can't connect to VESC-Tool :smirk:
```

---
## \#19 Posted by: Zimbombe Posted at: 2018-04-07T20:00:23.574Z Reads: 31

```
So the Bms should´nt be the problem because the Vesc get´s the full 24,5 V
```

---

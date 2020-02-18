# Max Volt for 6374 motor

### Replies: 17 Views: 512

## \#1 Posted by: Alex.Scheff Posted at: 2018-03-13T10:37:30.118Z Reads: 102

```
Hi,
I want to use [this](http://alienpowersystem.com/shop/brushless-motors/aps-6374s-sensored-outrunner-brushless-motor-200kv-3200w/) motor and it's just for a 10s battery but I want to use a 12s battery pack. If I just go up to 60Amps could it also work?
Motor with 3200W
50,2V(full charged 12s pack) × 60A (max Amps) = 3024W
Still under 3200W
Could this work or should I never go over 42V (full charged 10s pack)?

Thanks!

Alex
```

---
## \#2 Posted by: bimmer Posted at: 2018-03-13T10:54:09.732Z Reads: 94

```
What ESC are you using?
```

---
## \#3 Posted by: Alex.Scheff Posted at: 2018-03-13T11:03:05.749Z Reads: 86

```
Maytech vesc, 60V 50A  (dual setup so I use two)
```

---
## \#4 Posted by: bimmer Posted at: 2018-03-13T11:17:43.531Z Reads: 82

```
As far as I know maytech vesc's have the ERPM limit  of about 60.000 Erpm. 
Most motors have 7 Poles so you have to divide by 7 and get 8570 rpm.
The Motor has 200KV so 200RPM per V that equals 10.000 RPM at 12s (50V)
So at the top end you are pushing your Vesc to an area where they are prone to failure.

Its why I am selling 170KV 6374 Motors as they will not break most people's ESC's.
```

---
## \#5 Posted by: Alex.Scheff Posted at: 2018-03-13T11:20:10.255Z Reads: 72

```
Awesome thanks, so if I go with lower kv it might work?
```

---
## \#6 Posted by: bimmer Posted at: 2018-03-13T11:22:16.004Z Reads: 68

```
Yes anything over 170KV will over long kill your ESC at 12s.
```

---
## \#7 Posted by: Alex.Scheff Posted at: 2018-03-13T11:23:13.899Z Reads: 67

```
Okay thank you very much, I will look for a lower kv motor because I really want to go with a 12s.
```

---
## \#8 Posted by: Nordle Posted at: 2018-03-13T12:21:50.420Z Reads: 60

```
[quote="Alex.Scheff, post:7, topic:48962"]
I will look for a lower kv motor
[/quote]

[quote="bimmer, post:4, topic:48962"]
I am selling 170KV 6374 Motors
[/quote]

This is nuts:D
```

---
## \#9 Posted by: bimmer Posted at: 2018-03-13T12:30:43.947Z Reads: 50

```
how so?
10char
```

---
## \#10 Posted by: Nordle Posted at: 2018-03-13T12:41:16.344Z Reads: 49

```
I just like that kind of conversation. I'm no native english speaker, i ment its awesome not crazy:)
Sometimes you don't see the forest because there are to many trees. I just want him to buy your motors:D
```

---
## \#11 Posted by: bimmer Posted at: 2018-03-13T12:46:15.030Z Reads: 46

```
By the idiom you used I am assuming you are German or Austrian.
```

---
## \#12 Posted by: Nordle Posted at: 2018-03-13T12:57:06.424Z Reads: 41

```
I'm italian, but we speak german here;)
```

---
## \#13 Posted by: Alex.Scheff Posted at: 2018-03-13T12:59:12.625Z Reads: 38

```
Guter Mann
```

---
## \#14 Posted by: Nordle Posted at: 2018-03-13T13:03:18.120Z Reads: 37

```
You speak german too, bimmer is probably out of range^^ 
I can recommend APS, has almost every kv you want or can order them for you, also his motors come with sensors if desired and all i got have silicon wires.
```

---
## \#15 Posted by: bimmer Posted at: 2018-03-13T13:04:08.629Z Reads: 38

```
I took my 1200gs through the Dolomites in 2013. Pretty sure that should be close to you.
```

---
## \#16 Posted by: Nordle Posted at: 2018-03-13T13:08:43.343Z Reads: 37

```
Indeed, i'm right there.
![IMG_0820|690x245](upload://1PyM020pHcB2dJ2anNNEu1yFRv5.JPG)
```

---
## \#17 Posted by: bimmer Posted at: 2018-03-13T13:23:28.965Z Reads: 33

```
Btw.

With DHL and a small reduction in price my motors are the same price as APS while being plug an play for vescs. Sensor is already 2mm micro jst and at 200mm better suited.
```

---

# Breaker switch discharged one of my cells?

### Replies: 13 Views: 1338

## \#1 Posted by: arfintr Posted at: 2016-08-08T05:24:47.794Z Reads: 67

```
My breaker has the one input and one output, so I read online that I need to hook just the live wire up to the breaker - I did that and one of my lipo cells out of the 8 now sits at 1.2 volts after sitting for a day hooked up to the off position switch.... Does the breaker have a polarity for the switch like a diode or something? Was I supposed to hook it on the black wire instead? I am guessing since real current flows from Black to Red (->+) that the electrons actually somehow drained through the black wire that did not have a switch.. welp I am down a cell and will probably have to do some lipo surgery. Thoughts?
```

---
## \#2 Posted by: barajabali Posted at: 2016-08-08T05:28:58.058Z Reads: 64

```
Link the breaker you used please
```

---
## \#3 Posted by: Tarzan Posted at: 2016-08-08T05:31:27.603Z Reads: 66

```
Did you use a lipo alert?
Usually they drain just one cell.
```

---
## \#4 Posted by: arfintr Posted at: 2016-08-08T05:33:38.934Z Reads: 62

```
http://www.jaycar.com.au/100a-circuit-breaker/p/SF2266 Here it is - seems the same as any other, Jaycar is a big electronics store too so I don't think the breaker is untrustworthy
```

---
## \#5 Posted by: arfintr Posted at: 2016-08-08T05:34:51.683Z Reads: 58

```
Yeah, the one cell is drained - is this normal? My esc sputtered out because it knows the cell is below minimum voltage and my charger will not charge through balance connector because it is below the minimum 3.3 volts.
```

---
## \#6 Posted by: Tarzan Posted at: 2016-08-08T05:37:40.702Z Reads: 56

```
You have to diconnect the alerts while not riding. The power to operate these things is taken from one cell and in the end on cell is fucked up.
Sorry to say that, but your lipo is dead.
```

---
## \#7 Posted by: arfintr Posted at: 2016-08-08T05:43:58.431Z Reads: 55

```
Oh I realized my miscommunication - I don't use an alert. The Lipo was connected like so - the red from Lipo through the breaker to the red on ESC and on the black connected straight from battery to the ESC. When the Breaker was off the esc was off so I thought that the circuit was incomplete and that would be an effective switch? It seems not to be the case.. Do I need my breaker switch set on the black wire instead? That is all I wish to clarify since I want a switch instead of plugging and unplugging the battery.

As for the Lipo there is not much I can do for it other than remove the cell and chuck it.
```

---
## \#8 Posted by: Tarzan Posted at: 2016-08-08T05:49:01.505Z Reads: 49

```
From my understanding you did it correct!
I don't know why one cell is discharged that deep.
Your balance leads where unplugged too?
```

---
## \#9 Posted by: arfintr Posted at: 2016-08-08T05:55:31.297Z Reads: 51

```
Balance unplugged as well I am running 2 4S in series and the last cell on one of the 4s closest to the negative is dead - I noticed the slight discharge lower than the other cells a day after I got the breaker running however it didn't dip below the 3.3V and I passed it as some kind of random quirk.. I left it for an entire day with the breaker off and it seems to have done the damage now. Perhaps I need to do some testing to check if the cell itself hasn't gone bad coincidentally, maybe a sacrificial lipo to check for drain in the last cell? Cross my fingers it was just the bad lipo.
```

---
## \#10 Posted by: arfintr Posted at: 2016-08-08T06:00:06.908Z Reads: 48

```
Update with a multimeter - when the switch is disengaged there is definitely no circuit made with the positive terminal of the battery at all, if there is any current leaking it has to be somewhere on the esc.
```

---
## \#11 Posted by: barajabali Posted at: 2016-08-08T06:04:01.738Z Reads: 48

```
You can revive that cell just charge it individually at as low amp as you can .1 or .2 amp. And it'll jump right back up to 3.7 volts. Don't charge fast because internal resistance is really high when the voltage dips down that low so low amps=cooler charging 

As I understand it
```

---
## \#12 Posted by: arfintr Posted at: 2016-08-08T06:12:15.915Z Reads: 47

```
Interesting - that seems to be a pretty common fix from a quick google search - cheers. I will update in a couple days if my test reaches any worthwhile conclusion.
```

---
## \#13 Posted by: arfintr Posted at: 2016-08-10T11:13:00.392Z Reads: 22

```
Update: The cell is revived and functioning great - breaker switch has been working fine the past two days with the batteries plugged in, no cells are further damaged. I'm wondering what could have caused the voltage drop in the cell a couple days ago but at this point I am just happy the problem is gone, cheers for the help!
```

---

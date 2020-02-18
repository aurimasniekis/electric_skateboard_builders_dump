# Vedder Anti-Spark broken / Switch without Function?

### Replies: 12 Views: 1170

## \#1 Posted by: kampfhahn Posted at: 2016-07-15T19:42:45.473Z Reads: 151

```
Got my Vedder Anti-Spark today and wanted to test it without plugging an esc on.

So i just connected a 20 V Power Supply to the IN-Connectors of the AS and my multimeter to the OUT-Connetors and measured exactly the 20V there. Fine.

But: The voltage is at the OUT-Connectors regardless if the Switch of the Anti-Spark is set to on or off?! Does anyone have an explanation for this behavior?
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-07-16T22:24:38.646Z Reads: 132

```
Maybe you can provide some pictures of your Vedder Anti-Spark switch. Without pictures there could be endless possibilites for the failure...
```

---
## \#3 Posted by: mason Posted at: 2016-07-16T22:28:38.568Z Reads: 129

```
you might have gotten one with the bad mosfet batch.
```

---
## \#4 Posted by: Nordle Posted at: 2016-07-16T22:28:52.033Z Reads: 128

```
Your fet could be damaged, it's one of their characteristics to be always switched on if they are _(damaged^^)_.
```

---
## \#5 Posted by: kampfhahn Posted at: 2016-07-17T13:44:58.912Z Reads: 107

```
I now put everything together and the switch works fine. Maybe the behavior i talked about in post 1 is normal when no ESC and motor is plugged in.
```

---
## \#6 Posted by: Nordle Posted at: 2016-07-17T13:48:27.984Z Reads: 105

```
No it isn't.
 ~edit~ indeed it is!
```

---
## \#7 Posted by: kampfhahn Posted at: 2016-07-17T14:06:43.393Z Reads: 101

```
Hm kay. But why does it work anyway when everything is put together?
```

---
## \#8 Posted by: ikjahaa Posted at: 2016-07-17T14:15:57.983Z Reads: 97

```
Is it possible your multimeter closed the circuit?
So the 20V bypassed your switch, by flowing through the multimeter ?
```

---
## \#9 Posted by: Nordle Posted at: 2016-07-17T14:19:26.385Z Reads: 97

```
I remember something similar happend to me when i built this circuit. If i switched it of and measured voltage it was still high. But if i connect any kind of load (voltmeter already was enough) voltage drops slowly (depends on the load) to zero. Now with a esc connected there is a small load.
I assume its because the cap in the circuit must be discharged before it turns the mosfet off.
```

---
## \#10 Posted by: kampfhahn Posted at: 2016-07-17T14:25:56.140Z Reads: 98

```
Sounds reasonable. So no need to return the AS. I'll test it with a LED or something else when i'm back in the workshop.
```

---
## \#11 Posted by: Nordle Posted at: 2016-07-17T14:35:04.324Z Reads: 96

```
Take a resistor, or do you have ''e-skate rated voltage'' LED's?^^
```

---
## \#12 Posted by: kampfhahn Posted at: 2016-07-17T14:39:55.617Z Reads: 95

```
Of course :) Got a 12V power supply and a 470 ohms resistor. No need to use the skate voltages, i just want to confirm the theory with the cap that has to unload first.
```

---

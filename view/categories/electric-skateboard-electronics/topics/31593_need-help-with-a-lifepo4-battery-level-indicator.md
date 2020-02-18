# Need help with a LiFePo4 battery level indicator

### Replies: 5 Views: 632

## \#1 Posted by: Johnonon Posted at: 2017-08-27T20:28:12.437Z Reads: 58

```
Hi everyone, 

Recently I finished building my board, and quickly realised that my LiFePo4 battery is showing wrong battery level, after doing a little bit of research I finally knew why my indicator was acting like that. It's because LiFePo4 batteries have a very flat discharge curve so my indicator will be showing nominal voltage 90% of the time. I am using a 12S1P A123 battery pack and a custom made level indicator made out of zener diodes (made a similar indicator for my other board and it works perfectly, so it's not my indicator's problem). Did anyone encountered a similar problem? What would be the most simple solution? Maybe it can be solved with a arduino?
```

---
## \#2 Posted by: pakue Posted at: 2017-08-27T20:42:51.428Z Reads: 53

```
Can you increase the sensitivity of your indicator so it can show the small voltage changes?
Another option would be to get a premade LiFePo4 fuel gauge like these http://www.szgrn.com/battery-gauge.html.
```

---
## \#3 Posted by: Johnonon Posted at: 2017-08-27T21:56:45.274Z Reads: 42

```
I was thinking about increasing sensitivity, but since my zener diodes are 2v apart it would be difficult to do such thing, and my local electronic shop only have those zener values that I am using right now, that's why I am considering using arduino, but I have never used one, so I don't know if it's possible at all. I was thinking about getting a premade indicator, same as your link, but these chinese indicators does not look as good as selfmade :slight_smile:
```

---
## \#4 Posted by: pakue Posted at: 2017-08-27T22:25:19.958Z Reads: 34

```
I'm guessing you use zener diodes to turn on LEDs in sequence? A comparator and a voltage reference would also work for this. The advantage would be that you could set the value to whatever you want.
```

---
## \#5 Posted by: Johnonon Posted at: 2017-08-28T06:03:31.516Z Reads: 21

```
Hmm very interesting idea, I never thought about using a comparator, I will definitely look more into, thanks
```

---

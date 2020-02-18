# Arduino Voltmeter

### Replies: 7 Views: 698

## \#1 Posted by: IsTalo Posted at: 2017-02-22T19:28:49.890Z Reads: 79

```
HI Guys, I bought a lot of things for my skate but forgot the [Voltmeter](http://alienpowersystem.com/shop/batteries/6s-batteries/6s-battery-gauge-board-copy/) and I want to make one now with a Arduino, I don't found anything about it on the forum and I want help of you, How Would I do It? I could be a [Voltmeter Like This One](http://alienpowersystem.com/shop/e-board-kits/battery-indicator-display/) too
```

---
## \#2 Posted by: Pantologist Posted at: 2017-02-22T19:53:27.602Z Reads: 77

```
There is very little point by using an Arduino. You'll have to use a voltage divider. The Arduino can only read up to 5v on its pins.
```

---
## \#3 Posted by: IsTalo Posted at: 2017-02-22T20:05:02.862Z Reads: 71

```
Yeah, but there are Voltage Modules for arduino that reads to 25v, a 6s battery have it
```

---
## \#4 Posted by: emepror Posted at: 2017-02-22T20:21:41.101Z Reads: 65

```
you could use something like one of these: https://www.sparkfun.com/categories/151
```

---
## \#5 Posted by: IsTalo Posted at: 2017-02-22T20:32:48.006Z Reads: 59

```
Yes, but it support the Current?
```

---
## \#6 Posted by: emepror Posted at: 2017-02-22T20:34:46.554Z Reads: 55

```
id go with the 90A or 180A choice, 90A should be fine for a 6S setup I think. Single motor?
```

---
## \#7 Posted by: IsTalo Posted at: 2017-02-22T20:47:00.466Z Reads: 48

```
Yeah, I think so, If u use vesc you can change your battery current to lower than 80a
```

---

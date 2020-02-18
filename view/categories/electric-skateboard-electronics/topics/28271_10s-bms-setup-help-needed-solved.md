# 10S BMS Setup &#124; Help needed! \[SOLVED\]

### Replies: 7 Views: 727

## \#1 Posted by: patrickgoeler Posted at: 2017-07-22T10:34:06.400Z Reads: 107

```
Hey guys, 
I have spent quite some time digging through every important post of this forum and this resulted in my setup below. I would love some feedback on whether everything is connected as it should be.

I am asking because I fried a 42V Charger when trying to charge the batteries. The XT90 Loop Key was not connected. There was a spark in the charging port and then the charger was dead.
At the moment I cannot figure out what I did wrong and I am afraid to just try again and fry another one.

Thanks for the help :slight_smile:
<img src="/uploads/db1493/original/3X/7/2/72f7d1bc52bfd09d7627e054fca5f556d63fcafe.jpg" width="375" height="499">
```

---
## \#2 Posted by: trancejunkiexxl Posted at: 2017-07-22T14:56:44.420Z Reads: 86

```
nice pic dude! im sorry to hear about your electrical issue but im very interested in hearing your progress.. i recently fried a 50.7 charger myself.. ya they 40$ each it sucks! I would wait for some of the electrical crew to see your post can you share more info about your lipos and charger setup?
```

---
## \#3 Posted by: MysticalDork Posted at: 2017-07-23T05:34:56.559Z Reads: 75

```
I'd check the polarity of your socket. The drawing looks correct, so assuming the actual setup is wired the same way, the only real possibility is that the charging plug was wired backwards and the charger got a blast of -36v which fried it. Some of these chargers have a fuse, you may want to check and see if it has one, and check if it's blown.
```

---
## \#4 Posted by: Namasaki Posted at: 2017-07-23T06:48:36.389Z Reads: 68

```
Mixed polarity of the charge port and charger plug would be my guess as well.
```

---
## \#5 Posted by: patrickgoeler Posted at: 2017-07-23T09:11:46.864Z Reads: 62

```
@trancejunkiexxl Sure! I am going with a 10S 5A Lipo BMS Setup (5x 2S from Turnigy), the FOCBOX from Enertion and a Turnigy Motor (213kv). I build the board myself with plywood and more parts from Enertion. The biggest challenge will be the motor mount atm, not sure how I will build that yet.. As a remote I will (or at least try to) use this Wii Nunchuck: https://www.amazon.de/gp/product/B001WYAB5W/ref=oh_aui_detailpage_o01_s00?ie=UTF8&psc=1 I havent gotten to try it out yet, because I wanted to resolve any electrical issues before connecting the VESC.

@MysticalDork @Namasaki Thanks for the input guys! :slight_smile: I will make sure the polarity is right the next time and keep you posted as soon as the new charger arrives.
```

---
## \#6 Posted by: patrickgoeler Posted at: 2017-07-23T12:19:25.504Z Reads: 56

```
<img src="/uploads/db1493/original/3X/c/2/c295e2750f41aa2bee3bff0f5ffb28b4b37227b9.jpg" width="666" height="499">

So it turns out if I were to plug in the charger right now the Plus-labeled pin would connect with the Minus-labeled charger hole, which is not correct, right?

So you guys were right, thank you so much @Namasaki @MysticalDork
```

---
## \#7 Posted by: trancejunkiexxl Posted at: 2017-07-23T14:33:35.302Z Reads: 48

```
congrats on finding the problem!!!
```

---

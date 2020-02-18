# Strange ESC sound when it&rsquo;s on

### Replies: 5 Views: 445

## \#1 Posted by: ctincristy Posted at: 2019-01-04T06:46:53.433Z Reads: 54

```
Hey there. I'm using the usual cheap Chinese hubs from my 1 year old wowgo 2 paired with an ownboard ESC. It's the first time using the new esc and only now did I notice this strange subtle sound  similar to how gas sounds when you turn on a stove. I am also running it sensorless because I have problem with the sensors, still is very smooth and strong. I get the same noise even when I plug in the sensor cables. I never really listened to my old esc because it was inside the metal case. Now I'm laser cutting a smaller enclosure and I'm paying attention to all the details. Here is also a link to my reddit post where I have a video containing the sound.
![20190104_013901|666x500](upload://u7SVzBkiNclm8pWPhuWNTf3xpDr.jpeg)  
https://www.reddit.com/r/ElectricSkateboarding/comments/acfpmw/esc_noise_when_turned_on/
Also, the XT60 conector doesn't fit all the way in and I'm holding it with rubber bands.
1) is it ok if I hear that sound?
2) is it ok to have an MDF (wood resin and glue) enclosure for the ESC?
3) eventually how to make the enclosure not ugly or at least water tight. Thinking of putting a transparent lid to show off its ugliness and lots of hot glue
```

---
## \#2 Posted by: goldrabe Posted at: 2019-01-04T07:28:40.303Z Reads: 41

```
The humming sound is normal it's called coil whining. Bad laptops suffer from this too. 
It's fine to run the ESC without sensors plugged.
```

---
## \#3 Posted by: linsus Posted at: 2019-01-04T12:43:40.300Z Reads: 34

```
that XT connector.. Be real careful. if its the one with a small resistor for antispark feature, then the first 5mm connects thru the resistor in the antispark and not cable->plated connector-cable. Can create magic smoke and melt the connector if you run load through the resistor. (I've done this while beeing lazy when bench testing)

Try to get a pair that fits properly.
```

---
## \#4 Posted by: ctincristy Posted at: 2019-01-09T04:59:08.948Z Reads: 21

```
well that's what actually happened because of the old ESC. I plugged it in the battery while the motors were unplugged. magic smoke appears, inside of connector gets melted. For now I just shaved off some of the excess, enough to have a significant contact between the connectors until a replacement comes. It worked well the 5 days I've been testing it. You suggest buying a good cable? Or just replace the connector. I did the thing I wrote above many times before, this was the first time it happened
```

---
## \#5 Posted by: linsus Posted at: 2019-01-09T07:58:27.614Z Reads: 19

```
Might not fail the first time, if the connector isnt pushed all the way in, chance are you're running current through resistor/too small contact patch in the connector. Thats why it melted. 12-8 AWG should be fine regarding the cable. looks like u got a phat one in the pic. Just get two connectors that fit properly
```

---

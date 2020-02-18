# Random short burst braking while driving

### Replies: 10 Views: 134

## \#1 Posted by: Marksmoura Posted at: 2019-04-16T14:54:44.591Z Reads: 61

```
Hello guys my skateboard sometimes randomly brakes for a very short time.
I am using two vesc 4.12 with split ppm. The receiver wires are short and the receiver is next to the battery instead of being next to the vesc or motor wires. 

It seems like a short pulse half a second.
This only happens if I accelerate or when I hit the brakes but this is totally random and I can't replicate. 

Sometimes I accelerate and the motor brake hard for like 500ms or less and almost throws me out of balance.

If I brake just slight it happens some times just a slightly hard slow down and sometimes a really hard brake for a very short time so I never fall to this. 

I rebind the remote but I am not sure if it is the remote because I test unpluging it while accelerating, I take the sensor cables out and this doesn't happen. My fail safe is set to iddle. 

It could be a short but I open the motor and didn't really found anything. I was running firmware 2.16 and now I am using ackmaniac 2.54 moded for the modded blc.

My last resource now is to connect a Bluetooth to the best and drive it while using the android app to see what happens here. 

Does someone have some insight about what it can be?
I have some heattubes on the bullet connects a little extra tube so when I plug the males they get covered by the heatsink and I found out sometimes one of the fases the heatsink shrinked like the bullet connector got hot or something.
```

---
## \#2 Posted by: skatardude10 Posted at: 2019-04-16T15:15:33.950Z Reads: 50

```
Do you have PPM smoothing turned on for both vescs? It's called median filter or something like that under APP/PPM.
```

---
## \#3 Posted by: rusins Posted at: 2019-04-16T15:24:19.137Z Reads: 46

```
Hmm a short between your phase wires could definitely cause a sudden breaking + heat up the bullet connectors. Could you take some pictures of your board and the internals? Maybe someone will spot something wrong :man_shrugging:
```

---
## \#4 Posted by: ZachTetra Posted at: 2019-04-16T15:26:24.463Z Reads: 47

```
Maybe the bullet connection in shrink wrap if you can see some metal showing and possibly take a look at the ESC and motor windings for signs of damage
```

---
## \#5 Posted by: Jinra Posted at: 2019-04-16T15:30:21.997Z Reads: 46

```
Get it to happen again and before restarting or turning off the board, connect to the vesc and check for faults
```

---
## \#6 Posted by: Marksmoura Posted at: 2019-04-16T16:10:36.486Z Reads: 34

```
I tried to connect to the vesc and check for faults but for some reason the com port doesn't show up until I turn off the board and turn it back on.

The smoothing I have enable.
The white and yellow cables you see are the USB cables because the connector was broken so I just welded 3 wires. Ground and signals. 
The receiver I used super glue so it doesn't move around and the plug on the receiver also has some glue so it doesn't unplug while riding 

![15554311299305245693582032179612|375x500](upload://eQ1pclaL0HXFMmKu65dLO1K1ga3.jpeg) 

![15554311730003108592642531286750|375x500](upload://uPOY1ITYnOMyp35C1HUDkIN8xyF.jpeg)
```

---
## \#7 Posted by: Jinra Posted at: 2019-04-16T16:15:00.350Z Reads: 28

```
Man those vescs have seen better days. I had an issue before where my VESC wouldn't connect after erroring (small braking like you). It ended up being a slow burn DRV failure. It didn't completely fail until a month or so later.

I'd probably replace the vesc..
```

---
## \#8 Posted by: Marksmoura Posted at: 2019-04-16T16:19:43.661Z Reads: 27

```
I didn't ride more than 70km with them. 
They were new.
They came with just 2 capacitors so I am not sure exactly if I should add more capacitors. The wires are relatively short. 

It looks a mess because I welded most of the wires instead of plugging as I was afraid it could be a contact problem. Now I must make sure which one exactly has the problem. 

If I disconnect one motor can I safely ride while the 2nd vesc being connected?
```

---
## \#9 Posted by: Jinra Posted at: 2019-04-16T16:23:42.956Z Reads: 22

```
I was mainly saying that since one of the coils seems to have a piece missing on it. I think my 4.12's had 3 63v 680 uF capactiors. If you have at least 2040uF per VESC you should be okay on the capacitors, if not, you may want to add more. Those also look like cheaper Vescs, which tend to fail.
```

---
## \#10 Posted by: Marksmoura Posted at: 2019-04-16T16:59:25.693Z Reads: 17

```
Since im working in China at the moment I just bought two more. The broken one when I find which I will scrap it and the 2nd I leave it for parts or as a replace.

This are also cheap but don't seem to have missing parts like this two I already have where can chip is missing and so on. 

For 60eur I get two and I should get them maybe until next Sunday :smiley:

![Screenshot_20190417_005607|447x500](upload://8oKPhbbeJZk824Wm4hRgb1yrtQY.jpeg)   

About the caps I will get some more and try to fit them there.
```

---

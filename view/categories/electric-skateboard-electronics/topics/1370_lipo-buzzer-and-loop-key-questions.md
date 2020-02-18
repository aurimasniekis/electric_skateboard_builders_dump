# Lipo Buzzer and Loop Key Questions

### Replies: 8 Views: 1895

## \#1 Posted by: paragon Posted at: 2016-02-15T03:02:00.177Z Reads: 115

```
<img src='/uploads/db1493/original/2X/d/d0106f12906b16e2cdff413a3acc072ac9ee44cf.jpg'>
Hello, I, like many others use one of these cheap buzzers to monitor my lipos while I ride. I was wondering if it would be possible to add a switch to this, so that I could keep it connected at all times.

Also, for a loop key like the one below, why is it that the side with the exposed bullet connectors (female connector) is attached to the board? Isn't this a safety hazard if someone were to put their finger there and connect the circuit? Feeling 20v or more doesn't seem healthy.
http://www.electric-skateboard.builders/uploads/db1493/original/1X/a5a2c96986fc0c6a7c5233555124f7121f732895.jpg
```

---
## \#2 Posted by: Kaly Posted at: 2016-02-15T03:30:07.313Z Reads: 116

```
For the Lipo saver you will need to attaché and extra jxt terminal to conect the Lipo saver and still have a balance port for your charger, after this just need to solder a on/off switch in the negative cable of the jxt terminal that the Lipo saver is conected. 

On/off switch here 
http://m.ebay.com/itm/2Pcs-Red-Self-Lock-ON-OFF-lock-Mini-Push-Button-Switch-/181758607370?txnId=1453814461008

Jxt extension 
http://m.ebay.com/itm/10-PCS-6S1P-Balance-Charger-Silicon-Cable-Wire-JST-XH-Connector-Adapter-Plug-/231608533530?nav=SEARCH
```

---
## \#3 Posted by: laurnts Posted at: 2016-02-15T03:31:50.756Z Reads: 114

```
Then just add a switch for the voltmeter.

For the loopkey, well its easier to make the loopkey like this and not the other way around. Ofc you would like to add some protective tape / cover around it. Neverthless you can't get electrical shock with just touch bare positive / negative lead only as your body doesn't complete the circuit. (remember that loop key is only attached to positive / negative side only!)
```

---
## \#4 Posted by: Kaly Posted at: 2016-02-15T03:33:37.511Z Reads: 115

```
The xt-90 loop key is not an issue 20v you will not feel.
Like @laurnts said you won't complete the circuit.
```

---
## \#5 Posted by: cmatson Posted at: 2016-02-15T03:42:04.214Z Reads: 112

```
I wouldn't attach one of those standard lipo buzzers permanently because I'm pretty sure they just run off your first lipo cell. 

It's better to jut get a simple volt meter like I've added to my board here:<img src="/uploads/db1493/original/2X/3/387b766a20a8109ac84fbd2b28821693b493e272.jpg" width="690" height="388">

Also, the reason for the loop key is to have it more hidden within the enclosure. If you put the male end on your board, then it will either have to stick out from the enclosure, or be mounted perfectly to allow the other xt90 to slide over it without interfering with the enclosure.
```

---
## \#6 Posted by: Kaly Posted at: 2016-02-15T04:20:24.526Z Reads: 108

```
By installing a on/off switch the volt meter will not drain the battery while is off. 

The simple volt meter just give you a battery voltage and not a single cell voltage. 

Personally I like to know the state of all the cells in the pack this way you get to know your battery and keep an eye in its evolution.
```

---
## \#7 Posted by: lowGuido Posted at: 2016-02-15T04:32:18.288Z Reads: 102

```
You can switch the lipo alarm on the negative lead (first pin)
```

---
## \#8 Posted by: paragon Posted at: 2016-02-15T05:58:03.556Z Reads: 98

```
cool just wanted to be sure, normally people switch positive, but in this case switching negative makes sense.

Just to verify, fuses go on the positive power lead (connecting the battery to the esc) and a 60a fuse should be fine for a 6s board with a 1:5.5 reduction and 8in wheels?
```

---

# Possible to mod Boosted Board remote to use for DIY build?

### Replies: 12 Views: 2623

## \#1 Posted by: Airmacx Posted at: 2016-06-14T13:19:31.769Z Reads: 266

```
I really love the feel of the BB controller, despite what people say, I was just wondering can I possibly open it up and mod the inside with my own chip or something and use it to control my mono drive build. 

Possible, or impractical, or simply not possible?
```

---
## \#2 Posted by: fraannk Posted at: 2016-06-14T15:51:35.670Z Reads: 257

```
Following! :D Really love the look of it
```

---
## \#3 Posted by: lowGuido Posted at: 2016-06-14T16:34:50.570Z Reads: 251

```
I suppose it depends on what speed controller boosted use and how it gets its input from the receiver. 
anything is possible with the right electronics...
```

---
## \#4 Posted by: Nordle Posted at: 2016-06-14T16:51:16.693Z Reads: 246

```
If you can fit an arduino in it.
```

---
## \#5 Posted by: KMeyerson Posted at: 2016-06-14T22:35:58.272Z Reads: 219

```
Here are my thoughts on the subject,

Boosted boards use an encoder that doesn't measure the motor (thus saving space and making the motors cheaper), instead they measure the position of the belt as it turns the drive wheel. I don't know if this encoder is required for operation. 

Boosted board motors (see above for encoders) might have some degree of timing sensitivity with the encoders. You should try to match or exceed the boosted motors (not hard given that they're not actually very good motors as far as size and power go). If you can swap it out with your own thats a win!

Boosted boards are build with 12s1p batteries (do note that they use 26650 cells that cont. discharge at a max of 70Amps and peak around 130Amps).  I would not suggest using a battery pack that cannot match the stock discharge rate of 70Amps out of a fear of battery damage and meltdown. By increasing your parallel packs you can match discharge rates. For example, 12s3p 18650 cells with cont. discharges of 25Amps would provide you with a combined discharge rate of 75Amps.
```

---
## \#6 Posted by: Airmacx Posted at: 2016-06-15T00:13:32.951Z Reads: 207

```
Yeah ill try to get hold of one and open it up.
```

---
## \#7 Posted by: RunPlayBack Posted at: 2016-06-15T00:51:22.520Z Reads: 194

```
This is good info, but how does this pertain to the Boosted remote?
```

---
## \#8 Posted by: Airmacx Posted at: 2016-06-15T01:29:39.154Z Reads: 188

```
Yeah as @RunPlayBack said, how does this relate to the subject of me wanting to use the remote for my DIY build. I was planning on taking out the insides, and replacing it with my own parts, and just putting a receiver or something that connects the two in the board. Or is it more complicated than that?
```

---
## \#9 Posted by: Paulf Posted at: 2016-06-15T11:16:26.709Z Reads: 170

```
Has anyone got a picture of the inside of this remote ?
I think that this is definitely doable but we need to see what's inside this remote to go further...
```

---
## \#10 Posted by: Airmacx Posted at: 2016-06-15T12:25:16.772Z Reads: 164

```
If only I still had mine... I don't want to blow $150 to get a remote just to open it up and potentially not work. I'm gonna try look for second hand one.
```

---
## \#11 Posted by: KMeyerson Posted at: 2016-06-15T13:21:50.984Z Reads: 162

```
You used the word "controller" not remote.  Controller  refers to speed controller, not remote control.

Regardless, with their latest updates I doubt you'd be able to connect easilt via onboard Bluetooth. I'd suggest using bluesniff to identify the uetooth packets but they should all be encrypted now.  Instead you could also put a teensy with a NRF and use their buttons/switches.
```

---
## \#12 Posted by: Paulf Posted at: 2016-06-16T11:11:27.548Z Reads: 143

```
you'll definitely need to put some kind of micro controller in this remote 
I can't remember where but I'm sure I've seen somewhere that they have been working on encryption of the signals on their latests software upgrades...
```

---

# Confirm Wiring Diagram

### Replies: 4 Views: 159

## \#1 Posted by: bshin100 Posted at: 2019-07-24T22:22:13.511Z Reads: 49

```
I realize that there's a number of wiring configuration topics on here, and I've read a ton of them. From all those, I think I've figured out how to wire my setup, but I'd like to pass it by all of you just to confirm that I won't fry my components or light my house on fire.

![image|690x267](upload://hlz5YJlK8bluBtBlT1k3nnA9lqb.jpeg) 
My battery is a 12s2p Li-Ion from MBoards, which has a built-in BMS and a charge port (not pictured), and I'm pretty sure the battery meter I bought has a little switch on it itself, but if not, I can always add a momentary switch if I find that it's an issue. 

I'm not too sure about whether I need a fuse or not, I've seen people post both ways. If I should add a fuse, what Amp rating should it be? If both motors have a peak current of 45A, should the fuse be rated for 90+ A?

Also, there's an XT60 connector between the battery and fuse, I just forgot to draw it. I've seen setups with many more connectors between the VESC and the rest of the wiring (left). Is it necessary or just a convenience?

[Full Parts List](https://docs.google.com/spreadsheets/d/1rAdDfoDBLXXPcLyFwsk4NGGoB_o_kkf0g2Eyqb2e5I0/edit?usp=sharing)

Any feedback would be appreciated! Thank you!
```

---
## \#2 Posted by: a13xr3 Posted at: 2019-07-25T12:30:28.430Z Reads: 34

```
It all looks right to me. I don't personally fuse my boards. Probably should tho... 

I assume your battery fuse should be equivalent, or maybe a slight bit higher, to the max recommended battery drain amps, and I would use an automotive style fuse so you can replace it more easily if it does pop, otherwise you'll be stranded. Also do know that battery amps and motor amps are two separate settings in the VESC are not equivalent. 

DickyHo and Board Dynamics make inexpensive mounts you could also consider.
```

---
## \#3 Posted by: captclearleft Posted at: 2019-07-25T12:43:12.824Z Reads: 29

```
I don't run a BMS.  So, I am not an expert on this particular setup.

That being said...

Doesn't the Loop key go between the Battery and the ESC???

The way it is setup now - the ESC is powered with the loop key  "not" installed.
```

---
## \#4 Posted by: ShutterShock Posted at: 2019-07-25T15:18:59.989Z Reads: 22

```
You are reading the diagram incorrectly, he has it in the right spot :)

I personally don't fuse my boards but my BMS is wired for discharge and limits at 60 battery amps
```

---

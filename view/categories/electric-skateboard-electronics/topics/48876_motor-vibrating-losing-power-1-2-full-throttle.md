# Motor Vibrating losing power 1/2-full throttle

### Replies: 7 Views: 431

## \#1 Posted by: cspaghetti97 Posted at: 2018-03-12T17:30:41.905Z Reads: 77

```
Hello all,
My situation is this, I had a 9s lipo set up just the basic batteries from hobbyking which I had to remove everytime I wanted to charge them. So I ordered some liion18650 cells and built my own pack using vruzend kit. The new batteries are 8s6p. I connected them to my focbox(enertion vesc) to so some testing before i installed my bms. The problem I found is after about half -full throttle the motor start vibrating and it loses all acceleration. It only does this with my new battery packs. So I started testing with different motor max settings on the bldc tool. Using 25A it does not occur, but 40A or higher the motor does its vibrating tantrum. So I tried a different remote...same thing. I plugged in my freinds vesc because we are both building board at the same time and boom, it works perfectly with his vesc. So now I assume I have a problem with my vesc(focbox). It sounds like an amp problem due to the fact that it only occurs when i increase the motor max setting. Has anyone dealt with this before? Thanks 
Info:
Single Motor: 63mm 3200W alien power motor 240kv
Motor Pulley: 15 tooth
Drive Pulley: 40 tooth
```

---
## \#2 Posted by: cspaghetti97 Posted at: 2018-03-12T22:18:16.991Z Reads: 59

```
Update: 
I reconnected my zippy lipo batteries and the board to off great no problem, but i immediately put back on the custom li-ions and it started doing the same problem again.
```

---
## \#3 Posted by: E1Allen Posted at: 2018-03-13T00:17:54.204Z Reads: 51

```
what kind of 18650 cells are you using?  single or dual motor?
```

---
## \#4 Posted by: dg798 Posted at: 2018-03-14T13:14:50.906Z Reads: 34

```
Also are ur cutoff voltages right for an 8s
```

---
## \#5 Posted by: Jumpman Posted at: 2018-03-14T13:36:36.312Z Reads: 27

```
Vruzend?  I thought they were only rated at 3.5A per cell for the battery contacts.  Maybe try setting battery max at 17.5A?
```

---
## \#6 Posted by: linsus Posted at: 2018-03-14T13:46:32.168Z Reads: 26

```
Sounds more like the motor is saturating then it beeing a ESC problem. Any chance you can try a different motor and see if it occours in the exact same way?
```

---
## \#7 Posted by: cspaghetti97 Posted at: 2018-03-14T15:39:20.514Z Reads: 24

```
Thanks for the replies, i did read up that the vruzend is only good for 7a burst and 3.5a continuous. Wish i read this before i bought the kit but oh well. I had the batteries laid out flat which meant only one connection was between each cell. So i went ahead and made the packs 2x12 so now there are 12 connections to make the packs in series. Now the motor doesn't vibrate as noticeable but it is still there at higher throttle bursts. I know it is the vruzend kit now wish i read that before i bought the kit. Also I added a cell to each pack to help with the amount of amounts i was trying to move so now the pack is 8s6p
```

---

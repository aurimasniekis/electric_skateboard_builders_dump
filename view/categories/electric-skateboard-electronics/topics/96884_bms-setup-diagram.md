# BMS setup diagram

### Replies: 6 Views: 177

## \#1 Posted by: stalejarmynd Posted at: 2019-06-18T20:42:00.660Z Reads: 56

```
Hi.

I have plans to build a 10s3p battery, and I'm getting confused about the BMS setup. My friend had this diagram for the charging, but the BMS kept getting hot, like 'ouch' hot. The positive and negative is connected to the first and last cell in the battery pack, where the power are going out to the VESC. Will this setup kill the cells? 

![64309792_2333412823592859_8960479854625554432_n|281x500](upload://6pWGbUDF2ZjOi3VcJk1VgPAgZCg.jpeg)
```

---
## \#2 Posted by: pjotr47 Posted at: 2019-06-18T20:45:48.566Z Reads: 55

```
Diagram?

This is a diagram ![image|690x266](upload://tZfTGKfBOL1rezTwd1FmsYMKGfu.jpeg)
```

---
## \#3 Posted by: stalejarmynd Posted at: 2019-06-18T20:48:43.218Z Reads: 55

```
I could try making it better, and more understandable. Did you understand what i meant?
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-06-18T20:50:26.658Z Reads: 54

```
You need to connect the battery gnd to B-

The charge port gnd to p- if you don’t have a chg - on the bms

And the positive from the charger to the postive off the pack
```

---
## \#5 Posted by: stalejarmynd Posted at: 2019-06-18T20:51:47.430Z Reads: 55

```
![46|690x365](upload://eMepjjTqB8CK5ZkRbzYzUfv0tsV.jpeg)
```

---
## \#6 Posted by: dino15309 Posted at: 2019-06-19T01:36:00.277Z Reads: 34

```
I'm just going to list some things that you probably already know, but hey just in case:

If your 10s bms has 11 wires. This is fine, it just means that the first sensor wire goes to the negative terminal. From there, each of the following leads go to the positive terminal of each "cell" (you might have multiple li-ion cells in parallel within the "cell").

I am using a very similar setup and it works beautifully. As far as wires go, the wires to the charger port only need to be as thick as all the little leads going to the battery. your wire to the B- does not have to be 8 AWG, nor should any of the wires in your board. I use 10 AWG and it works just fine (it will be a lot easier to solder. Tab Welding to the cells is your best option, but soldering is also viable (that probably triggered someone). Make sure that your iron is at least 80 watts, and you are in and out in under 5 seconds. Let the battery cool for like 30 secs and repeat (I have done it so I know it works). 

If you get a spot welder, be sure to use at least 2 layers of nickel strip on the cells in parallel, and a 10 AWG wire between cells, alternatively just more layers of nickel (between cells needs to have ample amounts of conduit). 

Make absolutely sure that you are getting real Li-ion cells, as you can be ripped off. I used battery junction and they were great, especially for Samsung 25r cells

If I left anything out just tell me :rofl:
```

---

# Trying to convert &ldquo;Slave&rdquo; VESC back to &ldquo;Master&rdquo;

### Replies: 4 Views: 361

## \#1 Posted by: kaaaaahle Posted at: 2017-10-28T18:28:28.623Z Reads: 77

```
I have a dual motor board with 2 Torque Boards VESC's. One of my motors broke, so I just took out the second "slave" VESC and disconnected the CAN cable and it worked fine with 1 motor and VESC. The VESC I've been using is now acting up so I need to swap it out for the other one. I'm having trouble getting my remote (standard DIY RC remote) to connect to it.

When I connect the VESC to BLDC it connects and detects the motor fine (spins up and senses it) so I know the VESC is good... but it's just not responding to the remote for some reason when I power it up. Anyone know of a setting or something in BLDC that you need to set it as the "Master"? I tried changing the "Controller ID" back to 0 but that didn't fix it. Is there something I'm missing?

Thanks
```

---
## \#2 Posted by: Lunasi Posted at: 2017-10-29T04:43:01.779Z Reads: 56

```
@okp @Hummie This is my buddy, was trying to help him set up his VESC today but we couldn't figure out how to get his vesc to connect to the remote for some reason. Any advice for him? I've set up a single VESC before myself but have never done dual motor and haven't had to do settings for slave/master. We tried switching the values like in some video tutorials but for some reason it wouldn't connect.
```

---
## \#3 Posted by: Hummie Posted at: 2017-10-29T05:00:27.006Z Reads: 51

```
Some transmitters have complex binding that has to be done. And jams me up often. All I can think is its not binding.  There is an option for other methods of control but forget. 
Maybe plug ur transmitter in or one u know is good and binded
```

---
## \#4 Posted by: i2oadsweepei2 Posted at: 2017-10-29T13:59:01.614Z Reads: 31

```
I know it's obvious, but have to ask. When you switch from dual to single the slave under app config is set to (no app) Did you turn ppm back on? On the same screen uncheck "send status over can".

All the best.
```

---

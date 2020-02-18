# Remote control issues?

### Replies: 8 Views: 402

## \#1 Posted by: Danny414 Posted at: 2018-05-08T22:00:25.726Z Reads: 66

```
I have a 10s5p custom 30q lion  battery pack, 2 focbox's and 63xx motors

Ok so I'm having weird remote issues..

I had the nano x controller and it would disconnect often.. sometimes id have to shut the board off and turn it back on a couple times to get it connect.. and my board actually took off by itself once..

then I purchased the newer maytech rmini remote.. at first it was cool but shortly into me thinking everything was ok.. occasionally when accelerating it seems like it would limit power briefly.. after reading online many people were saying its the remote or could be placement of the receiver.. so I've moved the receiver pretty much every where as far as I can move it and I will get the problem.. then today the remote itself shut off twice on me and it was charged.. so I replaced this one with another maytech mini and it is doing the limiting power thing again.. it always seems to be at random times too.. and it dosent have to be an extreme amount of acceleration... I had one ride where it didn't do it at all, the whole ride..

what are some other common issues.. could it be the VESC? battery? BMS?

Thanks guys!
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-05-08T22:08:39.224Z Reads: 55

```
Could you post screenshots of your focboxes settings? Also how many amps is your BMS good for? Did you build the pack or buy it?
```

---
## \#3 Posted by: Scoo_B_SK8 Posted at: 2018-05-08T22:09:09.373Z Reads: 57

```
get under the hood and check DRV chip and fets.

i had a maytech that was half way blown and would cut out from time to time. 

 also could check it off the list of whats wrong by simply looking at those. 

 check wires/solder joints too.

 Use terminal and check remote responses.
```

---
## \#4 Posted by: Danny414 Posted at: 2018-05-08T22:22:51.331Z Reads: 49

```
you know whats weird was when I was connected to the master focbox to calibrate the new remote.. when I had the he display ticked and the disabled box ticked in PPM tab.. there was no response and I noticed the focbox disconnected itself.. and a last week the master focbox completely reset itself back to defaults.. but as soon as I get home I will start messing around with a few more things.. I think im going to switch focbox roles.. make slave master and master slave and see what that does too
```

---
## \#5 Posted by: Danny414 Posted at: 2018-05-08T22:27:46.471Z Reads: 44

```
I purchased the pack from one of the guys on this forum.. the bms can shoot out up to 40a.. here is just one of the pics I have on my phone, I’ll take the others when I get back
![image|666x500](upload://m0QoNYbLQ2xTC9UPdbjjbf6fxuf.jpeg)
```

---
## \#6 Posted by: Danny414 Posted at: 2018-05-08T23:09:09.112Z Reads: 36

```
Ok here they are 

![image|666x500](upload://fom8MKbWw0iSqHPDzmT0vIvDq6B.jpeg)![image|666x500](upload://aicwiFe8fnyXyW60U76CUusfCs8.jpeg)![image|666x500](upload://7xk0XZI0FVzkK3Qgpd83W96qRRU.jpeg)![image|666x500](upload://ghvczxt53iGne8J6fkBrJnomMFF.jpeg)![image|666x500](upload://m0qaJlHIFV2l1fg5IsMHloOeOTE.jpeg)![image|666x500](upload://9ZxrtbDQbxIBppWEQ6qifAli9pU.jpeg)
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-05-09T00:42:38.488Z Reads: 29

```
Look over your battery cut off settings & maybe lower min input voltage to 6

Check your battery pack with multimeter when fully charged.  Make sure your getting what your expecting.
```

---
## \#8 Posted by: Danny414 Posted at: 2018-05-09T00:58:21.552Z Reads: 26

```
Will do. I checked the battery when I first got it and it was pushing out 42volts.. I just switched the focboxs from master to slave and slave to master and rode around for a bit and it was smooth.. but we’ll see over the next couple days.. I put at least 10 miles on a day so should know soon enough.. thanks
```

---

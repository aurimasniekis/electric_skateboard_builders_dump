# Need help: Hall sensor detection not working with brand new motor and esc

### Replies: 10 Views: 2925

## \#1 Posted by: kylepls Posted at: 2017-11-07T19:46:48.276Z Reads: 223

```
Hello all!

I am having a bit of trouble getting the BLDC tool to complete the hall sensor table. I have created a 5 pin to 6 pin adapter to connect the leads coming off of the motor to the vesc (4.12). I am very certain that I have correctly soldered all the joints together as I have resoldered this twice and have had similar results. 

Any help is appreciated! 

Motor: https://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html?rmmds=myorder&cur_warehouse=CN

<img src="/uploads/db1493/original/3X/c/a/ca5ab86193b2cc6d508ffc4495e4b804b4efe5fb.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/f/af167687bfe647c7b460d901400670e0110dadc9.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/0/3/03821cef33d70f9cdc802a7f8b0e6fc8bf9b9f83.png" width="690" height="407">
```

---
## \#2 Posted by: bullrider12 Posted at: 2017-11-08T08:52:07.241Z Reads: 199

```
I think you have a retry similar problem like me:
https://www.electric-skateboard.builders/t/unknown-hall-error-255/37058?u=bullrider12

If you got a solution for this, pleas tell me!! :slight_smile:
```

---
## \#3 Posted by: vishal_tejwani Posted at: 2017-11-08T09:16:50.610Z Reads: 193

```
if got solution i need too, same setup
```

---
## \#4 Posted by: kylepls Posted at: 2017-11-09T20:33:55.541Z Reads: 194

```
Still having the issue. Need help! :frowning:
```

---
## \#5 Posted by: AntiumOne Posted at: 2018-03-22T01:13:55.888Z Reads: 175

```
I have had the same issue with a 200kv racestar 5045 motor. 

https://www.banggood.com/Racerstar-5045-BRH5045-200KV-6-12S-Brushless-Motor-For-Balancing-Scooter-p-1117661.html?rmmds=search

I have done a ton of research and I finally got my sensors to work.  I though the sensors were bad and considered replacing them all together but I found the solution before it came to that. 

What it came down to was the correct wiring of the sensors to the vesc. The sensors were perfectly fine and had no issues. 

The black and red wires from the sensor turned out to follow convention (red = positive, black = ground) even though the wiring diagram online says otherwise. 

I swapped the wires around until I read the following from my multimeter.  The ground of the multimeter was placed on the ground pin for the hall sensor. 

5v pin should be approx. 5v

temp pin is skipped

hall 3 pin was approx. 0v

hall 2 and 1 pin were approx. 3v

You will know everything is wired correctly when one hall sensor is zero volts and the other two are around 3v.  When I received UNKNOWN HALL ERROR: 255, each hall sensor pin was reading ~4.3 volts which is incorrect. 

If you don't have a multimeter, go pick one up.  They are fairly cheap, and will help you resolve this issue. 

Running the motors in sensored mode is well worth the extra effort.  No more cogging, and I have excellent start up torque. 

Good luck.

Edit:  Just swap the red and black wires around and the other hall sensor wires that ARE NOT white.  The white wire (middle wire) is almost certainly hall 2.  Swap the wires around until you get the correct reading with the multimeter.
```

---
## \#6 Posted by: kylepls Posted at: 2018-03-22T01:33:54.720Z Reads: 165

```
I'll give this a shot later tomorrow. Can you post what pin you put each wire to for comparison purposes?
```

---
## \#7 Posted by: Redfire1 Posted at: 2018-04-14T05:11:57.022Z Reads: 149

```
@AntiumOne hi morning I can’t get my head around this wiring sensor looking at this pic from right to left what’s the pin sequence and what’s the wire colour sequence I am using a racestar 5056 motor 140kv ![image|690x425](upload://3ozsJGSV22YRm1vwf6ZhRirUNhX.jpeg)![image|409x499](upload://GkgNv8bqT20btmDJhONhI7lk6R.jpeg)![image|230x500](upload://eQqJ1ifraMalnH6PbeHneNnQFkG.jpg)
```

---
## \#8 Posted by: Redfire1 Posted at: 2018-04-14T05:23:11.782Z Reads: 139

```
@AntiumOne that’s the sensor 6 pin wire that come with my vesc and I found this diagram of a vesc layout 
![image|311x499](upload://trkdA8cdKAN2gO7FQhN6TAi6ByP.jpeg)![image|375x500](upload://gh7YwPEYBtvARXwHhaw1T6GhBv3.jpeg)
```

---
## \#9 Posted by: Redfire1 Posted at: 2018-04-14T05:27:11.877Z Reads: 138

```
@kylepls hi did you get you sensor to work and how did you connect them I have the same setup ![image|409x499](upload://GkgNv8bqT20btmDJhONhI7lk6R.jpeg)
```

---
## \#10 Posted by: kylepls Posted at: 2018-04-14T17:10:39.582Z Reads: 124

```
I never got it working :frowning:

I'm gonna just call it quits on trying to make this thing work. Sensorless works good enough for me.
```

---

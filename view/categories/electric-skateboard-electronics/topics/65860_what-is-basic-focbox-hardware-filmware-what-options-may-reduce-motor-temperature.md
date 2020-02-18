# What is basic focbox hardware/filmware? What options may reduce motor temperature?

### Replies: 6 Views: 210

## \#1 Posted by: cypa9904 Posted at: 2018-08-23T19:04:16.575Z Reads: 102

```
Hi. :slight_smile:
 I got foxbox 2 months ago. Should I update it? Or it already has newesy versions?

 Btw anyone knows what options may reduce motor temperature? Focboxes are cool, maybe 40°C but motors are very hot, for sure hoter than 65 degrees.
 I read sth about changing duty cycle but idk if there is sth else that could help.

My setup
Dual 10s 192kv brushless sensorless motors. Mountainboard 8" wheels, 1:4.55 reduction.
Thanks for any help! :)
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-08-23T19:23:38.978Z Reads: 95

```
The FOC box is a 410,411,412 hw. You shouldn't NEED to update it but you are welcome to. I like to use @Ackmaniac firmware which would require you to update the firmware with his. 

Are you running BLDC or FOC? Changing may impact your temp. We would also need to know your motor/battery amps to help solve this.
```

---
## \#3 Posted by: cypa9904 Posted at: 2018-08-23T19:31:14.957Z Reads: 94

```
Oh xd how do I know what hw it has? I mean 4.10 or 4.11 or 4.12? :) I do not get it :smiley:
My motors : turingy  6374
Battery -> 4x li po 8ah 5s 30C which gives me 16ah 10s 30C, they are literally cool so they are ok :) I do not have a bms, i control cell voltage with my battery.
I am running foc. I do not want to use akmaniac filmware because of warranty xd. I know that I can but I would prefere not to do it.
```

---
## \#4 Posted by: Hummie Posted at: 2018-08-23T19:34:44.462Z Reads: 86

```
i dont think you will find any way to decrease the motor temp other than decreasing your gear ratio or reducing the current to the motors with the vesc settings. higher voltage wont help
```

---
## \#5 Posted by: cypa9904 Posted at: 2018-08-23T19:38:11.218Z Reads: 84

```
I read 2 posts where people said that they updated filmware and changed some frequency and it worked then. This is why I wonder if there is sth else. And I do not get this 4.10 4.11 4.12 fw xd. I literally dont know why are there three versions and if I can update it. Btw after updating filmware do I need to configure motor settings, detection and so on once again?
```

---
## \#7 Posted by: briman05 Posted at: 2018-08-25T01:21:24.803Z Reads: 52

```
Do you have a dual set up dual if you have had the focbox over 2 months your out of the warranty period unless you go the platinum warranty for a year
```

---

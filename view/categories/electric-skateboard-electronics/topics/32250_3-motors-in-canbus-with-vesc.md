# 3 motors in canbus with vesc?

### Replies: 8 Views: 579

## \#1 Posted by: facepalmsareus Posted at: 2017-09-04T16:51:37.805Z Reads: 112

```
Has anyone tried to use 3 vesc's and 3 motors (or 4 motors and 4 vesc's?) i'm thinking that would be a really awesome offroad board or if i wanted to make an electric go kart that would be an easy way to make a drive chain but i don't know if more than 2 can be done...
```

---
## \#2 Posted by: BigBoyToys Posted at: 2017-09-04T17:01:32.162Z Reads: 112

```
Yeah I use 4. To be honest Id recommend using additional receivers linked to the same remote transmitter as linking more than two vescs via CAN hasnt been a trouble free experience.
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-09-04T18:12:42.102Z Reads: 100

```
can't u just use(2vesc)(2vesc) y cable (reciever) instead? I juse wanna know why u use 2 reciever
```

---
## \#4 Posted by: BigBoyToys Posted at: 2017-09-04T18:43:08.434Z Reads: 90

```
Yes, Ive used:
1. 1 receiver for 4 VESC's with a ppm cable split 4 ways.
2. A single ppm shared via a 4 way CAN bus cable.
3.  Two receivers (1 for front motors, and 1 for rear motors) with CAN. 

Ive decided Id just pay an extra $20 so each VESC could have its own reciever. All three of the above mentioned strategies worked, but ive had issues while running all three and none since going 4wd with independent control. So Im sticking to what has worked for me.
```

---
## \#5 Posted by: facepalmsareus Posted at: 2017-09-05T03:45:47.721Z Reads: 66

```
What controller do you use? Thanks for the advice btw!
```

---
## \#6 Posted by: BigBoyToys Posted at: 2017-09-05T04:08:48.776Z Reads: 62

```
My builds all have different controllers. Torqueboards, Ollins, VescX, FOC box's, VESC 6. Ive been mostly using FOC box's lately due to their form factor, enertion's customer support has been good to me as well.
```

---
## \#7 Posted by: lowGuido Posted at: 2017-09-07T00:32:26.483Z Reads: 41

```
you could have two lots of 2 VESC canbus connected and then split the PWM cable once to each pair.
```

---
## \#8 Posted by: facepalmsareus Posted at: 2017-09-07T02:59:21.035Z Reads: 34

```
can you upload a picture of what you mean?
```

---

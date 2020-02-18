# WIP, new motor controller

### Replies: 4 Views: 345

## \#1 Posted by: adammunich Posted at: 2019-06-11T17:56:54.465Z Reads: 135

```
Sup,

I'm Adam, a hacker who's versed in electronics design and is dis-satisfied with how every electric scooter I've ever bought has broken both physically, and occasionally my bones too. 

For the past few months or so I have been developing a new motor controller which characterizes the motor in such a way as to extract the maximum possible torque and speed out of the machine. I gave up trying to follow the code in VESC, so _it is not a vesc derivative_ --it is a completely different animal with new software.

I plan to support dual motors and will have advanced features to ensure I don't for example, destroy batteries. Given how much time I've been investing it probably makes sense for the motor controller to find its way into other people's esk8's as well. 

What would be important to have in a controller, y'all? I also don't have a name for it...
```

---
## \#2 Posted by: rusins Posted at: 2019-06-12T13:09:53.010Z Reads: 87

```
A feature I'd like to see implemented:

Acceleration control mode – so that while riding on flat you can't give your motors any more than 30A because more will throw you off, but while riding hills it'll give them up to 60 or 80A, because going up hill requires more torque for the same perceived acceleration from the rider.

On flat acceleration control mode would feel similar if not better than current control mode :slight_smile: 
(If anyone knows how to achieve this with a regular vesc, hmu)

Idea or the name: MuhESC (letters from your last name :stuck_out_tongue: )
```

---
## \#3 Posted by: JulianS Posted at: 2019-06-12T14:10:20.936Z Reads: 69

```
Hmm that should be possible rather easily, it probably needs an addition to the Vesc but basically you a) could increase current with speed or b) use the acceloremeter that's built in.

@adammunich you're actually from munich? ;)

Do you you have an exact description for the type of controller you want to use? Is it using a b6 bridge? If so building off a Vesc makes a lot of sense, no need to reinvent the wheel.
```

---
## \#4 Posted by: Paulycnotes Posted at: 2019-10-24T00:58:49.752Z Reads: 18

```
Well... To definetely have the option of using Sensored or Unsensored Motors (using FOC or Sinisuisidal) as well as having a Turbo button that will increase the Voltage for a few seconds to give you an extra boost (such as the Backfire Board).  Also, to make sure you may use up to a 12S and not the usual 10S which they have but cant get you to the speeds that you want to because ALL or MOST of the ESK8 Motors are really RC Motors which have KV Ratings (For example... my motors have a KV of 170.  Therefore, the RPM's are based on 170 revolutions per 1 Volt).  Therefore, on a 36V (10S) you dont get as much out of that 170KV motor due to the lower voltage.
```

---

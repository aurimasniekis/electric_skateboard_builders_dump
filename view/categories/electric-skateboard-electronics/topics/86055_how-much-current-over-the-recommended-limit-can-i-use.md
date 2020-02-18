# How much current over the recommended limit can I use?

### Replies: 5 Views: 229

## \#1 Posted by: skaterscooter Posted at: 2019-03-04T14:22:27.548Z Reads: 105

```
I have  [this motor](https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html) and the 'Max Loading' is rated at 65A which is what I'm running at the moment. I'm using it on a bike with a VESC 4.12. Would it harm the motor to run at say 80A or is 65 the absolute limit. I will have to add additional cooling to the VESC as it gets quite hot when going up hills but that's not too hard. Any thoughts?
```

---
## \#2 Posted by: Friskies Posted at: 2019-03-04T14:44:54.506Z Reads: 94

```
Running higher amps through your motors won't get your a higher top speed only torque. I would say that 80 will be fine and the motor is rated for 65A continuous. I could be wrong though.... I was would say worst case the motor will overheat the magnets and you will lose power.
```

---
## \#3 Posted by: captclearleft Posted at: 2019-03-04T16:27:50.850Z Reads: 70

```
I agree with Friskies.  The amperage will give you more torque (uphill power).  

I would worry more about my batteries, and VESC before the motor.  

Example: VESC 4.12 is rated at 50a continuous and 240a for "short" burst.

A [Lipo 5A 20C](https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack-xt-90.html) is  rated for 5x20 = 100a continuous ( I would not do this Hot Hot Hot!).

An 18650 Cell rated at 3a is usually thought of as 2c - 8c depending on battery...  (You would have to look at the specs).  So, Lets say you are using cheap aliExpress knockoffs at 2c or 3a x 2 = 6a ...  If you are running your 18650 cell pack at lets say a 4p.  Then that is 4x6 = 24amps.  I could have explained that better...

I am open to correction...  I am not an 18650 guy...
```

---
## \#4 Posted by: skaterscooter Posted at: 2019-03-04T21:00:41.637Z Reads: 48

```
Ok thanks for the feedback. My li-pos are rated for 120A max so should be ok there. They also have quite a bit of ventilation. I'll try running at 80A and see if it makes a considerable difference and nothing get too hot! As Friskies mentioned and I forgot to, I'm trying to increase torque and therefore acceleration not speed.
```

---
## \#5 Posted by: pat.speed Posted at: 2019-03-04T21:03:04.672Z Reads: 45

```
Lipo ratings are exaggerated, I don’t think you could pull more than about 60-70a with them over heating
```

---

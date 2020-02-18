# Understanding Battery Current Max?

### Replies: 3 Views: 499

## \#1 Posted by: Ryguy Posted at: 2018-08-25T21:30:17.982Z Reads: 155

```
So I have a 9s2p battery (Samsung 30q) with the diyelectricskateboards vesc and a single bkb 6374 190kv 320W motor. The motor is rated at max 70 A.

I keep reading that you have to set the motor max and max brake in the Golden zone. Which I believe would be 65 A Max, and -55 A Max brake. However not sure enough to test and fry my motor.

Also, for battery current max I cannot find somewhere explaining how to set this value up just specific numbers for batteries like 10s3p. I'm thinking for my setup the battery current max should be 40A and the current max regen -10 (some said as low as -6).

If someone could help me understand and make sure my values are correct I would be much appreciated (Don't feel like braking another motor) Thanks!
```

---
## \#2 Posted by: professor_shartsis Posted at: 2018-08-25T22:01:40.902Z Reads: 143

```
here is a comparison of different battery current limits (10a, 20a, 30a, 40a, 50a, 60a), all with 60a motor current limit...

during full throttle acceleration, increasing the battery current limit improves the vehicle thrust at higher speeds, as seen from the yellow line, bottom left chart -- vehicle thrust in pounds, 2 motors bldc.

https://image.ibb.co/gDnNa9/10a_20a_30a_40a_50a_60a.gif
```

---
## \#3 Posted by: Andy87 Posted at: 2018-08-25T22:14:02.399Z Reads: 132

```
With your 2p 30q pack you can set your bat max to 40a without problems. Your bat min with -10 should be fine as long as you don’t plan to drive down a 5km hill with reg breaking all the time it’s usually just for a short period when you charge back into your cells.
You can set your motor max anywhere to your max rating of your motor and the min according to your personal preference of breaking force. 
As for me you choose the right settings for your application
```

---

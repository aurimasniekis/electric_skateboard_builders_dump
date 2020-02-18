# Automatic brake lights, using an accelerator as the main sensor

### Replies: 6 Views: 833

## \#1 Posted by: NilsS Posted at: 2017-08-04T21:08:08.812Z Reads: 161

```
anyone know if its possible to use an acceleromoter with an arduino based microcontroller. (I am not using a vesc so i cant tap the braking signals) to create an automatic brake light? Anyone with experience with acceleromoters?
```

---
## \#2 Posted by: t0m_r1dd1e Posted at: 2017-08-04T21:24:01.330Z Reads: 158

```
Yeah this would totally be possible. Cool idea! Accelerometer to Arduino controlling a relay, should be pretty simple. This would do it: https://www.sparkfun.com/products/13963

Run power and ground to that acc, run a signal wire from a1, a2 or a3 depending on how it's oriented, and then just figure out the threshold where you want the brake light to turn on.
```

---
## \#3 Posted by: saul Posted at: 2017-08-04T22:25:29.398Z Reads: 147

```
yes you could do this. but it would be more work to read the imu data and figure out whats happening.

I just read the rx signal directly and trigger brake lights. you can see some of how I did here. updating now...

on a side note. I have thought about using an accelerometer/gyro for some carve control lights. ;)
http://www.electric-skateboard.builders/t/brake-lights-and-turn-signals-finally-for-any-esc/15888/17
```

---
## \#5 Posted by: NilsS Posted at: 2017-08-04T22:37:41.573Z Reads: 122

```
Unfortunately i am using an ESC/reciver combo board, witch makes this quite hard without an oscilloscope. tracking traces is kind of hard.
```

---
## \#6 Posted by: saul Posted at: 2017-08-05T03:31:29.357Z Reads: 105

```
thats true. in that case the imu should work.
mpu6050 are pretty cheap and easy to work with over i2c.
```

---
## \#7 Posted by: NilsS Posted at: 2017-08-05T09:18:16.327Z Reads: 90

```
I have a MPU 6050 on my racing drone.
```

---

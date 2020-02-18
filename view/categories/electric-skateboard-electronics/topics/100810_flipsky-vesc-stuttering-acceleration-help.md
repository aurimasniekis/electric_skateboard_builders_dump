# Flipsky Vesc stuttering acceleration help

### Replies: 6 Views: 166

## \#1 Posted by: yulaw2k Posted at: 2019-08-24T22:21:47.613Z Reads: 57

```
https://www.youtube.com/watch?v=R8ObhL0iMa4&feature=youtu.be

Heres a video of where I am at right now.
Just got everything about hooked up. I cant get the hall sensors to work, but I dont think they ever worked on my diy meepo board years ago which is where they are from. 

When I slowly hit the accelerator you can see the motors just stutter, then one starts going, and the other will finally start spinning at max speed. I havent tested it on the ground yet to see if it makes a dif, because I am still building everything.
```

---
## \#2 Posted by: yulaw2k Posted at: 2019-08-24T23:15:24.766Z Reads: 51

```
I am guessing its because of the hall sensors not working? Any idea if theres a way to test the hall sensors on a motor? I am fairly certain I wired them the right way (On the far motor) but they are not being detected.
```

---
## \#4 Posted by: shupeste Posted at: 2019-08-25T21:55:15.783Z Reads: 40

```
How did you figure it out, kinda dont wanna go digging. Having the same problem when its only accelerating
```

---
## \#5 Posted by: yulaw2k Posted at: 2019-08-25T22:16:59.785Z Reads: 37

```
I actually didn't figure it out. After some forum searching i believe because my hall sensors are not working which causes the stuttering, but once it gets going it's perfectly fine till it's a complete stop. I also can't figure out how to get my hall sensors working or even figure out if they work at all. I read some post about checking the voltage on the hall sensors but I need some finer more precise points on mine to check.... I'm planning on upgrading to a mountain board setup so I'll just go without hall sensors till then, unless anyone can offer any advice.
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-08-26T00:05:58.372Z Reads: 35

```
@yulaw2k  To check the hall sensors: Supply 5v to the red and black wires. Then, one at a time, probe for voltage between ground and the hall wires, while slowly rotating the motor. You should get a signal that alternates between close-to zero (0-0.5v) and close-to-VCC (3-5v) on each of the three hall wires as you rotate. If so, then your halls are good. If not, then they're either dead or not wired in a manner I'm familiar with.
```

---
## \#7 Posted by: yulaw2k Posted at: 2019-08-26T02:08:24.106Z Reads: 29

```
Oh man, thanks alot! Thats a great and clear explanation.
```

---

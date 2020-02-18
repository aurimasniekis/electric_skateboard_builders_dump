# Flipsky VESC Setting to fix motor sudden pause issue

### Replies: 8 Views: 157

## \#1 Posted by: AutoCar Posted at: 2019-11-01T14:35:42.928Z Reads: 57

```
Hi, I am running a Flipsky VESC with a Traxxas Slash 4x4 RC car. So my application is different from the e-board, but the purpose of the VESC is the same. My car is controlled by a computer program and the program set speed and steering command to the VESC. I am part of the DIY robocar group and the car races with each other on a fixed loop track. More info can be found here https://diyrobocars.com/

I found however, sometimes the car suddenly paused during a race. When it happened, the VESC flashed red. It stopped there for a couple seconds and then re-launch and continue to run. I found the behavior is repeatable and it pretty much paused at the same locations along the track. I guess it was because it triggered some VESC limit and shutdown the motor. I am pretty new to VESC so I help you can help me with the VESC setting show in the picture. Any idea if there is error messgae I can retrieve? Is my setting OK? What is the root cause of the pause?

Thank you very much. 

![Screenshot%20from%202019-11-01%2007-28-09|690x423](upload://tk8p3HkvMi2qkzn60dYrIiZMLBk.png)
```

---
## \#2 Posted by: adman Posted at: 2019-11-01T17:05:13.768Z Reads: 45

```
I would check your fault codes on your vesc and set your 100amp values to 60amp.
```

---
## \#3 Posted by: AutoCar Posted at: 2019-11-01T18:25:41.683Z Reads: 42

```
Thank you for your feedback. 
How can I check the fault code? 
And also why set the currently lower?
```

---
## \#4 Posted by: AutoCar Posted at: 2019-11-03T21:09:51.765Z Reads: 30

```
I found the issue. The fault code was FAULT_CODE_OVER_TEMP_FET. And the temperature is out of my limit. I changed the limit to 300, the car ran fine for some time. However, got this fault code again in a few minutes. The temperature was 304. When I touch the VESC, it did not feel it was this hot. Should I change the limit 500? 

Also, the VESC was wrap in plastics when I received it. Should I cut and remove the plastics?

Thanks.
```

---
## \#5 Posted by: bigben Posted at: 2019-11-04T06:54:56.725Z Reads: 28

```
You’ll need some kind of heat sink on there. (Removal of the plastic will help a little)
Maybe a different version of vesc based controller with built in sink.
```

---
## \#6 Posted by: banjaxxed Posted at: 2019-11-04T07:13:43.531Z Reads: 27

```
You might be able to buy a heatsink from flipsky if not then look for any 4.12 or make your own

3DServisas made these (I still have a pair)

![image|281x500](upload://b7GVVnr3fsNfDCqoXqcWjCnUfMk.png)
```

---
## \#7 Posted by: AutoCar Posted at: 2019-11-07T01:00:01.862Z Reads: 23

```
I found the highest temperature limit I can set in BLDC tool is 300. Is there a way to set this this limit higher, for example, 500?
```

---
## \#8 Posted by: ChrisZ Posted at: 2019-11-15T10:50:33.159Z Reads: 12

```
Check out MICHOOBY shop, very cheap price for VESC case US$14.9/pcs
```

---

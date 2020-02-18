# Weird VESC behavior or motor problem?

### Replies: 1 Views: 270

## \#1 Posted by: evoheyax Posted at: 2017-08-12T23:27:13.759Z Reads: 46

```
The past week, I have spent rewinding and re-sensoring my 4 hummies hubs. Everything seems good at first sight, but there's clearly something wrong. And I have yet to figure out what is wrong. 

My problem: One of the front motors stutters and cogs quite a bit. When I tried it yesterday, there was no cogging or anything, but the day before, their was cogging also. For the last 2 days, it has always passed the foc detection tests with out any issues. Today, it failed, over and over. I had to spin it by hand a bit to overcome the cogging so it could pass the test. It then seemed fine. I pushed backwards, and the motors quickly over came the backwards riding and through me forward with great acceleration. Sensor detection has always passed also. Even with sensors turn off, it cogs more than the others do with the sensors turned off.

I'm basically trying to figure out where the problem is: the VESC or the motor.

Based on the cogging, I would say it's the motor. But the speed controller is a custom quad vesc made by @chaka. I was using it about a month ago and a motor short circuited (carvon v2). I was riding with it so IDK how long, and with the 3 other motors still running fine, I didn't notice that much of a difference to cause alarm at first. This VESC also says the temp sensor is at -30 C, which it's clearly not at. There's no faults thrown, even during acceleration or braking.

It feels like the VESC is acting funny, and when ran on other VESC, it worked without issue.

Anyone have any tests in mind that might help diagnosis this?
```

---

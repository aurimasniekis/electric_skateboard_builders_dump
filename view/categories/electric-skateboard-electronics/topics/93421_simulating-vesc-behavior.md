# Simulating VESC behavior

### Replies: 9 Views: 109

## \#1 Posted by: janpom Posted at: 2019-05-10T20:39:53.272Z Reads: 47

```
I'd like a very simple VESC software model that I could use for my DAVEga developments. The idea is that instead of hooking it up to a real VESC and reading real VESC data, I generate some data randomly and use that for testing. This would be very useful for late night coding when I can't make noise with real VESC and motors to test stuff.

It doesn't have to be very sophisticated but I also don't want completely random values that would contradict each other. For example, I don't want the RPM to go down when duty cycle is going up, etc.

My idea is that given a VESC state, I randomly generate a decrease/increase in the duty cycle and I compute how that influences the RPM, battery amps, motor amps, battery pack voltage, mAh discharged, etc. Say for an average board with average components and an average rider riding on an average surface. The goal is to get very rough estimates in a simple way.

Has anyone ever tried doing something like that? Would anyone be able to give me some formulas? For example, given duty cycle and current RPM, compute new RPM.
```

---
## \#2 Posted by: linsus Posted at: 2019-05-10T20:45:53.698Z Reads: 44

```
If you're familiar with the data representation, cant you develop an emulator? Its the best I can think of.
```

---
## \#3 Posted by: janpom Posted at: 2019-05-10T20:51:55.891Z Reads: 41

```
I guess I'm not sure what you mean. Maybe you misunderstood the question. It's not about data representation. It's about getting the values right. You can't just randomly generate the data for each reading. Like get 1,000 RPM from one reading and then get 100,000 RPM from the next one that happened 100 ms later. That could just never happen in the real world.
```

---
## \#4 Posted by: linsus Posted at: 2019-05-10T21:11:36.423Z Reads: 36

```
Whats the purpose then? Is it not to have a quiet way to simulate data output? Are you sure you're not overhinking it?

I get that you might want "real world values". But you'll have to define variable dependencies that is quite linear in your emulator. I mean. Trying to copy the data output of a certain hill..is..abit overkill? 😂
```

---
## \#5 Posted by: janpom Posted at: 2019-05-10T21:18:02.705Z Reads: 32

```
As I said, I'm not looking for anything sophisticated. I'd just like a simple model that would very roughly simulate what might happen on a VESC in the real world. I would be happy with anything that wouldn't generate data that's obviously wrong at first sight such as the RPM example I mentioned.

Ideally I'm looking for simplified functions that would give me a new value of a variable (RPM, motor amps, battery amps) by taking its current value and the duty cycle as input.
```

---
## \#6 Posted by: linsus Posted at: 2019-05-10T21:20:58.572Z Reads: 27

```
Then I sugest digging into the code. The formulas are all there. Even the inverse clark transformations for the FOCalgorithm
```

---
## \#7 Posted by: oyta Posted at: 2019-05-10T21:22:37.174Z Reads: 26

```
What about logging a ride and «playing» it back in? I think you have shown that you use Metr - I guess you can reuse those datas.

I am not sure about your test setup, but you need at least some software to translate Metr logs to the same format as you get from the VESC.
```

---
## \#8 Posted by: janpom Posted at: 2019-05-10T21:23:37.951Z Reads: 24

```
That's a great idea. Thanks.

I actually have some Metr logs I can use straight away.
```

---
## \#9 Posted by: linsus Posted at: 2019-05-10T21:31:10.355Z Reads: 20

```
Thats probably the most time saving yes 🤣 god Im dumb
```

---

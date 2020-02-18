# Independent lipo buzzer switching mechanism with transistors, for control of each battery

### Replies: 1 Views: 101

## \#1 Posted by: michondr Posted at: 2019-05-02T12:41:01.844Z Reads: 24

```
Hi there guys! 
I'm building new battery out of S3 lipo cells out of hobbyking. the configuration will be a little bit strange, either 3s2p4s or 3s4s2p, because no bigger batteries could fit in my case under the deck.

I plan to have each 3s battery hooked up with the cheap lipo under-voltage protection buzzers in case anything goes wrong

![image|513x500](upload://aFVFHPgl1OI6dWxdEXBm87TNLxq.jpeg) 

the thing is, according to what I've read, they drain cells unevenly. 

offtopic story - I've killed two 5s batteries either because of these (2 cells died) or because of my ignorance of keeping them under-voltage when the buzzer was not connected :smiley: 

my point: I'd like to construct a simple circuit that switches the GND wire of balance leads on every 3s pack independently. this could be for sure done with relays where the coils would be connected in parallel and current would flow through then when a sparkless plug is inserted (completing circuit, supplying power to VESC). however, we live in an era of transistors, lowering the price of the switching mechanism, making relays obsolete :D the problem is, that I have no clue how to make the transistors not share the same ground, as between ground of each buzzer is ~3.7V difference

diagram of what I want to do (with relay):
![image|496x500](upload://8ozToOqx39wVGSVXDvbU15iSirg.png) 

my question is, how to connect 8 transistors (probably in parallel) so that the voltage difference is no problem. Or other solutions for this problem
```

---

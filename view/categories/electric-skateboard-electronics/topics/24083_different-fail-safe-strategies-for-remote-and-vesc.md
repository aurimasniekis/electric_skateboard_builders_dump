# Different fail-safe strategies for remote and VESC

### Replies: 3 Views: 890

## \#1 Posted by: Mathias Posted at: 2017-05-28T20:25:49.983Z Reads: 154

```
I am currently planing my first build and am a bit hung op on the choice of remote. I've read tons of reports here regarding the reliability of different remotes and their "fail-safe" behavior. 
Most people seem to be happy with a remote, which will send a neutral throttle signal to the ESC in case of a fault. This is obviously better than jumping abruptly to maximum braking, or repeating the last signal. 

But I live an extremely steep, urban area. Going down a 20% slope, the remote crapping out, and setting the throttle to coasting is just as bad as a board jumping to full throttle on flat ground. So the best fail-safe behavior that I can imagine would be if the board slowly starts ramping up to maximum brake current. 
As far as I understand, the VESC firmware already has a fail-safe feature, that can be configured to apply a certain brake current. But for this to to work properly you need:
1) A remote, whose receiver will STOP sending signals to the VESC all together. Not neutral, not reverse throttle. 
2) A slow ramping of the braking current to not simply throw you off. 

I'd appretierte the input of the more experienced builders here! How do you set up your fail-safe? Does this controlled braking type of fail-safe exist at the moment? 
And yes, I am aware that there are very reliable controllers out there (GT2B etc.), and many of people will have the urge to reply "I've used XX remote it for XY and never had an issue", but I still think it is worth discussing such a crucial safety feature for something as dangerous as an electric skateboard...
```

---
## \#2 Posted by: saul Posted at: 2017-05-28T22:30:32.470Z Reads: 130

```
As for as i know this type of feature doesn't exist yet. 
but I think you may have read too many horror stories. 
My mini remote has done great, with only 1 failure a couple weeks ago where the breaks did not engage and I had to jump off.

But this was my fault for going too fast, where I knew the hill would be too much for me without breaks. what it really comes down to is to, is dont ride beyond your skill!
Your breaks will be there 99% of the time, but you shouldn't expect them to save you, and you also shouldn't expect any other sort of failsafe to either.

now thats out of the way.
I'm working on a custom remote, and will likely implement a fail safe like you said.
on lost connection, the rx will ramp up breaking to a stop. 
But i'm not sure how this will actually feel, and I really would prefer this is never needed to be used.
```

---
## \#3 Posted by: Mathias Posted at: 2017-05-28T23:13:22.704Z Reads: 115

```
[quote="saul, post:2, topic:24083"]
But this was my fault for going too fast, where I knew the hill would be too much for me without breaks. what it really comes down to is to, is dont ride beyond your skill!Your breaks will be there 99% of the time, but you shouldn't expect them to save you, and you also shouldn't expect any other sort of failsafe to either.
[/quote]
Well, you are right, but this is not the way I meant it. A it is a safety feature, not a license to be stupid. Nevertheless, we should try to make it work, as it may save somebody from getting injured or worse some day. You also don't put on your seat belt in a car or a helmet on an esk8 with the intention to put it to use. 
[quote="saul, post:2, topic:24083"]
now thats out of the way.I'm working on a custom remote, and will likely implement a fail safe like you said.on lost connection, the rx will ramp up breaking to a stop. But i'm not sure how this will actually feel, and I really would prefer this is never needed to be used.
[/quote]
That sounds cool! Although, I think in the long run the fail-safe routine should be handled by the VESC instead of the receiver. I'll start my build next month, and I guess for now I'll get a remote with a standard fail-safe, that I can set to neutral, or a small braking throttle. But I'll definitely start to look into this. I just don't want to reinvent the wheel, and would like to know if someone already did.
```

---

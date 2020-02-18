# How do I run Sensored on VESC? FOC?

### Replies: 11 Views: 4717

## \#1 Posted by: Brando Posted at: 2016-10-12T02:05:21.219Z Reads: 417

```
I am planning on replacing my TB 12S 120A car esc with torqueboard's vesc. I know that vescs are great with startup torque even without sensored setups, but I want all the smoothness that I can get.
I have no idea how I would run sensored though, considering that the phase wire order matters when using sensored. The vesc have no indication as to which phase wire goes where. Does anyone know how to find the right phase wire order for sensored vesc?
Also I plan to run in FOC. Does anyone have any experiences running FOC in sensored mode. That seems like double the risk. :scream:
```

---
## \#2 Posted by: Jinra Posted at: 2016-10-12T02:20:28.845Z Reads: 415

```
sensored phase wires only matter if you're not using the VESC. Once you plug in and do detection, input the correct hall sensor table and you'll be fine. Phase wire order only matters for direction.
```

---
## \#3 Posted by: Goombaacez84 Posted at: 2016-10-12T02:28:25.795Z Reads: 408

```
I don't know much about running a sensored motor aside from what benefits you gain from it. What I can say though is FOC seems to be hit or miss in general... I know lots of people have been successful with it (and I'm jealous), but I just burned out my DRV after 3 miles of riding FOC on my rspec. 

I think BLDC is the 'for now' long-term solution if you don't mind the roughness of it and don't want to take the risk. I'd be more than happy to find out ways to make FOC more successful though, because I sure loved that smooth acceleration and quiet start-up :grin:
```

---
## \#4 Posted by: Cisphyx Posted at: 2016-10-12T02:47:19.271Z Reads: 380

```
I run a sensored motor on FOC, it is very smooth. I've got a 230kv 6374 on a space cell (10S), probably pushing it a little bit . You definitely want the highest quality VESC you can get if you're gonna do that though. I blew up my first VESC from Enertion in about 10 minutes. I've been using a VESC from chaka for a couple weeks now though without issue, though I won't be surprised if it ends up blowing a DRV before too long as well. I also have a TB 12S ESC to fall back on if that happens though, which is reliable but nowhere near the smooth level of sensored FOC VESC.
```

---
## \#5 Posted by: Brando Posted at: 2016-10-12T03:07:27.648Z Reads: 360

```
How do I input the correct hall sensor table in? Can I just click the "measure" button in the "Detect hall sensor" section and apply? Or do I need to manually enter data?
```

---
## \#6 Posted by: Jinra Posted at: 2016-10-12T03:09:48.081Z Reads: 352

```
you run motor detection and it'll give you the hall table. Put the values in the hall sensor field. You can also hit apply and it'll do it for you.
```

---
## \#7 Posted by: Brando Posted at: 2016-10-12T03:23:42.206Z Reads: 344

```
Awesome thanks. Seems painless.
```

---
## \#8 Posted by: Plumb77 Posted at: 2016-10-14T01:38:16.330Z Reads: 321

```
Could you please explain what a foc is ? I have ordered a sensored motor from @JLabs and was planning on purchasing a vesc from enertion or torque boards will I have an issue? Thanks in advance
```

---
## \#9 Posted by: Brando Posted at: 2016-10-14T02:05:06.882Z Reads: 304

```
It's is basically a different way of sending electricity to the motor. It uses a smooth sinusoidal wave to switch between motor phases making the motor run quieter and smoother. Bottom line, it is a completely optional, and somewhat untested feature on the vesc that you need to manually setup. As shown by this thread you could run sensored motors on foc mode if you wanted. Here is a good article about foc: http://www.electric-skateboard.builders/t/vesc-faq-what-is-foc-field-oriented-control/419
```

---
## \#10 Posted by: Plumb77 Posted at: 2016-10-14T13:35:20.861Z Reads: 290

```
Would I need any additional plugs/adapter to hook up to the vesc or does the sensored Eire on the motor just plug right into the vesc
```

---
## \#11 Posted by: Brando Posted at: 2016-10-14T15:28:10.739Z Reads: 279

```
You do need a adapter for the sensor wire.
This one below is an adapter for torqueboard's motors. I would assume it would work for other sensor wires too, but I'm not sure.
diy-electric-skateboard-kits-parts/vesc-sensor-wires/
```

---

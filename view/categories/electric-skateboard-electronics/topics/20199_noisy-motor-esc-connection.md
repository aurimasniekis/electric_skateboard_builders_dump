# Noisy motor ESC connection

### Replies: 13 Views: 604

## \#1 Posted by: aha_96 Posted at: 2017-04-03T15:31:16.640Z Reads: 89

```
Hey so i had this issue with motor
```

---
## \#2 Posted by: Okami Posted at: 2017-04-03T19:47:56.053Z Reads: 66

```
To be honest, i partly think this might be because of the esc you use.. but if you know and have read that other people dont have issues with this esc.. then it might be something else..

Also.. in the first run you made.. it seemed like the sounds disappears when motor starts to spin faster..

so yeh.. i cannot really tell.. since I also didnt understand if 1st run is without sensors .. or both ''runs'' are in sensored mode
```

---
## \#3 Posted by: aha_96 Posted at: 2017-04-03T20:20:46.792Z Reads: 60

```
Yeah sorry about that. Actually, first run is sensorless. It makes some noise but I consider it "normal". Nevertheless, when I run it sensored it makes that weird noise, and I forgot to say, it comes from the motor. 

Thank you for replying
```

---
## \#4 Posted by: aha_96 Posted at: 2017-04-03T20:21:39.545Z Reads: 56

```
The thing that surprises me is the fact that, after searching in many forums, I haven't found anything like it
```

---
## \#5 Posted by: Okami Posted at: 2017-04-03T20:38:18.653Z Reads: 49

```
yeh im not 100% sure what the thing is.. i just remember a while ago someone also said that sensored car esc's not always work that great.. just dont remember about which car esc it was said.

maybe @Kaly can chime in, i think he has dealt with sensored motors a bit.. just not sure will he be able to help as u use car esc @aha_96
```

---
## \#6 Posted by: aha_96 Posted at: 2017-04-03T20:42:56.223Z Reads: 48

```
Yeah probably has to do with something like that. Either way I can run it sensorless, so it isn't a big issue. Anyways, I appreciate any help as I'd love to use it sensored.
Thanks a lot
```

---
## \#7 Posted by: Okami Posted at: 2017-04-03T20:43:58.681Z Reads: 46

```
yeh wait for some other folks to chime in, maybe update the title - car esc / your esc's model, so if someone also has it, so he can gain some interest in the topic.
```

---
## \#8 Posted by: filipandre95 Posted at: 2017-04-03T20:46:53.819Z Reads: 43

```
I think its because of the ESC. Consider getting a bigger ESC that is not made for RC cars.. or a vesc =)
```

---
## \#9 Posted by: aha_96 Posted at: 2017-04-03T22:52:11.173Z Reads: 37

```
If I had to do it again, I'd definitely get the VESC. Unfortunately that's not a possibility right now. So I guess I'll just run it sensored. 
Thanks for the input
```

---
## \#10 Posted by: aha_96 Posted at: 2017-04-03T23:17:09.309Z Reads: 34

```
*sensorless
```

---
## \#11 Posted by: Kaly Posted at: 2017-04-04T02:28:26.516Z Reads: 34

```
The problem with your motor and esc making noise when the sensors are connected is because of the order that the sensor wires are inserted into the sensor connector. 

What you need to do is first take notes or a picture of how the sensor wires are arrange into the connector. 
You will have 6 wires one  of each red, white, yellow, green, blue and black. 

- Now you are going to focus on the yellow, green and blue wires. This are the  phase sensor wires and need to be connected in the same sequence as the motor phase wires.  in order for the combo to work without that noise, which can kill your esc. 

- Next swap the position of any 2 wires form the yellow, blue and green. Then test the motor with the sensors using just a minimum throttle, if the motor do not jerk then you can increase the throttle input and you are all good to go. 

- if the motor jerks then by using the picture of the position of the wires, swap any other 2. You will have at least 3 combinations. 

- if this do not help with the issue then I can send you link to a 36 combination of the sensor wires and phase wires for you to find the correct one.
```

---
## \#12 Posted by: aha_96 Posted at: 2017-04-04T12:33:05.279Z Reads: 26

```
Wow awesome, I'll give it a try tomorrow morning and get back to you. Seems very straightforward. 
Thank you VERY VERY much
```

---
## \#13 Posted by: aha_96 Posted at: 2017-04-07T14:09:20.947Z Reads: 21

```
So I dedicated yesterday morning to it. Unfortunately, unsuccessfully. Made connectors for those 3 sensor wires and tried every combination possible. One combination, nevertheless, worked for about 20 seconds and then it started making the exact same noise again. So, for now, I live it in stand by. I have some exams coming up and want to focus on that. 

Thanks a lot anyways
```

---

# Which of these two motor is most suited for me?

### Replies: 9 Views: 279

## \#1 Posted by: grapplingdonkey Posted at: 2019-05-21T14:05:39.987Z Reads: 89

```
Hello,
I need some input on motor choice for my build.
I'm choosing between these two:
https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html 
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-213kv-brushless-outrunner-motor.html 
I have this battery:
https://eskating.eu/product/flat-10s2p-eskating-electric-skateboard-battery-30q/?v=7516fd43adaa 
and this ESC:
https://eskating.eu/product/electric-skateboard-speed-controller-maytech-based-upon-the-vesc/ 

Which motor, battery and ESC combo would be most logical?  Any help is greatly appreciated.
```

---
## \#2 Posted by: BigZwatt Posted at: 2019-05-21T14:06:59.887Z Reads: 76

```
![SEARCHGIFlookacrazycoolnotcap|640x360](upload://91D857RdjdvdTGB6mvtQIO8LBiU.gif)
```

---
## \#3 Posted by: grapplingdonkey Posted at: 2019-05-21T14:13:52.938Z Reads: 73

```
I know these types of threads are annoying however they are a great help to someone like me. I did try and search to see someone with the same set-up asking the same question but I didn't find anything. If you don't want to help you don't need to. @BigZwatt
```

---
## \#4 Posted by: MrDGOrman Posted at: 2019-05-21T14:29:39.609Z Reads: 68

```
Hey bro, welcome to the community.

I'd first like to apologise for @BigZwatt. I positively hate it when someone responds with "USE THE SEARCH FUNCTION" because I'll be totally honest - that doesn't return shit. Also, his response is not constructive at all and quite frankly a waste of everyones time and energy. So to reconfirm, ignore that tool.

Anyhow, back to the topic. First of all I'd always recommend going for a sensored system. The sensors allow for better diagnostics if you ever come into issues. It's just generally a better direction to go in. Providing the ESC allows for a sensored motor I would opt for that.

One thing that's worth noting is those KV ratings. The higher the KV, the faster you'll go, but sadly that means you'll lose out on torque and hill climbing ability. I have a 190kv motor from skating (6374) and that works a treat. I'd honestly recommend that you look at something between 150 and 190kv. That's going to be better all round for you.

I'll vouch for the motors you can get from eskating. They're bomb proof. I've had mine for over a year and it's been solid since the get go.

I hope this helps bro :+1:
```

---
## \#5 Posted by: grapplingdonkey Posted at: 2019-05-21T14:31:36.302Z Reads: 62

```
Thanks dude, I already have their battery and I'll look in to their motors. I also might need to educate myself on sensorered motors because I actually don't know all of their benefits except for better braking.
```

---
## \#6 Posted by: MrDGOrman Posted at: 2019-05-21T14:46:51.230Z Reads: 56

```
Sensored motors help with motor positioning, their temperature, braking, etc. It's just better for a ESC to understand where the motor is, what it's "doing" and how well it's performing. It'll add benefits like safety measures aswell. My board will reduce power if the motors get to hot. It saves them melting inside and dying a horrible death.

We've all been at your stage so be sure to ask any questions you may have. Drop me a private message if you need any advice :slight_smile:
```

---
## \#7 Posted by: BigZwatt Posted at: 2019-05-21T14:54:26.698Z Reads: 50

```
Im fully willing to help.  Wasnt meant to be a "tool" saw it as i was driving to work and didnt hace time to respond so i figured before i helped id pont ypu towards the search function.
```

---
## \#8 Posted by: Skunk Posted at: 2019-05-21T15:12:10.969Z Reads: 40

```
[quote="MrDGOrman, post:4, topic:94528"]
positively hate it when someone responds with “USE THE SEARCH FUNCTION” because I’ll be totally honest - that doesn’t return shit.
[/quote]

Maybe you don't know how to use the surch function correctly? 

[quote="grapplingdonkey, post:3, topic:94528"]
I know these types of threads are annoying however t
[/quote]

However there are threads dedicated to random questions and motor discussion. (You can find them with the surch function) 

It's not that people dont want you asking questions and to answer them. 
Ask all the questions you want.  Just don't start new thread for them. 
No one expects you to find every answer on your own.

That being said. Typically 200kv or under is what people aim for. 

If you get the low kv you can easily add more top speed with proper gear ratio.
```

---
## \#9 Posted by: rusins Posted at: 2019-05-21T15:39:47.067Z Reads: 31

```
The second motor is larger, meaning it can be safely used with a higher current, which gives more torque. (Motors usuallly have 4 numbers, the first 2 are its width in mm, the second are its length in mm)

However, the second motor also has a higher KV value: 213. This means that it will spin faster than the first one at the same voltage, meaning your top speed will be higher, but you'll have less torque.

At 10s battery voltage the latter motor will give you a theoretical max eRPM of 61740, which is just above the max your ESC can handle safely, so both are fine choices. I recommend using an esk8 calculator (http://calc.esk8.it/) to put in your pulley / wheel size values, to see which motor better represents the top speed you want to achieve.

Btw, first motor is much lighter, in case you care.
```

---

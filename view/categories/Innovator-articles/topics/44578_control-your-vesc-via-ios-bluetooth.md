# Control Your VESC via IOS Bluetooth

### Replies: 6 Views: 1209

## \#1 Posted by: ZackoryCramer Posted at: 2018-01-24T23:48:45.032Z Reads: 178

```
Hello! I recently finished the basic model of a VESC addon that can connect to an App I created using Bluetooth. All you have to do is just connect the model into VESC's UART port and fire up the App and connect. I am planning to finalize the system and sell the module and app as a kit.
Tell me if this is something I should keep pursuing.
![2018_01_23_IMG_0158|281x499](upload://9Zjh3S2gwt9OlPE3902hqmIAmlW.jpg)
```

---
## \#2 Posted by: Sirshaunsta Posted at: 2018-01-25T21:30:08.152Z Reads: 149

```
I like this idea, especially if you can optimize options like throttle and braking curves, max volt and or amp draw settings etc.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2018-01-25T22:13:26.430Z Reads: 140

```
No offense but I think that's a terrible idea. A smartphone is the wrong device to control the power. And i see the risk that beginners would safe the money for a propper remote because they think the iPhone can do everything.
Would be easy for me to add that feature to my app but that would be very ruthless.
```

---
## \#4 Posted by: raz Posted at: 2018-06-15T22:58:08.187Z Reads: 91

```
[quote="Ackmaniac, post:3, topic:44578"]
the power. And i see the risk that beginners would safe the money for a propper remote because they think the iPhone can do everything.
[/quote]

I agree with Ackmaniac. The one thing you do not want to cheap out on is the way you control your esk8.
A smartphone is just too unreliable for speed control as any app, there are quite a few things that can go wrong. Just to name a few potential problems that may arise:
- Loss of bluetooth connection because of an OS bug (the sole reason why I hate bluetooth)
- Accidentally pressing the lock button while riding
- The app may crash or lock up because of the OS not being optimized properly (Chinese phones, custom roms, etc.)
- Input lag / transmission lag
- Popups/Notifications on the phone such as Facebook Messenger. You could accidentally tap the wrong icon and suddenly you are unable to control your board while riding at a high speed.
- Memory overflow

The best way to be safe is to make the control system as uncomplicated as possible. There is a saying that goes: "more code, more bugs." And there is a lot of code involved in smartphones.

Unless you are an experienced esk8 builder, know your phone really well and have a lot of smartphone app development experience, do not do this. It is life threatening.

If you are going to pursue this make sure that the receiving end has code implemented that checks if the smartphone is responsive every ~15ms. If it detects that the phone was not able to respond in 15ms then the whole system must disengage (no braking, just 0% throttle).  Also limit the speed to ~18 km/h and test it out for a few months. That's my 2 cents.

Again, I cannot repeat it often enough: this is a dangerous project.
```

---
## \#5 Posted by: cryo Posted at: 2018-06-16T03:06:36.047Z Reads: 70

```
have to agree with @raz @Ackmaniac here. A phone isn't the best choice of remote, can you imagine trying to use a note 8 in one hand while riding?
```

---
## \#6 Posted by: Dimotro Posted at: 2018-07-16T16:39:53.046Z Reads: 50

```
It isn't the best choice, but for me currently with a broken remote it would be nice to at be able to have this feature. Not that i would go full throttle on a smartphone, but for low speeds i don't see the issue even if it fails now and then.
```

---

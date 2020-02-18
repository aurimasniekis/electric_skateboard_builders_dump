# Weird Signal Issue

### Replies: 10 Views: 765

## \#1 Posted by: AbrownMN Posted at: 2016-06-23T00:31:03.393Z Reads: 83

```
So, I had a really nice ride around today and when I got back home I flipped of my mini GT2b remote and as soon as I flipped in off my motors started ramping up to full speed. Why on earth would the signal start upon turning OFF the remote? Sketchy. Anyone got an answer to this?

I have also had an intermittent issue where they just sort of glitch(ily) move after coming back from a ride. Am I getting interference or something?
```

---
## \#2 Posted by: AbrownMN Posted at: 2016-07-10T16:13:39.380Z Reads: 43

```
Still having this issue, can anyone offer some advice? If I turn it on from cold just laying on the table motors up it doesnt have the issue. If I grab the board and shake it or tap it on the table a bit roughly the signal starts getting sent in a glitchy manner to the motors. After this happens, if I am to turn the remote off and leave the battery pack on they will shoot immediately to full throttle. With the remote completely off how is it that signal is still being sent?

Edit: In the real world application, as soon as I hit a few bumps on the road ( simulated by my tapping it on the table) I can hear the signal trying to send in that same glitchy manner to the motors even when I am just coasting.

I will put up a video if what I am saying makes no sense.
```

---
## \#3 Posted by: TheWrongHombre Posted at: 2016-07-10T16:56:50.325Z Reads: 41

```
@AbrownMN

I have a similar issue. When I turn off the remote, the motors go to full throttle.

I haven't tried debugging the issue since it hasn't been a big deal. Would be nice to understand why it's happening though...
```

---
## \#4 Posted by: AbrownMN Posted at: 2016-07-10T17:22:07.137Z Reads: 36

```
Yeah, that's not a huge deal. Still sketchy if you ever somehow managed to turn it off while riding and didn't catch it right away. Could injure yourself or send your board into the water if you ride a path next to a little river like I do pretty often. I am more concerned with the random glitchy signal being sent while I am just trying to coast. It's chirping and annoying and probably not great for the board. Would love any advice I can get. Could it be some other device in the case interfering somehow? It's not environmental interference as I have repeated it in multiple rides and parts of my house.
```

---
## \#5 Posted by: AbrownMN Posted at: 2016-07-10T17:24:08.308Z Reads: 38

```
Just read something online that says it's probably a reversed channel or some setting in the VESC programming..I'll have to tinker with that. I'll let you know.
```

---
## \#6 Posted by: elkick Posted at: 2016-07-10T17:34:29.543Z Reads: 37

```
You need to activate faile safe, then it won't happen again. 
Just google it for gt2b, there are some YT tutorials around.
```

---
## \#7 Posted by: lox897 Posted at: 2016-07-10T21:50:24.809Z Reads: 33

```
Not sure if this helps, my board had an issue where one of the capacitors on the UBEC was smashed. Whenever the UBEC got smashed around (When I hit a bump) the board would start beeping and the motors would stop responding. If you have the VESC, have a look at the 5v power supply.
```

---
## \#8 Posted by: AbrownMN Posted at: 2016-07-12T14:29:30.040Z Reads: 30

```
Thanks for the tip! I did hear something about that, but assumed my controller wasn't sophisticated enough. Just figured that was for the super nice GT2b's with the screen. I am assuming it's just something I'd have to configure in VESC programming?
```

---
## \#9 Posted by: AbrownMN Posted at: 2016-07-12T14:29:41.660Z Reads: 29

```
Thanks, I'll pop it open and take a peek.
```

---
## \#10 Posted by: elkick Posted at: 2016-07-12T17:04:53.387Z Reads: 24

```
I'm abroad currently, so just a short answer: I have made a short tutorial for the mini remote fail safe function on my homepage (esk8.de, tutorials), it's for the Mini remote, but that's a similar receiver like the gt2b.
```

---

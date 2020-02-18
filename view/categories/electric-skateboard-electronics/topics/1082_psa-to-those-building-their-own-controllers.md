# PSA to those building their own controllers

### Replies: 8 Views: 1541

## \#1 Posted by: Sharkface Posted at: 2016-01-23T20:10:59.354Z Reads: 74

```
https://www.youtube.com/watch?v=cCgZAo5JECs

So this is obviously a little situational as you would have to go past somebody who was specifically looking for a boosted board. Or a GT2B (which doesnt this guy frequency hop or something?) might be another example since its so widely used. Regardless, you would have to simply go past the wrong person and boom, bye bye board.

The only thing needed to stop this was a simple layer of encryption. For example, this website/forum doesn't use SSL. All I need to do is find a way to sniff the traffic coming to the server and I would be able to get everyone's password from this site (assuming that there are no layers in between me and that server, IE cloud flare).

As you are building be considerate of the users that you are giving parts to. If your controller gets so popular that you have multiple revisions, maybe its time to go that extra mile and add every possible safety feature. Safety features like redundant signals, encryption layers, so many possible things could be done

Its a modern world out there people... we are not as protected as we often think. Ride Safe, Ride Hard, and Ride Respectfully. 


P.S.: if we wanna get a group buy going on an SSL cert so we have that layer of encryption I can arrange/install that with ease.
```

---
## \#2 Posted by: chaka Posted at: 2016-01-24T01:43:03.358Z Reads: 61

```
AFH vs FHSS. AFH is vulnerable but the GT2B is FHSS and not easily hackable. AFH or otherwise known as bluetooth is what is used on the boosted board.
```

---
## \#3 Posted by: torqueboards Posted at: 2016-01-25T01:34:21.104Z Reads: 49

```
Yeah, it's because boosted is bluetooth. Doubt you can have the 2.4ghz like you can with the bluetooth or as easily.
```

---
## \#4 Posted by: Sharkface Posted at: 2016-01-25T03:20:58.177Z Reads: 48

```
Yeah bluetooth is going to be a lot easier because the standard is setup and in place. So with the standard in place you can just use frameworks to actually communicate over the bluetooth signal. With the framework being used as a programmer all you have to do is actually put a bit of encryption in place... then the real problem is actually figuring out how to decrypt it very fast when received by the board. Or you can just frequency hop or some crap.... 

iiidddkkkkkkk def need to look into it more and shit
```

---
## \#5 Posted by: longhairedboy Posted at: 2016-01-25T18:52:24.131Z Reads: 45

```
right now the only hacking that happening on my signal is the wifi making my motors tick while the board is charging. 

@cmatson and I have both experienced this. We have both seen it happen, and have both made it stop by leaving our remotes on while the board is charging. In his case it was the GT2B doing it, and in my case it was the Steez doing it. 

It happens any time power is applied to the system (on or just charging) and the remote is OFF and not providing a clear and powerful signal to drown out any surrounding 2.4 GHz noise. Our house is flooded with Wireless G still due to legacy devices. 

So honestly I'd be more worried about broad high amplitude noise attacks on that frequency band that drown out any useful signal and cause uncontrollable chaos than i would be about direct street facing attacks via targeted signal injection.
```

---
## \#6 Posted by: sk8ace Posted at: 2016-01-25T20:00:49.810Z Reads: 39

```
It's interesting for sure but highly unlikely anyone will ever be "hacked". There's no point to it besides making someone fall off. 

Should manufactures add encryption? Probably.
Will they? Not likely. 

Like others have said, I'd be more worried about noise and interference. 


This forum uses Discourse and passwords are encrypted. Adding a second layer isn't really necessary. You can't get plain text passwords by doing a man in the middle attack. Best bet would be a session hijack. Even still, no one keeps their personal info on here so attacking would be fruitless.
```

---
## \#7 Posted by: Sharkface Posted at: 2016-01-25T22:45:03.017Z Reads: 37

```
[quote="sk8ace, post:6, topic:1082"]
Should manufactures add encryption? Probably.Will they? Not likely.
[/quote]

so sad, so true :frowning: 

[quote="longhairedboy, post:5, topic:1082"]
It happens any time power is applied to the system (on or just charging) and the remote is OFF and not providing a clear and powerful signal to drown out any surrounding 2.4 GHz noise. Our house is flooded with Wireless G still due to legacy devices.
[/quote]
That explains why I was getting the same issue you describe but it stopped when i moved.
```

---
## \#8 Posted by: RunPlayBack Posted at: 2016-01-27T04:08:58.371Z Reads: 32

```
This is a great topic and something I brought up to with a few security researchers that I work with. Most of them are pretty excited about my DIY build and we're always looking for video concepts that involve debunking some kind of hacking myth or experimenting with attacks. One idea was how to protect an electric board from hackers. Coincidentally, I was just on an email chain with Mike Ryan (dude with the short hair who hacked the Boosted) who saw my build article. I shared with him all the various remotes that are available for DIY and he seemed interested in seeing which ones would be the easiest to jam. Either way I'll probably be producing some kind of security/eboard related soon and share it here.
```

---

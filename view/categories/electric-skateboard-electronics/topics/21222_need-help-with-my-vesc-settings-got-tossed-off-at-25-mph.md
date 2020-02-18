# Need help with my VESC settings, got tossed off at 25+ mph

### Replies: 18 Views: 1375

## \#1 Posted by: Mattmccrary8 Posted at: 2017-04-17T17:23:40.550Z Reads: 220

```
Ok so I completed my first build and it's a dream come true until I got thrown off at 25mph and ate shit. Luckily I only have a few scraps but my brakes have been skipping as well. I'm assuming their most be a lot wrong the my VESC settings. 

I weigh 195lbs

Motor TB 63 190kv
TB VESC BLdC
36t 16t pulley 15mm belt
2.4 ghz nano remote 
2x 5s 5000mah batteries in series to make a 10s setup 

<img src="/uploads/db1493/original/3X/9/4/942e42d56a2b2faddc9a024a2cc28166a9708a97.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/b/f/bf0b8ae15251889dd43a4f89ec319e19480349aa.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/f/6/f63634d77aac336615bcc90959a4f3d1374467bf.JPG" width="666" height="500">
```

---
## \#2 Posted by: Titoxd10001 Posted at: 2017-04-17T17:38:34.973Z Reads: 206

```
That remote has known reliability issues I personally wouldn't risk injury using it. Also your pulsewidth looks a little off, usually it displays percentage and should be exactly in the middle at 50%. Then test failsafe (neutral when connection is lost) is working, turn off the remote and the pulsewidth should stay at exactly 50%, if not you would have to adjust it
```

---
## \#3 Posted by: Mattmccrary8 Posted at: 2017-04-17T17:50:08.893Z Reads: 201

```
So what about the random breaking at full speed? Can I shit that off? And how can I prevent belt skipping? Notice anything wrong in my settings?
```

---
## \#4 Posted by: Titoxd10001 Posted at: 2017-04-17T18:03:40.302Z Reads: 197

```
Again check your pulsewidth to make sure it's dead center when controller is on and off. If there is no issue with that then it might be your controller.

Make sure wheel pulley is perfectly centered and you want to ease into brakes as much as you can. Is your motor pulley aluminum or steel?
```

---
## \#5 Posted by: jaykup Posted at: 2017-04-17T18:03:56.836Z Reads: 188

```
+1 for controller issues.  Pulsewidth looks weird.  failsafe likely not setup correctly.

Short term: set your failsafe to neutral instead of full brake - the controller is probably cutting out while riding and "failsafing" to brake.

Long term: Would recommend a GT2B with a 3D printed housing for better reliability.  Like the Baby Buffalo and Mad Monkey mods.  Both are really good, but I'm starting to like the Buffalo a lot better lately.  Less chance of accidentally grabbing a handfull of throttle when you aren't expecting it.
```

---
## \#6 Posted by: Guacamoleface Posted at: 2017-04-17T18:12:06.227Z Reads: 178

```
If your board is on and it has brake on wheels(with remote off) then your failsafe is wrong. You need to fix this with rebinding your remote to receiver.
And when remote dropped connection it brake and threw you off. 

If it rolls freely this most likely wont be the issue.  
So try check with board on and remote off if it brake while remote is off.
```

---
## \#7 Posted by: Mattmccrary8 Posted at: 2017-04-17T18:26:45.999Z Reads: 162

```
That's exactly what happened my board locked up and threw me flying, when I get home I'm going to rebound the remote. What about belt skipping?

Should I tighten the belt in this case so it doesn't skip because it only does it on brakes, not acceleration
```

---
## \#8 Posted by: Mattmccrary8 Posted at: 2017-04-17T18:27:33.174Z Reads: 155

```
I think it's aluminum, I got everything from DIY TB
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-04-17T18:35:37.393Z Reads: 150

```
If it's aluminum it will be really light, if it's steel it will be heavy. Aluminum brakes down super quick, did you have belt skipping problems when brand new? Steel last longer that's why I got some custom made and have them for sale, I have 15t
```

---
## \#10 Posted by: Guacamoleface Posted at: 2017-04-17T18:38:06.822Z Reads: 143

```
Just try start your board without your remote on, and try and see if it rolls or is keeping full brake.
preferly before you rebind it if so you know that is the issue for sure.

The remote itself is unreliable - Im in the same boat as you when it comes to that. I feel a tad more comfortable with it now that it doesnt full break on disconnect. But Im going for a new controller. Mine disconnects every now and then.

About the belt, do you keep yours loose? I keep mine tight, but not super tight. I can tell that I had some skipping by looking at my pulley. but nothing I've noticed. Im 75kgs(165lbs ish?) so not to heavy though.
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-04-17T19:01:09.262Z Reads: 135

```
that nano.. is that basically a repackaged Winning? The only time i've ever been thrown was because of that remote.
```

---
## \#12 Posted by: mmaner Posted at: 2017-04-17T19:07:36.431Z Reads: 132

```
Mount the truck clamp tight, mount the motor mount tight, mount the motor loose. Then pull the motor as far out you can while pushing down the belt 3/8s of an inch (make a tiny dot with a sharpy) the tighten the motor mount screws.
```

---
## \#13 Posted by: yaca Posted at: 2017-04-17T20:10:46.316Z Reads: 124

```
If you really want to use the Nano remote at least failsave should be in neutral 50%. You can check it on the bench with BLDC Tool. Look at the green (in your case blue) bar (Display on), give throttle - stay - turn off the remote. The green (or blue) bar has to go to neutral 50% - no brake no throttle. 
Btw. I can not see the percentage next to the blue bar, is it not visible in the Mac Version of BLDC Tool. You better change to ackmaniacs 2.54 Version, it's much better.
Beside of the correct pulsewith the nano remote has a throttle trim to adjust the neutral 50%.
```

---
## \#14 Posted by: Mrmoonlight Posted at: 2017-04-17T20:25:05.971Z Reads: 122

```
Check out the Benchwheel Remote. Very reliable and similar to the Winning.
```

---
## \#15 Posted by: mmaner Posted at: 2017-04-17T20:27:51.314Z Reads: 124

```
https://www.electric-skateboard.builders/t/remotes-commercially-available-options/15162
```

---
## \#16 Posted by: JLabs Posted at: 2017-04-17T20:29:32.632Z Reads: 122

```
I have some mine remotes left in stock. Arguably the most reliable controller on the market, next to the GT2B. It's small and slides right in your pocket, and you can remove the wheel if you wish. This will fix your issue and give you a lot more confidence when riding. 

https://electric-skateboard.market/product/2-4ghz-mini-remote-receiver/
```

---
## \#17 Posted by: BigBoyToys Posted at: 2017-04-18T03:20:19.042Z Reads: 99

```
+1 on rebinding the remote and that remote having intermittent connection issues. I haven't had issues with it since adding a ferrite ring though. I still use that remote on my 6000w 4wd hub board lol.
```

---
## \#18 Posted by: Kso79 Posted at: 2019-06-10T06:55:18.116Z Reads: 19

```
I bought 2 3,000W motors for my newish evolve gtx. I’m going to swap the motors next week. Any suggestions of what could go wrong.
```

---

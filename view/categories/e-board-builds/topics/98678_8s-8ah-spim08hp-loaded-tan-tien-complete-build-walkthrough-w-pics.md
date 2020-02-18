# 8S 8Ah SPIM08HP Loaded Tan Tien Complete Build Walkthrough w/pics

### Replies: 9 Views: 540

## \#1 Posted by: Brad99 Posted at: 2019-07-18T01:38:57.428Z Reads: 125

```
TLDR; I built a practical, cheap longboard and wrote about it. You don’t need any fancy expensive tools or parts to build one, and you should be having fun even when stuff starts to break. I imagine there are tons of people who want to build one but don’t think they can, you should just send it and build one anyways. Also, wear a helmet dumbo.
 
Please ask questions about anything and everything I’d love to answer them. There is no way I could have covered every little detail.
 
Let me preface something; tools. You do not need any fancy tools to completely make an electric longboard from almost scratch. The most advanced tool I had for making my motor mount was a drill, some files, and an old hacksaw. My soldering station was literally a wood-burning tool paired with some plumbing flux and plumbing solder. I did end up buying a rotary cutter to cut out the fiberglass enclosures for < $25, and a small tap for taping holes in the drive pulley. The only tool I feel someone would “need” to make the battery pack is a decent multimeter with continuity function, you’ll use it all the time.

![hacksaw|666x500,75%](upload://3OkJNBSWfPicsr5T2alZwO77uKw.jpeg) 
 
Abstract / Background: As of completing the build I am a rising senior Electrical and Computer Engineering student at a large University (both people and area wise) in New England. My goal/requirements was to have cheap (<$350, I’m a broke college student), fast-ish and long-ish range board to get around campus whenever the seasons/weather allowed. However, before building I made sure I was flexible with the goals and was willing to go over budget and change (or upgrade) the requirements as need-be. However, I do have access to a very high-quality maker space/electronics design lab at school with anything I would ever need because if my major if anything happens to break on it, or if I were to upgrade it while at school.
 
Board: (in my opinion the most important part) This was the most expensive part by far, I went with a Loaded Tan-Tien Flex 3 with bear trucks and 70mm wheels purchased used for $105. My reasoning behind this was that I already have some longboarding experience, I love riding them and wanted to be able to easily convert it back into a regular non-electric longboard so I could cruise around on it with my own leg power (Woah), so I would not be drilling into the deck or trucks whatsoever (I drilled into the wheels but those are cheaper). The original plan was to keep it as a drop-through deck which ultimately did not happen. I thought that there would be enough clearance between the battery/ESC enclosure (will talk about the enclosure later) and there was, in fact, enough clearance. However, this deck is a very flexible deck and I wanted to be able to jump up and down on it, send it off large curbs and over cracks without having to worry about scratching it too much. So I made the decision to “un-drop” through the deck. Now it feels sort of like a surfboard and I actually really like it, I guess you could say it feels almost identical to a boosted board (almost the exact same deck now).

![deck2|666x500,75%](upload://siFZTevLDtVplRX8Vw6LDsg79yP.jpeg) 
![deck1|666x500,75%](upload://e5yfgXUjLdfrb7Ghd5vf0aGn3MM.jpeg) 
 
Motor Mount: This has nothing to do with electronics, but I still wanted to make it myself. While this was monetarily the cheapest component, it took the longest to get right and has the most blood sweat and tears poured into it. If I had a CNC or some more specialized tools I believe I could have gotten it done quicker, but I’m proud of how I did it.
 
Made from a 2 X 1/8 X n” aluminum stock bought from a hardware store for under $10, I bent it along a 45-degree angle by heating it with a blowtorch, putting it in a vise and hitting it with a big hammer. The only other tools I used was a hacksaw, drill and a couple of different sized metal files. The design should be fairly obvious by looking at the pictures below. 
![mount1|375x500,100%](upload://3S7QLGowm8GyeS43VP1D7gHYIYj.jpeg) 
![mount2|666x500,75%](upload://bH7p6iXfF5BJ8mq0GlOjpZDLHvd.jpeg) 
![mount5|375x500](upload://iI1Tm9ldlFnsGtJ826MZU7lGMhx.jpeg) 


To help with the belt slipping that I experiences, I ended up adding an idler (actually two in the end) made with a screw, some nuts, washers, and three bearings off a pair of old skateboard trucks. This helped immensely and the belt barely slips anymore. Another note: I ended up essentially building a second mount and bolting them together into one 1/2in thick aluminum mount. Before this I noticed some flex, now it is solid as a rock.
 
![idler|375x500](upload://1iTlOVm966zGgs1KD2fesdJgKlE.jpeg) 

Batteries: Arguably the most important part of the electric system, I decided to make my own battery “pack”, but I did not use 18650’s like most others. Instead, I went with SPIM08HP cells (3.7V nominal, 4.2V max, 3.2V min, 200A discharge, 8AH LIPO).
 
My reasoning in picking these batteries instead of 18650 or premade lipo batteries:
1. No need for parallel cells, 8 amp hours will be plenty for my desired range.
2. They are flat (easy to mount/build)
3. No spot welder needed
4. They look cool
 
I originally purchased six cells for a 6S battery with BMS for charging and without BMS for discharge (I ended up upgrading to eight cells for an 8S battery to make it faster )
![6cell|666x500](upload://fM6svzJVj839Nxm7uE6j4ZuJqHf.jpeg) 
 
I used a fairly cheap no-name BMS from eBay for charging, and no BMS for discharge. Under-voltage shutoff would be done by the ESC, over-voltage charging shutoff would be done by the 25.2V charger (I would later change this to a 33.6V charger for the 8S battery), and the BMS would balance charge the pack as a whole.
 

![batt1|375x500](upload://bYAvr2d0bQNYR1wXXN0ifeZVlko.jpeg) 


Connections and anti-spark: To connect each cell together, I used an old leather punch to make holes in the metal, then used some random machine screws and nuts together with some small aluminum washers. To connect the 10 AWG wire to the cell I did A similar thing with the leather punch on the cells, but stripped away part of the wire in two places and ran a machine screw threw the metal with an aluminum washer on top and a random nut on the bottom, so far it is still holding just fine. I am also using an XT-90 antispark as a sort of “key”, with the female connector sticking out of the enclosure attacked with hot glue. I originally had three cells in the front and three in the back, now with the 8s set up I have four up front and four in the back.
![2019-06-03_19-21-34_920|666x500](upload://4gnF1b8uACn4fIiMyLRFKIpQMwI.jpeg) 

![outside|666x500](upload://9BvlDTPvCOqFS8BoNPIEC3s7J8b.jpeg) 

 
ESC: This is the only main component I did not make, I purchased a cheap brushless ESC with a controller on eBay for ~ $40. If you know about electric skateboards, then you probably know about the VESC, and it is probably something I will upgrade to when the cheap ESC I am currently using eventually and inevitably breaks/burns out.
 
Motor: Using a single C6374 170 kV brushless motor I got on eBay for ~ $50 after shipping. I have no complaints with the motor other than the 10mm D shaft can be tricky to connect to. Make sure to use Loctite (blue, NEVER red) on the motor mount screws, mine never fell off but it did loosen enough the first time so that the belt almost came off.
 
Driving/Driven pulley(s): Let me preface this by saying that I have access to a 3d printer which I built a couple of years before my longboard. While it is an older DIY printer and can be a bit finicky, It can print with some very good quality, rivaling some of the new $1,000+ printers on the market today (2019).
 
My goal was to print both the driving and driven pulley, try to guess which one didn’t work before reading (think more rotational velocity equals more friction over a given time)
 
Driven (wheel) pulley: 32T 15mm printed in PLA, took a couple tries to get it correct, no major failures just simple printing errors. Even though PLA is a fairly low-temperature plastic it’s still working after over 50 miles.
![driven|666x500](upload://maA7DEigcedhwJUOtOZkgYqB4aJ.jpeg) 
![drivenbelt|666x500](upload://lHiOzKc92OUnLxSEYPnYFfY6AEH.jpeg) 
Driving (motor) pulley: 15mm 5HTD 295mm Belt
 
#1 Originally printed a 16T PLA pulley (*Note*, this is the exact same material printed in the same way as the wheel pulley), had to use a file/Dremel to get it to fit correctly on the 10mm D-shaft of the motor. The pulley component worked great while testing for the first 50ft, then melted and the belt fell off… lesson learned
 
#2 Printed the same STL file, the only difference was that I used ABS plastic (supposedly higher temp). Worked great for the first 50ft, then snapped in half. Turns out that I only printed with 60% fill. (pic 3.)
 
#3 Printed same STL file, same ABS material, the only difference is that I now printed 100% fill. Worked great for the first 75ft (improvement!), then snapped in half. I came to the conclusion that this ABS is of very cheap quality.

Red (left) is ABS before it broke, white (right) is PLA after melting
![drive|666x500](upload://7Y9o9pT6mjfj0BhLvNyrzD9ssvt.jpeg)  


*Note* The ABS came from china and was very cheap, the PLA, on the other hand, was a slightly more expensive and a more high-quality material. They both have their uses, this just wasn’t the cheap ABS’s proper use.
 
#4 I finally came to my senses and bought a cheap < $5 aluminum 14T 15mm pulley, with an 8mm round bore. This doesn’t even come close to fitting the 10mm D-shaft on my motor. So I first drilled it out with a 3/8 in (9.525mm) bit because that was all I had and attacked it with a round file until it fit snugly around the shaft. I then drilled, tapped and put in 3 small set screws into the aluminum low enough so they would not touch the belt while turning. This has been working for over 50 miles.
 
![drivvee|666x500](upload://aT1mlJkZBFlX4zgI2bWC6eDLTxX.jpeg) 

Battery and ESC enclosure: This is one of the reasons that I got these flat battery cells, they could be easily placed into two separate enclosures each containing what was originally three cells, but now four. I originally planned on using some sort of x2 sandwich enclosure, but I couldn’t find the size I wanted at a reasonable price. I had some leftover Bondo fiberglass cloth and resin from repairing our sunfish (sailboat) the year before, so I fabricated a custom case from some molts I quickly made. The molds were just 2 2x4’s duct-taped together that I attacked with an aggressive low-grit belt on a handheld belt sander until they were the right shape. I then wrapped it and the longboard deck in plastic (saran) wrap and coated it with what I think was olive oil (that was all we had in the kitchen) so the epoxy resin didn’t stick to it.


Note this picture is BEFORE raising the deck while it is STILL drop through, it is not this low now.
![encccc|666x500](upload://p9MV6HocdLR0RaDrGr62IGYgVCz.jpeg) 


 
After it was cured I cut it out with a rotary cutter and cutoff wheel I got from harbor freight for ~ $25. I tried to attach it with some “industrial strength” Velcro, however, it wasn’t strong or flexible enough to counter the flex of the deck. With some straps holding it to the deck, the Velcro does a great job to keep the enclosure from sliding around.

 
Prototype and test (breaking stuff): This is the best part, a friend once told me “it’s the most fun that you never want to have again”. There were many hurdles that didn’t quite fit into any of the categories listed above, here are just a few of them:
 
 Obviously, you don’t want to be four miles away from your house/work/class and have your skateboard completely fail. The solution to this is to stress test it many times with extreme situations. For me this meant many full accelerations, emergency braking, going off jumps, and simply testing everything till a lot of it inevitably broke (eg. All the drive pulleys).
 
TIPS
1. R.T.F.M: Read the “freaking” manual, or in this case datasheet. When I installed the new 8S BMS (technically 3-10s) I wasn’t able to read any voltage off of the output and thought the one I received was faulty. Turns out I was the fault, and I simply wasn’t using the correct connections…
 
Upgrades I am making:
I currently am adding some WS2812B individually addressable led strips on the back, they will be flashing red at night and possibly some other lights on the rest of the board. The reason they are not on the board right not is that I accidentally burnt out my Arduino Nano by setting a buck converter powering it to the wrong voltage.
 
I also need a better way to attach the enclosure to the deck, I will not drill into the deck. I may use modified straps of some sort, or make my own binder clip like clamps. Not sure yet.
```

---
## \#2 Posted by: Brad99 Posted at: 2019-07-18T01:42:10.544Z Reads: 94

```
![2019-07-17_20-35-46_499|666x500](upload://3D4XuTIXguasOHaeJRaYUeAxorJ.jpeg) 
![2019-07-17_20-36-09_690|375x500](upload://8hT9AF2gVwHyWBFGm1CP0VO3xud.jpeg) 
![2019-07-06_11-12-19_700|666x500](upload://dW5rrBM4K4tP8WFkzg5Yi6GOUs9.jpeg) 
![2019-06-20_21-16-59_014|375x500](upload://eNOaRAeNoQniGUzXx0sUiw3jGw.jpeg)
```

---
## \#3 Posted by: AlanZhou Posted at: 2019-07-18T03:11:18.617Z Reads: 88

```
[quote="Brad99, post:1, topic:98678"]
*Note* The ABS came from china and was very cheap, the PLA, on the other hand, was a slightly more expensive and a more high-quality material. They both have their uses, this just wasn’t the cheap ABS’s proper use.
[/quote]

 printing the motor pulley is not a good idea, no matter what material you use, unless you have a metal 3d printer.
```

---
## \#4 Posted by: murdomeek Posted at: 2019-07-18T07:25:51.668Z Reads: 72

```
dang, this is the ghettoist build i've come across in a longg time

Be safe riding bro!
```

---
## \#5 Posted by: Wilsonliang777 Posted at: 2019-07-18T10:03:45.186Z Reads: 71

```
My first built was like this 3 to 4 years ago.  Diy electric skateboard came a long way.most  Pls be safe.
```

---
## \#6 Posted by: Brad99 Posted at: 2019-07-18T12:41:31.896Z Reads: 61

```
I still have faith in it, I have some nylon filament I'm going to try next. Just need to dry it out first
```

---
## \#7 Posted by: trainingforutopia Posted at: 2019-08-09T19:46:00.760Z Reads: 36

```
@Brad99  I love your build! I am shooting for something similar, also with a Tan Tien, but flex 2 board. Do you see any viable way of keeping it dropped through? I am thinking about using a chain to drive it and over-mounting the motors in the back.
```

---
## \#8 Posted by: Brad99 Posted at: 2019-08-12T13:37:05.204Z Reads: 26

```
@trainingforutopia I almost over-mounted the motors on the back, but the only reason I did not was I still wanted to be able to kick up the board with the tail. If you mounted the motors behind the wheel, and made the enclosure just a little bit thinner, I don't think there would be a problem with clearance at all.
```

---
## \#9 Posted by: trainingforutopia Posted at: 2019-08-12T17:45:40.381Z Reads: 23

```
Thanks! Yeah, I also would like to kick it still. I thought, that if you mount the motors totally vertically, then you still have the kick free. So you could set your foot behind the motors and kick it. With some kind of protection for the motors/belts there should work. Or is that over-engineering? Might be better off just going DD or Hub drive.
```

---

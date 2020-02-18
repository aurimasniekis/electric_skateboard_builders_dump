# The First Try &#124; homemade deck &#124; single SK3 6374 &#124; VESC 4.12 &#124; Benchwheel remote &#124; 10s LiPo &#124; Caliber II &#124; Flywheels

### Replies: 10 Views: 1239

## \#1 Posted by: Jaydan Posted at: 2017-06-19T12:23:32.907Z Reads: 145

```
####UPDATE NO.1: [post #9](https://www.electric-skateboard.builders/t/the-first-try-homemade-deck-single-sk3-6374-vesc-4-12-benchwheel-remote-10s-lipo-caliber-ii-flywheels/25689/9?u=jaydan)
---
####ORIGINAL FIRST POST:

hey,

after being inspired by casey and terrified by the price of a boosted board, i decided to build my own electric skateboard. 
being a student on a budget, i want to keep the costs down. however, i figured that saving on the electric components is not the brightest idea. i will try to save money on the skateboard parts. this means, that i will borrow the deck, trucks, wheels, and bearings from a friend of mine and if everything works out well, i will eventually buy my own stuff. that way i can minimize the financial risk and still get a good board.
so far, i've done quite a lot of reading and came up with the following parts:

-VESC 4.12
-Turnigy SK3 6374 192kv
-Benchwheel remote
-2x Turnigy or Turnigy 5S 5000mAh 20C battery in series
-15:36 transition on a 15mm belt
-90mm flywheel clones (the wheels i will borrow are 76mm or at least they used to be, they are a lot smaller now)
-Caliber II 50° Trucks

i already ordered the VESC and the motor pulley and am in the process of building the motor mount.

actually, i didn't want to spam this great board with another first-build-advice-seeking thread, but i couldn't justify spending all the money without having someone at least taking a brief look at my part list. if you want to, i will try to convert this thread and document the build as soon as i get all the parts and enough time to build the board.

two further question regarding the c-rating. the theoretical max discharge of the battery would be 100A. regarding the specs on hobbyking.com, the motor has a max current of 80A.
1. should i limit the current in the VESC's settings to 80A?
2. what would happen, if the VESC/motor pull more than the max 100A? does the c-rating mean, that the battery will limit the current to the 100A (in this case) or is it more like that the battery can supply more than the 100A, but going above this value will damage the battery?

thanks mates!
```

---
## \#2 Posted by: Alanhunt123 Posted at: 2017-06-19T13:01:13.012Z Reads: 128

```
Hi Jaydan,

Congratulations on starting your first build! Your parts list seems good. 

The VESC is rated for 50A from the battery. I would set your battery max current somewhere around 40-45A, which will give you plenty of punch at the top end on 10S. As for motor current, you can set that to 80A, and have no issues. For a little more low end punch, you can try increasing the motor current. I've seen people on this forum use the full 240A! However, I can't recommend going much over 120A.

This may seem a little confusing, since you would think that motor and battery amps are always equal. This is not actually true, since the motor has what is known as duty cycle, or the percentage of time that the motor has current flowing through it. At 50% duty cycle, 10A coming from the battery is translated to 20A going through the motor, at 25% duty cycle, it is translated to 40A! Duty cycle is lower at low speeds, so now we can see why editing the max motor amps affects low speed torque.
```

---
## \#3 Posted by: Jaydan Posted at: 2017-06-19T13:47:14.102Z Reads: 110

```
thanks for your reply! didn't know about the duty cycle and the difference between battery and motor current.

yeah, it's indeed a litte confusing. took a few minutes to think about it, but still not sure if i got this right. 
so battery current = vesc current and because the vesc can only handle 50A i should set the max battery current setting in the bldc tool to 50A or slightly lower to be on the safe side (40-45 as you mentioned). depending on the duty cycle, motor current can be equal or higher than the battery current. this means 80A for the max motor current setting, because the motor can only handle 80A and i don't want to risk anything for now...

...right?
```

---
## \#4 Posted by: lucagj1 Posted at: 2017-06-19T13:56:25.875Z Reads: 101

```
When your have built your motor mount can you send measurements? I'm planning on making a board myself
```

---
## \#5 Posted by: Jaydan Posted at: 2017-06-19T14:44:00.365Z Reads: 98

```
i'm sorry, i didn't use any measurements. i used the first image in [this](http://www.electric-skateboard.builders/t/eu-us-22-carbon-motor-mounts-anodized-aluminum-clamp/20795/33?u=jaydan) post, scaled it on my laptop so the measurements for the screw holes were exact, took a thin sheet of paper, put it on my screen and copied the outlines. followed up by some scissor work i got a nice template, which i then used to cut the shape out of a 10mm (recommend 12mm) block of aluminium. i modified the shape a little bit, the only important part is to get the hanger hole to the right size, but you will have to use a file for that one anyway. i still have to make the motor plate, but except for the motor screw holes i will kinda eyeball the position and angle to the deck and stuff. you really have a bit of wiggle room here. hope i could help!
```

---
## \#6 Posted by: lucagj1 Posted at: 2017-06-19T17:29:39.585Z Reads: 80

```
Ok, could you send a pic when you have made it?
```

---
## \#7 Posted by: Jaydan Posted at: 2017-06-19T19:16:09.887Z Reads: 80

```
sure! 

any further thoughts on the parts?
```

---
## \#8 Posted by: Alanhunt123 Posted at: 2017-06-23T22:23:52.996Z Reads: 70

```
I believe that 80A limit for your motor was determined with the battery side in mind. So, you are more than safe setting it at 80A. But, if you feel it doesn't have enough punch on the low end, you can try increasing it. Just keep an eye on how hot your motor gets!
```

---
## \#9 Posted by: Jaydan Posted at: 2017-07-15T17:30:59.427Z Reads: 75

```
it's been a while.. exams are keeping me busy so i don't have much time to work on this project. nonetheless, i made some progress and finally reached a point where i feel that it's appropriate to revive this thread. 

so here it is:

##UPDATE NO.1
----------

during the last few weeks, i ordered and received all of the parts. waiting for my 10 parcels to arrive was awesome, it made me feel like it's christmas time. meanwhile, i continued my work on the motor mount.

this turned out to be pretty time-consuming. i wanted to build it myself to keep the expenses down, however, in retrospect i would much rather have preferred to spend the additional bucks and save me hours of work instead. it's not that i don't like the work, i indeed highly value the experience of doing things yourself, but this was in no relation. but maybe i'm just thinking this because the only tools i used were a hand drill, a file and a vice and thus i am not 100% satisfied with the result. anyhow, the mount works and that is what it's all about. here are some pics of it. @lucagj1 you might want to take a look at these.

<img src="/uploads/db1493/original/3X/1/0/10489d8239312df9bf03e7e9728de60a86a07318.jpg" width="375" height="500">
</br><img src="/uploads/db1493/original/3X/5/0/5019674470d503c1be928fd621288ed27a457d09.jpg" width="375" height="500"></br><img src="/uploads/db1493/original/3X/f/e/fe7eb3666497d7fc651cb61918fec4272fd32477.jpg" width="666" height="500"></br><img src="/uploads/db1493/original/3X/b/b/bbfabf48b84eabf3c9001cb3cb12069b61c84992.jpg" width="666" height="500">

i still need to enlarge the holes in the bracket part, so i can adjust the belt tension and rotate the motor a little bit.


next up was the cables and connectors and stuff. i have not done any soldering in the last five years or so and even then i was by no means an expert. having said that, my first solder joint was not pretty, but over time, i got more and more confident and in the end, i actually kinda enjoyed the soldering. 


after this was done, i was finally able to put all of the components together and set it all up. i have to admit, that i was kinda nervous and really hesitant to plug the xt-90 anti spark in for the first time but it turned out that my worries were not necessary. everything worked like a charm! with the help of jacobs video, it was a breeze to configure the vesc. i used pretty conservative settings for now because i definitely don't want to push the limits, although i will probably change my opinion about this later on. the pairing of the benchwheel was a little bit tricky (simultaneously pushing two buttons and plugging in the xt90 is not so easy). after this was done, i gave the motor the first spin with the remote. that was sooooo good!!

this happened last night with the board upside down on the living room table and it happend with the truck being mounted on an old skateboards deck, because i don't have the deck i'm planning to use yet. i don't know when i will get it, but when i do and i have the time to (finally) put everything together, i will treat you with some pics!


before this is gonna happen, i still have a few of questions for you guys:
1. fuses: do or don't? and if so, which?
2. i am afraid that my motor is too low. at its lowest point, the barrel nearly lines up with the two hangers. so anything that will scratch the hanger, will scratch the motor as well. on the other hand, there is barely enough space to the deck to ensure full turning radius. how do you guys have your motors mounted? 
3. i will loctite the motor pulley to the motor because the pulley doesn't have a set screw. that means, that my motor will then be stuck to the motor plate, however i really dislike any permanent bonds. what should i do if i still want to be able to work on the motor plate later on?

that's it for now! i will keep you updated as soon as this project moves forward
```

---
## \#10 Posted by: Jaydan Posted at: 2017-12-31T15:07:57.783Z Reads: 44

```
that's really amazing.. i started this thread more than half a year ago and still did not find the time to share with you guys whats going on with my board. thankfully the time between christmas and new years eve is always good to escape from your duties and allows you to focus on the important stuff. in my case this is..

## **UPDATE NO.2**


----------
this post has been on my to do list for quite some time because of how much has happened since my last post. the board is finished by now!! well, at least to some extent.. 

BUT IT'S INCREDIBLE!!! :heart_eyes:

so here is the progress since my last post:

1. i borrowed a deck from a friend of mine, put everything together and took the board for a spin. because i didn't want to drill any holes in the deck, i used zipties and ropes to temporarily fasten the enclosure. in my opinion this actually looked pretty badass. this first testride went really well. needless to describe this feeling of pure power under your feet! https://youtu.be/x9FhVKx1rcw
2. next i got some huge 90mm wheels to replace the flywheels which i used before (which i borrowed from a friend aswell)<br/>
<img src="/uploads/db1493/original/3X/1/0/10050ae1759dfc5f8dc05d6f4699e0a8162a58d0.jpg" width="666" height="500">
3. ordered a new deck, the slipstream dfa. i really love the shape, especially the kicktail. however, it's a little bit bigger than what i was acutally looking for.<br/>
<img src="/uploads/db1493/original/3X/d/a/da9f79395f4dc140d2758a5fea1da4797e5d8d35.jpg" width="666" height="500">
4. because i had my own deck now, i could finally come up with a more convenient solution for mounting the enclosure. i wanted to be able to take it off, so i went for clevis pins. i added some rubber between the deck and the enclosure, which ensures a snug fit. <br/>
<img src="/uploads/db1493/original/3X/c/0/c0b3a364ae6e252fd6220dfe3ca7369ec44275de.jpg" width="375" height="500"><br/>
<img src="/uploads/db1493/original/3X/9/6/9686014069fec06c2fd8cc5b6646f2f3e726f509.jpg" width="666" height="500"><br/>
<img src="/uploads/db1493/original/3X/3/7/370091fe3cbb8725638856c42ef91e9894cc96a1.jpg" width="375" height="500"><br/>
<img src="/uploads/db1493/original/3X/5/e/5e41f0c7e88f30ff9760d29853911926f80ef80f.jpg" width="375" height="500"><br/>
<img src="/uploads/db1493/original/3X/b/2/b27f88066e95b293bc97f74e7fbf2ee2443c19a2.jpg" width="666" height="500">
5. last addition (for now): a bluetooth module + @Ackmaniac's firmware. i also added a switch for the lipo alarms so i can turn them off without taking the board apart. this is what the inside of my enclosure looks like right now:<br/>
<img src="/uploads/db1493/original/3X/3/a/3a7dfce29568b209530b0e0b2f573d4b05275b48.jpg" width="666" height="500"><br/>

in the future i might add li-ions and a completely sealed enclosure, but for now it's not on my agenda.
feel free to ask me any questions! and i'm always open for any feedback or recommendations :relaxed:

oh, and one more thing: both of the lipo alarms show for the 5th cell a low voltage. it's always like a 0.1-0.3V difference in comparison to the other cells. however, when i measure the cells with the charger or a multimeter they're perfectly balanced. any thoughts on this?

that's it for now. huuge :hearts: to this community for enabling people like me to tackle projects like this! you are awesome! thank you!

edit: is it somehow possible to change the thread title after 6 months? :joy: i would really like to change the homemade deck to Slipstream DFA.
```

---

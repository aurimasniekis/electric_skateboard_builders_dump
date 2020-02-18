# Creation of &rdquo;E-board database&rdquo;. Please give your feedback!

### Replies: 24 Views: 2697

## \#1 Posted by: Okami Posted at: 2016-07-18T21:06:12.567Z Reads: 241

```
In short -  this database will include detailed info on builds and their stats. 

As of right now we have made a structure on what fields would be needed to gather the required info to later compile it in one place. 
<img src="/uploads/db1493/original/2X/6/6a80df12ff55aa32069a850c0f1494da0a552181.png" width="256" height="256"> <img src="/uploads/db1493/original/2X/b/b8cbb961f94b5e044b595f6e726dc491110a4257.png" width="128" height="128"> 

---
 Once data about different parameters and statistics are gathered, there will be an option to compare / filter it with the parameter you would like to see. 

For example, choose 10S battery system, 192kv motor and see what average power consumtion (Wh per mile) these boards have and what are their setups. 

---

You can take a look at our ''plan for eboard database'' here:
---
https://goo.gl/FyHX9F
---

---
If you would like to edit the existing document, please say so, as of right now it is only possible to make comments about it (level of given access)

---

Comments are welcome, share you vision on how you would like it to look. 

You can also read our ''objectives'' in the document.
```

---
## \#2 Posted by: Okami Posted at: 2016-07-18T21:58:58.550Z Reads: 227

```
What outcome does we project from this?
---

----
I think many of us have stumbled upon that there's not enough information concerning some of the stats / specs concerning the future build or it is quite hard to find it in seconds.

---
 This may include some of the values, which need to be measured in the field, like amp draw or power consumtion. It may not only include energy related questions but also specifics about different boards (their speed, gearing etc)

 To find this information, a decent amount of time was spent searching through countless threads and posts looking for something valuable. 

----
So that's why we came up with  the idea about a database / build log collection, so that all of this info would be in one place.

 I would relate to this, in a way '' wackyboards.blogspot.com '' collects all sorts of light mobility personal vehicles.


 It would just make it easier to find something and compare to other existing models / builds out there!

-----
```

---
## \#3 Posted by: Okami Posted at: 2016-07-18T22:30:03.840Z Reads: 197

```
How we plan to ''gather data'' ? 
---
-----
As everyone does not have access to wattmeters and other equipment, our basic proposition would be to log  _**distance / average speed / consumed Wh**_. 

That way it will be possible to calculate  **''Average Wh per mile''**. 

---
This can aid in helping to understand **what distance given battery can provide** for the rider / given setup.

---

Here is a ''model''  on what data users should log to access info about their **''Average Wh per mile''**. 

Model was proposed in private message by @whitepony
> **Board / Ride stats** ..................................(device to measure)
 

> Average speed: 23kph (14.3mph) ..................(gps app)
> Range: 48 km (29.8mi) ..................................(gps app)
> Wh consumed : 430 Wh,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, (charger)

>*Best way to measure Wh consumed is to take values from smart charger, otherwise there's an option to run till your battery pack is empty and then estimate how much you consumed based on your battery pack's size*

---
>Now, it is possible to make some more calculations out of this data. 
> The aim of the database is to make these calculations automatic, so here's an example on how they will be done:
---
> Calculate **Wh/km** or **Wh/mi** = 430 Wh / 48 Km = **9 Wh/km**
> Do the inverse, calculate **km/Wh** = inverse = 0.111

>Calculate Average energy consumtion **(avg W)** = 48 km / 23kph = 2.08 hours ride (time) -> 
430Wh / 2.08 (h) = **206W** (power consumption on average)
 
---

Our idea is to compile / collect the given data and make it possible to output it in just one chart, so it is possible to analize and study different setups at once!

----
 People with wattmeters / VESC's configured for data output will be able to offer / share more in-depth data about their ride's and board setups.

---
This will include some more advanced topics / stats, like:

 **peak amp / average continous amp draw data** and some others

In my opinion, this information would be valuable when building a custom battery pack, so it would be more easier to take into account / estimate what the energy needs may be.
```

---
## \#4 Posted by: Okami Posted at: 2016-07-18T22:49:47.631Z Reads: 162

```
What else is needed?
---
----

As of right now, I have @DeathCookies in my ''team''. 

He voluntarily decided to support this project / idea and take hold of ''constructing'' / programming everything needed for this database / build log collection. 

---
I'm basically a supporter of this idea, I would like to see some more in depth data from others, that's all.

So, naturally, I have this motivation / drive to move this project further and not leave it sitting in my head till someone else, perhaps, picks it up later. 

I'm just seeing that it could benefit others right away and there will be a need for more tools like this if this community tends to grow even bigger!

---

My vision right now is as follows: 
---
----

Make a database / build log collection, so that:

1) It is possible to quickly sort through different setups and see what amp draw / distance / etc specs they are having,  what gearing, what wheels, what trucks they have on their boards. 

Contact them, if needed.

(There's going to be an option to include username / email, for extra feedback from others)

2) By doing this, get a quick raw estimate on what current demands each setup / wheels etc are having. Estimate what specs / stats will my build have by comparing similar builds / models already made by others.
```

---
## \#5 Posted by: lox897 Posted at: 2016-07-19T05:39:50.132Z Reads: 139

```
Is @evoheyax in this team as well? Isn't he making a database?
```

---
## \#6 Posted by: evoheyax Posted at: 2016-07-19T05:46:32.851Z Reads: 141

```
My database: [esk8parts.us](http://esk8parts.us)

I've been programming this site in my spare time. I've been spending more time lately on making a better board the last few weeks. But I want to keep going. I posted a topic about needing mods a few weeks ago, but didn't get any thing really.

The site is incomplete by far, but I will have some time in early august to hammer out the real features. Right now, I need mods to check categories and decide what specs should be kept for every category of part. I'm also likely missing part categories.
```

---
## \#7 Posted by: zeno Posted at: 2016-07-19T06:19:51.170Z Reads: 140

```
Cool! I had a similar idea actually :) 
If extra development help is needed / wanted let me know!
```

---
## \#8 Posted by: Okami Posted at: 2016-07-19T10:01:37.856Z Reads: 138

```
Do you know any **programming language -  PHP, HTML, Javascript?** 

If yes, then there is a possibility that you might help @DeathCookies at some point, so he does not have to code everything.

---
If you are not into programming that much, then there's another area where help is needed
 
**VESC Related information**

It would be great, if VESC users could suggest what entries / data fields should be there for ''Vesc related data''. As I am not an Vesc expert / user myself, then we fall  a little bit short on this one.
```

---
## \#9 Posted by: shred Posted at: 2016-07-19T10:16:03.015Z Reads: 123

```
Hey Okami, really like your idea!! I checked the google doc today and was thinking it might make sense to add battery cutoff value, besides I think it looks quite complete. 

Maybe a nice feature for all the VESC users could as well be a upload option for the VESC settings, just a idea :)
```

---
## \#10 Posted by: DeathCookies Posted at: 2016-07-19T11:33:06.321Z Reads: 115

```
[quote="shred, post:9, topic:6291"]
Maybe a nice feature for all the VESC users could as well be a upload option for the VESC settings, just a idea :slight_smile:
[/quote]

Really great idea! Later I will implement an upload of the config file of the VESC that it will automatically extract the needed information!
```

---
## \#11 Posted by: shred Posted at: 2016-07-19T11:38:14.063Z Reads: 107

```
:D wow that sounds awesome! really looking forward to see this project progressing! 

And sorry, but my programming skills are a bit rusty, but if you have questions related to hosting, apache configs or something, feel free to come my way.
```

---
## \#12 Posted by: karma Posted at: 2016-07-25T11:41:47.322Z Reads: 103

```
I am a Java Script developer and web designer with experience in React, React-Native, Webpack, Babel. (Ofc I also know vanilla, jQuery, HTML and CSS) I could maybe help with the front end. Send me a pm if interested.
```

---
## \#13 Posted by: Okami Posted at: 2016-10-06T02:34:08.605Z Reads: 86

```
Hi there, to all of you who did notice this little project 

Some time has passed and I am willing to share the progess which has been made.

Here is the short link to the page we have created so far:

www.ej.uz/e8base

---

As of right now the page still lacks some important features and design attributes. It is possible to take a look and get a ''raw sample'' of what it should look and feel like once it is finished. 

---

Reason I'm posting this is because as of right now there's only one main programmer doing all the heavy lifting, if, perhaps, few more people could jump in (by investing few hours or so) this project could progress further at a faster pace!

If some of the ideas are still not clear or information is lacking or mixed, let me know! I will try to describe the concept and the expected outcome as good as I can!

--

Would be great to build this platform, which would be benefical to a lot of users, as I believe a lot of important data and notes can be missed in these long build logs and posts.

We intend to incorporate **compare function**, so that it is possible to take a look at 5 different boards at the same time.

Next level would be **VESC DATA UPLOAD**. You could see what parameters/settings others are using and perhaps borrow some of the ideas/info out of it.

And, finally, one of the things which are sort of close / important for me right now - somewhat decent **AMP DRAW DATA**, of course, this is heavily depending on the user input but I do hope that we generate some interest in the future and that we start collecting easy to access field data for Li-Ion battery pack builders.

--

Hold on till our next update!
```

---
## \#14 Posted by: karma Posted at: 2016-10-06T13:07:19.358Z Reads: 66

```
Important to know is that this project has the backend wtitten in PHP!
```

---
## \#15 Posted by: flatsp0t Posted at: 2016-10-06T13:16:36.170Z Reads: 74

```
Is this project somewhere on github?
This would make contributing easier.
If i find the time to finish my VESC XML parser and validator, i could add this too.

EDIT:
Maybe @makevoid wants to add some of his Ideas:
http://www.electric-skateboard.builders/t/vesc-configuration-web-tool-alpha/7171/8?u=flatsp0t


But maybe it is better to wait for the rewrite of the BLDC-Tool, as the data-structure will also be subjected to changes.
```

---
## \#16 Posted by: Bazingazunga Posted at: 2016-10-06T15:13:05.879Z Reads: 63

```
Hi guys just to chip in - I have experience (in order of best known) of HTML, PHP, and a little bit of JS. Im sure i could help out in my downtime if im needed? Depends on the amount of work - cant guarantee much as I have a full time job. 

I've checked out all the sites in this thread, at very least I could help out with  your data structures and display in PHP, and have a good shuffle round of the HTML/CSS to make the site more aesthetically pleasing :)
```

---
## \#17 Posted by: Jebe Posted at: 2016-10-07T11:00:49.048Z Reads: 61

```
Vesc esc firmware revisions vs failures. Known firmware issues and fixes
```

---
## \#18 Posted by: oneafrikan Posted at: 2016-10-07T11:03:04.624Z Reads: 59

```
how are you going to code this up?
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-10-07T13:13:11.291Z Reads: 54

```
[quote="oneafrikan, post:18, topic:6291, full:true"]
how are you going to code this up?
[/quote]

What do you mean exactly?
```

---
## \#20 Posted by: oneafrikan Posted at: 2016-10-07T13:30:50.939Z Reads: 51

```
Tech stack / language etc etc
```

---
## \#21 Posted by: DeathCookies Posted at: 2016-10-25T12:01:43.306Z Reads: 41

```
Currently pure php, js, css + html. Mixed wildly, strangely...
```

---
## \#22 Posted by: tueboard Posted at: 2016-12-28T00:20:50.105Z Reads: 40

```
What happened to this? I think it's a good idea
```

---
## \#24 Posted by: Okami Posted at: 2016-12-28T16:40:42.597Z Reads: 30

```
As I was not a direct programmer / maker of the project, more like  a co-creator / supporter of this database then, I think, @DeathCookies can answer this one better.

So, before he has answered to this topic personally, I will try to give my answer to this question:

So -  the short answer to that (from my perspective) is that **it got a bit stuck**..

He was just one guy doing all the heavy lifting, though there was @karma also who helped with design here and there but for the structure/functions side @DeathCookies was the only one progressing the project further from bare bones / structure perspective

I was helping with ideas and just tried to keep it on track, though, I think @deatchookies can reveal more on what stopped him from taking it further and also making it possible for others to join the project.

Personally, I remember him saying that he also has main job and that he had been very busy lately to continue the project (at the time it started to slow down).. and he also mentioned that he has done some mistakes to the code and general structure of the page, so it is very hard to revert that back, so that others could use and understand what he has made..

---

Personally, would have loved to see this project grow and propel (prospect) further.. I assume it is not a one man's (one programmer's job) to make this happen.. so in order to achieve this.. we either would need to encourage @DeathCookies to finish it up (make it accesible for others).. or just start from scratch sadly.. of course, the 2nd option is not so nice and motivating, 

**So I do hope it is still possible to resurect some parts of what has been already done and make it into a somewhat good and useful page for fellow eboard enthusiasts and builders, who might really need and would benefit from easier search engine of builds and also a compare function, which we so much advertised and strived for in the ''early stage''.**

So yeah, generally speaking, I still have not given up on the idea, the bad thing is that im not a programmer now myself.. and basically all the work which has been done relies on just one person and this person is @DeathCookies .. so he is the one to contact and ask for details and his opinion about the project ;)

I've seen some early attempts at discussing the idea of collecting vesc video logs but have not seen an actual place / manifestation of such idea yet.. so perhaps it is not that late yet to make an esk8 database ! :)
```

---
## \#25 Posted by: saul Posted at: 2016-12-28T17:13:14.530Z Reads: 29

```
I think now that there are some data logging options out there for vesc the database has a chance. but its still very early, the mobile apps don't have any sort of standard.

For now I went with general build guides on [my site](http://esk8.today/guides/build-guide/), and I just made a range calculator for decent estimates based on battery.

at some point I'm thinking some real tests on range based on wheel size, gear ratio, battery voltage maybe even deck style?
```

---

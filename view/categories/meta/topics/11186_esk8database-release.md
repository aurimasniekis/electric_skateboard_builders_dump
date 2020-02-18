# Esk8Database Release

### Replies: 14 Views: 1410

## \#1 Posted by: DeathCookies Posted at: 2016-10-15T16:42:59.969Z Reads: 129

```
Hey folks,
its me again :D In this thread I and the esk8database-team (@okami @karma) want to announce the (official) **_[esk8 database](http://gct-hp.de/esk8/)_**.

**What is it?**
It is a database with (hopefully) all builds in one place!

**Why an extra database?**
Because it is an annoying process to search this forum for specific builds, extract all information from the complete build thread and to compare these information next to another build!

**What does this database make special?**
Every build will be at one place and there will be functions tweaked to OUR needs to compare every bit and nut from one or more builds

**Does it cost anything?**
No, i want to contribute to this awesome community. So it is completly **free** and will be forever!

**How far did we get**
We have a working prototype to submit a build and to compare it with other builds:
- Every user needs to login with a google account and can share a build.
- Pictures will be used directly from dropbox
- Compare up to 5 builds next to each other



**What do we plan**
- improve the style (mockups by @karma :thumbsup: ) 
<img src="/uploads/db1493/original/3X/1/3/1346458b332cb168bb1bbe6b1d1a6664c07e8f95.jpg" width="300" height="236"><img src="/uploads/db1493/original/3X/5/d/5d28198cc0883594d16dac77114fb248ff148591.jpg" width="300" height="222"><img src="/uploads/db1493/original/3X/2/9/2982bd5dd7fb1f979c9391560f680c059e3ccbbf.jpg" width="300" height="222">

- Implement different charts
- everything **_YOU_** want! ([excel todo list](https://docs.google.com/spreadsheets/d/13cx3_dCjhTAUwIBR7pgbToA8tEjmy1Ev5aswBsv1MLw/edit#gid=0))


**What is my plan as developer**
My goal is to provide an unique database tweaked to your needs:
I am learned software developer but i underestimate the work of such a "simple" database. I did not plan it very well and have to pay the price for it. What do i mean of price? I have made everything from scratch. I did not use a framework which would have saved me tons of time.... I had made several work-arounds which results in slowly developement. 
My current goal are the following three points:
1. Extend the prototype with your needs
2. Rewrite the code by using a proper framework
3. Make the source code of the database open source

**Why dont i make it open source NOW?**
Because my code is really messy and no one could really contribute...

**Why do i want to make it open source after all?**
Because i like the idea of open source. Why should i hide my database when so much people could contribute in the future. I do think open source is the **best way** for the future!

**Side notes:**
I have a full time job and have created the database in my **free time** on my own for free. That and the poor planing is the reason why it took so long to publish this first prototype.
But in the beginning of the next year i will have more free time to develope the database even faster. That does not mean that i wont do anything this year. It only means that i can work on the database in my free time after my full time job but i am glad to contribute in this nice community!

If you like the database and want to contribute:
Feel free to help us:
- Update the todo list with new improvements/wishes
- Or leave a comment here with improvements/wishes
- Leave a little donation for the hard work
```

---
## \#2 Posted by: Goombaacez84 Posted at: 2016-10-15T17:42:03.023Z Reads: 81

```
Great work! I'm a dev for a living and I've thought of ways to use my developer skills to help the community, like writing a web-based version of the BLDC tool that just generates an XML file for users to upload via the traditional BLDC tool... This allows me to inject logic for things like adding warnings if users are putting in strange or abnormal values for various fields, or provide actual documentation about what the different fields do (with community input of course). I haven't taken the time to research the BLDC tool too much, the XML schema, design, or plan, so if anyone's reading this, feel free to implement said idea if you please.

I'm curious about the inner details of the stack you're using. It looks like the pages being served up are php pages, so LAMP stack?
```

---
## \#3 Posted by: IDVert3X Posted at: 2016-10-15T17:57:19.508Z Reads: 76

```
You said your code is a mess. Maybe you should use a framework, Laravel is great.
You can write very nice apps using it in no time. It's OOP MVC framework and has really nice DB model.
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-10-15T21:02:42.425Z Reads: 60

```
[quote="Goombaacez84, post:2, topic:11186"]
I'm curious about the inner details of the stack you're using. It looks like the pages being served up are php pages, so LAMP stack?
[/quote]

Yes, purhe PHP strangely mixed with pure Javascript ( + a bit jQuery and bootstrap)... weird approches but they lead to the goal :D

I will write you a pm in a second ;)
```

---
## \#5 Posted by: DeathCookies Posted at: 2016-10-15T21:09:23.023Z Reads: 50

```
[quote="IDVert3X, post:3, topic:11186, full:true"]
You said your code is a mess. Maybe you should use a framework, Laravel is great.You can write very nice apps using it in no time. It's OOP MVC framework and has really nice DB model.
[/quote]

Yes, currently i need to work with laravel in my other project! Nice match :smiley:
I will learn it right now but before i rewrite my code, i will **extend this prototype** to clarify what the community really needs. Then i will replan the whole database in laravel and write the complete source code under open source on github. there can everyone contribute who wants to. ;)
```

---
## \#6 Posted by: Dutch Posted at: 2016-10-15T21:20:27.384Z Reads: 46

```
What are you using to connect with your database ? MySQL, MySQLi or PDO. Would recommend PDO and never ever use plain MySQL, that's to unsafe nowadays.
```

---
## \#7 Posted by: DeathCookies Posted at: 2016-10-15T21:31:49.897Z Reads: 43

```
MySqli with less SQL-Injection...sadly... :frowning:
i just underestimated this project....

in the database 2.0 laravel will be PDO, Cross-Site Request Forgery and Cross-Site Scripting safe
```

---
## \#8 Posted by: Dutch Posted at: 2016-10-15T21:34:53.792Z Reads: 41

```
If you need help just ask. 
I have experience with HTML5/CSS3/PHP4/PHP5/jQuery/Javascript and some CSS preprocessor like SASS and LESS
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-10-15T21:37:04.775Z Reads: 41

```
PM sent in 10 seconds/characters.
```

---
## \#10 Posted by: lox897 Posted at: 2016-10-16T08:40:56.746Z Reads: 35

```
I'm getting an error when logging in: Duplicate entry '0' for key 'PRIMARY'
```

---
## \#11 Posted by: DeathCookies Posted at: 2016-10-16T14:28:16.237Z Reads: 30

```
When i am at home i will investigate in your error and Report back. Thanks for the information!
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-10-16T19:51:55.688Z Reads: 23

```
It is working again. Now you should be able to login. I have tested it with two different accounts ;)
```

---
## \#13 Posted by: Goombaacez84 Posted at: 2016-10-16T19:57:58.898Z Reads: 25

```
I was going to mention that it could be a database issue where the primary key isn't auto incrementing itself so it's always trying to create new records with the same id
```

---
## \#14 Posted by: DeathCookies Posted at: 2016-10-16T20:03:57.025Z Reads: 25

```
That was actually the problem. The installer script of the plugin integration did not work bug free...
```

---

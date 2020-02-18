# Is there a PC part picker type of website but for esk8 parts?

### Replies: 27 Views: 2414

## \#1 Posted by: SWaller Posted at: 2017-07-19T23:20:51.162Z Reads: 235

```
Do you guys know if there is a website like PC part picker but for esk8 parts? That would be awesome and I would be less confused. Slowly figuring this out though.
```

---
## \#2 Posted by: rpn314 Posted at: 2017-07-19T23:38:53.361Z Reads: 231

```
Not that I'm aware of (though an excellent idea!). Looking through other's builds on here and reading through a bunch of the FAQ and "noob" topics is your best bet.
```

---
## \#3 Posted by: SWaller Posted at: 2017-07-19T23:43:07.762Z Reads: 231

```
Hopefully someone is working on that, would make things a lot more organized. I have enjoyed looking through peoples boards, time to look into my own!
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-20T00:25:05.439Z Reads: 213

```
I could probably do this pretty quickly and without a ton of effort but the problem would be how to monetize it and make it worth maintaining in terms of updating parts lists available from various vendors and all.  Could just throw some advertising on the page or take kick backs from the vendors but that requires getting affiliate links or negotiating with the vendors (then a bit harder to stay completely unbiased too).  Let me know if you have any other ideas on how to make it worthwhile.  I think the main problem is there are just different vendors selling different sets of components and/or completes so if you are doing the DIY path you are kind of best off searching around if you want to get the best deal on the various necessary components.

Basically components are:

  - Power/Drive Train
    - Motor
    - Motor mount
    - Pulleys for motor and wheel
    - Belt
    - Hub Motors
  - Battery Power
    - Battery form factors/chemistry
      - LiPo/18650
      - Li-Ion variations like LiFePo
      - Lead-acid (Pb), NiMH
    - Practical understanding of, voltage, amperage, resistance, power loss, and amp hours.
    - Loop keys and power switches
  - Battery Chargers/Management
  - Electronic Speed Controller
    - VESC
    - X-Car Beast
    - other
  - Controller or Transmitter and Receiver
  - Wiring and connectors
  - Lights, telemetry, extra electronics
  - Enclosures
  - Decks
  - Trucks
  - Wheels
  - Risers

Feel like the last four have been covered a ton on the internet since they are more general skateboard things and not so much affected by eskate but could include some things that are relevant to just esk8 like deck stiffness, wheel durometer/size, pulley mounting.

---

Also there are a few ways to approach this.  Could be like a Dell or Apple pick a base model then add/remove components, or could be more like a new egg PC builder tool where you just fill in one of each type of thing and it tries to let you know if things are incompatible then tells you the price and specs in the end, or you could give it a target set of specs and/or price and see what it can come up with.... it is a good idea :slight_smile:
```

---
## \#5 Posted by: rpn314 Posted at: 2017-07-20T00:36:28.455Z Reads: 175

```
@wafflejock I'd be down with helping develop that!

I think affiliate links may be the best, possibly with some ads. IMHO, as long as we're open that they're affiliate links (some message saying "we appreciate your support of the site by using these links, which may give the site some money to keep up the site)
```

---
## \#6 Posted by: pennyboard Posted at: 2017-07-20T00:55:56.256Z Reads: 165

```
I think if you put the site together and maintain it, you should just throw up ads to monetize. I doubt people would mind since basically every site nowadays has ads, and it would cover the costs/time commitment for you.
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-20T00:58:14.559Z Reads: 164

```
Cool yeah would just need to pin down which approach we'd want to take and pick out a tech stack we can both deal with (or divvy up front-end/back-end work).  Also figure out what to do about the monetization division and hosting costs and all (can use a cheap digital ocean box but still a few bucks a month).

Once we know which approach we want to take can (do a little research on similar sites in other industries) lay out some basic wireframes or just do some prototyping of views in plnkr or codepen or whatever and then throw together a github/gitlab repo with some "minimum viable product" and can flesh it out from there.

Personally have a lot of angular 1.x experience so for front end I'd prefer either using that for expediency of getting it done or using angular 2+ so can get a better handle on that since I've only done some basics with it so far.  Otherwise could use React but that'd be a somewhat bigger learning curve for me.  We could go frameworkless too in terms of the JS on the front end but I do like having something deal with the nuanced things like AJAX requests.  Have used bootstrap a ton and angular-material (google's material design CSS) a fair amount but not too familiar with other CSS frameworks/base styles.

On backed I'm most familiar with PHP and MySQL or Postgres (really just use Eloquent ORM and/or laravel so don't touch the SQL directly most of the time), but don't mind working with Node frameworks either really (no real experience with Ruby or Python though for any extended period of time).

Anyhow all the technobabble aside definitely going to think about this a bit more, let me know if you all have thoughts/feelings on the different possible approaches, in the long run maybe could have user submitted parts for different categories as well to reduce the maintenance burden and keep things up to date.
```

---
## \#8 Posted by: SWaller Posted at: 2017-07-20T01:11:29.537Z Reads: 138

```
Thank you for this list. With the monetization through ads wouldn't that require a bunch of traffic?
```

---
## \#9 Posted by: Jebe Posted at: 2017-07-20T01:13:03.932Z Reads: 137

```
I think @longhairedboy is working on something like this.
```

---
## \#10 Posted by: treenutter Posted at: 2017-07-20T01:16:34.936Z Reads: 134

```
@longhairedboy's configurator is live, and it's awesome! www.longhairedboy.com
```

---
## \#11 Posted by: wafflejock Posted at: 2017-07-20T01:23:38.448Z Reads: 136

```
Ah okay.. hmm yeah will leave him to it then more experience and think he sells parts anyhow so is sort of a way to make it worthwhile to do as well.  Thanks for the heads up guys.

---

That is a pretty nice layout was thinking something similar in terms of the main tabbed navigation for high level parts, still might be worth doing for something that is across more vendors and options, but yeah need to figure out how to make that worth doing.  Ads would require a lot of traffic to really make up for the hosting and development time but would at least help offset the hosting some, with affiliate links usually you can get a percentage of products purchased through the links I believe (depends on the affiliate program).  Best scenario is really as it is with longhairedboy though were you also have products... only down side with that is you are automatically biased and sort of need to downplay other products.
```

---
## \#12 Posted by: SWaller Posted at: 2017-07-20T01:35:46.495Z Reads: 107

```
I saw his configurator, not nearly as many options and vendors as I was thinking it was going to be. I saw only 3 decks, 2 batteries, etc. I do think it may still be worth doing.
```

---
## \#13 Posted by: wafflejock Posted at: 2017-07-20T01:40:48.995Z Reads: 103

```
Yeah it's a pretty nice layout for the things he's selling it would be nice to have but needs to be maintained... think we would actually probably be best off starting with user submitted data that we curate/verify to get the thing populated so it's not a huge time investment on that up front or over the course of time for any one person, but setting up the forms for data submission and all does take a little time so would be good to make some actual money back from the thing somehow for the time invested to develop it in the first place.  It could be packaged up as a "hybrid app" where it shows up in the play store (maybe app store too but more work to submit there and costs more to keep it active) and then could either do ad overlays or a $1 version with no ads but sort of sucks having to restrict it to mobile only though... I'm still in considering it phase :)
```

---
## \#14 Posted by: longhairedboy Posted at: 2017-07-20T15:04:14.798Z Reads: 91

```
Just want to chime in here. My thingymabobber is specifically for ordering custom boards from me, not necessarily for generating a parts list for yourself. For that it will fall severly short because i'm trying to whittle down what the customer actually gets to choose from because things like ESCs, trucks, and motor mounts are the kinds of things i would rather just use the best of, and are often limited by other factors such as supply, parts availability, dependancy on other parts, etc.  Bearings, wheel options, deck shapes, pulley ratios, battery pack size and artwork are the things i am focusing on.
```

---
## \#15 Posted by: SWaller Posted at: 2017-07-20T15:30:14.811Z Reads: 94

```
I fully understood that your thingy was for specifically ordering custom boards from you. Not sure if the guy that said "@longhairedboy's configurator is live, and it's awesome!" understood what I was getting at when I said what I said. I just found out about this esk8 world and a configurator on the skale of pcpartpicker would be awesome and help me a bunch. I actually saw your configurator a few days ago and it was the first time I said to myself, "Ah cool, someone is getting somewhere." Previous to this I would just go to websites looking at esk8 stuff and would just see a picture, an item, and a price. yours gave me a better perspective.
```

---
## \#16 Posted by: longhairedboy Posted at: 2017-07-20T16:15:41.574Z Reads: 93

```
I think something like that would require a community effort but i can tell you this:

The code i wrote would easily support it. It is completely extensible and loaded up with parts via JSON manually, so it can be updated manually with new part information with very little effort.

I suppose i could leave out the bits that add the specific items to the shopping cart and post it somewhere for people to use.
```

---
## \#17 Posted by: wafflejock Posted at: 2017-07-20T16:22:05.524Z Reads: 90

```
Hey I started putting this together in plnkr yesterday, made pretty good headway but doing the same for now just pulling data in from a hard coded JS object structure, think longer term can make a DB that can have curated user submitted part specifications and links.  Like I mentioned above only issue is monetizing it to at least cover costs since there's no product for sale, could just do donations but doubt that would even cover the costs.

---
Starting point below still working out how to determine what is necessary and optional (where I need to use radios, drop down, or check boxes for selecting items)
http://embed.plnkr.co/oh8VtizqeLvDVmHsQjvo/
```

---
## \#18 Posted by: SWaller Posted at: 2017-07-21T06:16:12.690Z Reads: 77

```
This is pretty good, did you do this all yourself? I'm currently taking java but my projects are super simple.
```

---
## \#19 Posted by: wafflejock Posted at: 2017-07-21T06:20:22.261Z Reads: 76

```
Yeah just threw it together last night I'm not super enthused with the layout but trying to figure out if I can keep a pretty generic data structure for the whole thing so the view parts don't need to have too many "exceptions" or conditional elements.  Hard part is lots of things are optional and some things you can choose more than one so just need to figure out appropriate input types and how to handle validation so can say if you missed selecting some key component also need to work on how the specs for a type of thing work with the data entry (which doesn't exist yet).
```

---
## \#20 Posted by: SWaller Posted at: 2017-07-21T06:34:08.700Z Reads: 72

```
I see where the headache can start to come into play. Most I have done was made a GUI vending machine. I applaud you for what I see so far.
```

---
## \#21 Posted by: wafflejock Posted at: 2017-07-21T06:49:23.033Z Reads: 69

```
Thanks for the encouragement!  An angular lead dev would probably scorn me for some of the things I did here, but that's the great thing about working alone :wink: 

Given you have some Java background you'd probably actually like Angular especially Angular 2+ (angular.io).  I'm using the 1.x variant here, it's basically a JS framework that reads the HTML and binds data from the JS into the HTML.  It also gives you dependency injection which is a big thing in the Java (enterprise) world.  Angular 2 they adopted TypeScript which is a Microsoft technology that is basically a superset of ECMAScript 6 (the latest JS tech) and adds optional Types like you have in Java (String, Number, StringBuilder, FileStream etc.) and allows you to define classes and do other things that more "highly developed" languages can do (then through some black magic they convert it back into JS so it works in a regular browser).  Anyhow all the stuff basically makes developing "web-apps" or "hybrid applications" a lot easier (especially with big teams) despite being a ton of stuff to learn up front (obviously I'm an advocate :) ).
```

---
## \#22 Posted by: SWaller Posted at: 2017-07-22T05:40:36.957Z Reads: 58

```
np, keep up the good work. You've got something good here. One month before school starts, I'm ready to get back to Java class so I can get on your level.
```

---
## \#23 Posted by: michaelcpg Posted at: 2017-07-22T07:15:41.463Z Reads: 60

```
Good to see another Angular dev on the forums :)
```

---
## \#24 Posted by: wafflejock Posted at: 2017-07-26T21:12:26.762Z Reads: 57

```
Hey everyone just posted this last night to github so other people can actually contribute to it:

https://github.com/shusain/Esk8Builder

Currently no backend it's just front end with some JS files that have the data for display in them, all that data could be moved to some backend system basically and then can have forms that submit data to the backend system and are flagged for review so they don't show up in the main data until someone has verified it isn't just spam.  For the time being I'll just do the verification myself but would be good to see if anyone is interested in taking on the backend since I don't really have a great solution for it long term (was thinking firebase since it's free for smaller projects but I also don't have a ton of faith in Google maintaining that service forever, perhaps some of the .NET guys on the forum could chime in on some options for hosting a backend where we don't lose an arm and a leg beyond the development time).
```

---
## \#25 Posted by: cfranci Posted at: 2019-03-04T20:09:47.341Z Reads: 35

```
Are you still wanting to develop this?
```

---
## \#26 Posted by: wafflejock Posted at: 2019-03-05T21:44:54.670Z Reads: 30

```
Ah sorry I had completely forgotten about this, it could still work as is but would be good to upgrade angular versions before adding much to it (still the data and structure with having things divided into services would still work fine).

The new angular versions use TypeScript and annotations on classes for defining components.  One plus side of it not being DB driven is the deployment can happen to github.io static web servers and keeps the cost at 0, downside being can't really have a form that pushes a commit and creates a PR so getting new data in requires someone to at least be able to edit the JS files.  Anyhow yah let me know if you're interested in fleshing this out more, there's a site ecalc.ch that has lots of component lists so you can select all the parts and it can calculate a lot of the load and lift for RC aircraft, was hoping to eventually get something like that built into here.
```

---
## \#27 Posted by: wafflejock Posted at: 2019-03-06T00:45:50.100Z Reads: 18

```
@cfranci if you'd be interested in contributing on this let me know (also what you'd be interested in adding and relevant skills, nothing required just curious about background) and can probably 'revive' the project, looks like I didn't define too many directives/components in the project yet so shouldn't be too bad to make the upgrade to angular 7 (pretty sure that's the latest).

I have also done a decent amount of VueJS work in the last year or I suppose could go with React but I'm less familiar (have only done 1 basic React site for the sake of learning it, used redux, redux-saga etc. etc., but yah just less familiar with that framework).

Vue has VueX, and Angular has NGRX that are roughly equivalent to redux (maybe not needed here but it's a helpful pattern in general).

---

Also if you're familiar with github and can figure out the project structure you can just put in PRs and I'll merge (then travis.yml file has deploy instructions that build and copy to "pages" to show up on github.io)
```

---

# I made an esk8 parts picker (kinda)

### Replies: 15 Views: 1028

## \#1 Posted by: Thanorak Posted at: 2018-04-23T05:53:04.532Z Reads: 259

```
So a month or so ago, I decided to build an esk8, and I've been lurking here for a while, trying to learn as much as I could.  Recently, my friends also became interested in DIY ek8s, so I decided that I would make a PC part picker-esque excel spreadsheet to help them out.  The idea was that you could put parts you found in the database, and then you could choose from lists of those parts.  It's actually turning out better than expected (Excel id freaking awesome for those who dont know), and the limiting factor for the part picker right now is our lack of esk8 knowledge.  So I thought, why not turn it over to the awesome people at this forum!  I could upload it to google sheets, share it with you guys, and you could help us out by filling out the database, and you'd have a part picker.  I'm not totally done yet, but this is roughly what it would look like:

![Esk8 Part Picker|563x500](upload://9sV301RLdlyntnlK0JVinP4dMBN.PNG)

Basically, you have a bunch of part catagories, and next to each one is a drop down menu of parts in the database.  For every catagory, there would be a page that looked like this:

![Wheels|623x500](upload://tIacVl4FO6s2UdgoQb5T8vQAPFs.PNG)

It would have a link to the part, as well as pricing and other information that I could use to calculate stuff like board specs and comparability.  Obviously this wouldn't be the only tool you'd need, but it'd be a pretty good place to start.

I probably won't be able to put this up until tomorrow, just trying to gauge interest.
[poll type=multiple min=1 max=2]
* No, just keep it to yourself
* Yeah, I'd be interested
[/poll]
```

---
## \#2 Posted by: Eboosted Posted at: 2018-04-23T06:12:17.599Z Reads: 220

```
That's pretty cool, can you also add the source to place the order?
```

---
## \#3 Posted by: Thanorak Posted at: 2018-04-23T06:18:13.201Z Reads: 212

```
I'm not entirely sure what you mean.  Right now, clicking on the cell directly to the left of the part you selected would take you to the cell where that part is located.  For example if i selected ABEC 11 97mm 75a as my wheels, and I clicked on cell A10 on the total cost sheet, it would take me to cell 7A on the Wheels sheet.  from there, you can click the link next to it would take you to the page to buy the wheel.
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-04-23T06:58:19.064Z Reads: 183

```
Where did you source 30q batteries for 3.39?
```

---
## \#5 Posted by: Thanorak Posted at: 2018-04-23T07:23:30.537Z Reads: 167

```
Ok, so [I made a video](https://youtu.be/GluihyUJUT0) of what it's gonna look like, more or less.  I think it addresses both @Trdolan03 and @Eboosted's comments, as well as showing off the basic features of the spreadsheet.  Id also like to add that the price there does not count the cost of shipping, so realistically it will be slightly higher, depending on how many you order.
```

---
## \#6 Posted by: Scoo_B_SK8 Posted at: 2018-04-23T07:51:33.207Z Reads: 166

```
ya man thats a great idea, not just an idea but already have a good start with database of parts.  I think if you had an "Add Part Link" instead of out right letting everyone have access and you be the OP to keep it in line and clean... or something like that.  i just think it would get ugly if everyone had access.

also another thing should think about are these items noted by @Eboosted
https://www.electric-skateboard.builders/t/these-items-should-be-on-the-drawer-of-any-esk8-builder/53066
```

---
## \#7 Posted by: Thanorak Posted at: 2018-04-23T07:58:33.733Z Reads: 150

```
Honestly I hadnt even thought about how I was going to handle other people using it, until a couple hours ago I thought my freinds and I were going to be the only ones using it.  And one of the "features" I was planning onn adding was a "miscellaneous parts" tab, where I would add a bunch of things just like the one in @Eboosted's post, and that list is a great place to start, so thanks.
```

---
## \#8 Posted by: lrdesigns Posted at: 2018-04-23T08:13:48.872Z Reads: 141

```
Cool, will you make it into an google doc or something like that then it can be worked on by multiple people?

I'd like to add these new wheels on the block (abec quality) 
https://boawheels.com/products/constrictor-100mm-wheels
```

---
## \#9 Posted by: koralle Posted at: 2018-04-23T08:32:29.066Z Reads: 127

```
If you find a way to include a belt calculator that considers idler pulleys, this thing will go tru da roof.
```

---
## \#10 Posted by: banjaxxed Posted at: 2018-04-23T09:18:54.688Z Reads: 120

```
Pretty cool, how do we allow concensus to determine  rankings of parts.

97mm Clone wheel Vs real abec 97 flywheel, both have same duro but we know they are chalk and cheese in real terms. Maybe a ranking element would help in deciding cost as one thing Vs quality as another
```

---
## \#11 Posted by: Scoo_B_SK8 Posted at: 2018-04-23T09:57:29.634Z Reads: 109

```
This thread could be your "Add Part Link"

the number of "Likes" for each request could take care of 2 things... 

-verification of part
 (cause your gonna have 3D printed parts i.e. pulleys, covers & designers selling here almost exclusively i.e. motor mounts)

-rank (like what @banjaxxed mention) 

maybe even having a minimum "like" count before even making the list
```

---
## \#12 Posted by: Thanorak Posted at: 2018-04-23T14:17:03.790Z Reads: 87

```
@lrdesigns Yes, I will be uploading it to google sheets probably later today, when I get everything working.

@koralle An idler mount would work with this sheet!  Since you can enter whatever parts you want into the database, all you have to do is enter an idler mount

 @banjaxxed’s post is something I’ve been thinking about ever since I decided to make this public, but I’m not yet sure how voting would work in excel
```

---
## \#13 Posted by: Thanorak Posted at: 2018-04-23T18:33:37.637Z Reads: 84

```
Ok so I just got done writing a script for an add parts button, like @Scoo_B_SK8 suggested.  It looks like this:

https://youtu.be/LORVwPUMX54

However, I am in college right now, and I have a couple midterms this week, so this is probably all the progress I'll make until thursday.  If there are any other functions you want, let me know and I'll get around to adding them when I can
```

---
## \#14 Posted by: Thanorak Posted at: 2018-04-24T07:13:58.217Z Reads: 65

```
Ok so I just finished making a button that, when  pressed, creates a new template at the end of the document and assigns the only editors to be me and that user who pressed the button.  Do you guys think that would work?  It also requires sharing your information with the sheet, and therefor me, so if you guys are uncomfortable with that let me know and I can try to think of a different solution
```

---
## \#15 Posted by: cfranci Posted at: 2019-03-04T20:04:21.678Z Reads: 29

```
I want to collaborate on this and take it up a notch. Can you share the sheet?
```

---

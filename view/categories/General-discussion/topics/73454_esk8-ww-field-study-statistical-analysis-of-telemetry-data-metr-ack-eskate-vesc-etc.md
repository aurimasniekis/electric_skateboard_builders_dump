# ESK8 WW Field Study. Statistical Analysis of Telemetry Data. METR / ACK / eSkate VESC etc

### Replies: 69 Views: 1374

## \#1 Posted by: bevilacqua Posted at: 2018-11-04T22:28:48.339Z Reads: 351

```
Hello fellow e-skate Builders, 

This semester I will write my semester-thesis (similar to a longer paper that has to be presented before the Master thesis). I went to the Institute of Automotive Technology at my university (TUM, Munich) and approached them with a topic of my own that basically consists on doing an eskate telemetry analysis, but on a larger scale: aka field study. They found the idea very interesting. They also found eskates quite fascinating and loved the potential it has as an alternative means of transport, especially in larger cities. 

Thanks to the immense potential of the VESC open-source architecture we can log tons of ride-information. That data can be later analyzed individually. My goal is to go one step further, which is statistically analyzing hundreds of logs simultaneously. Not focusing just on one rider but on our entire worldwide community. 

Large automotive companies have been doing field studies for many years, focusing on the development of their cars. Some OEM's such as Tesla for example constantly log every ride of each car worldwide. 

The goal of this is to obtain a deeper knowledge of how we use our electric drivetrain. There aren't many, or even any scientific studies that focus on estate drivetrains, and a big part of the forum knowledge is just based on personal "feeling" and experience. 

Most of the forum builds are not comparable to prebuilt-estates, which in many cases (not counting Raptors) limit the way they are ridden, as they lack in power and range. Many of the builds are quite some beast witch rarely get to their power limits. This allows analyzing what really is required by experienced riders. At least in electrical terms ;) .  

What I have done till this point:

- **Preprocessing of the Data**: 
 I've written an e-Mail scraper (via google-script) for the study Gmail-address (esk8data@gmail.com) that will automatically save all submitted ride data.
It will also complete the database with the provided rider weight, as this is a critical factor on power consumption. 
All the raw data preprocessing steps are done on Matlab: Metr and Ack. log-files have to be structurally identical so that they can be simultaneously analyzed. 

Future steps: 

- **Processing of the data**: 
The first step will be to plot several scattering diagrams to get a general view of the data. After that, I'll prepare some more specific analyzes. I had planned to keep working with Matlab (as it was suggested by my tutors) but I recently spoke with someone who does data science for work and they suggested me to switch to Python. In his words: "using Matlab would be like trying to hammer a screw into a wall" 


I wanted to **integrate** the **telemetry data** of the **METR App** **and** all the other apps that save their logs on a .csv format, such as the **Ack. app and the eSkate-App** for example. 

**Submitting the data** (via Email) should be fairly easy: 
_****Mail**: esk8data@gmail.com**_ 

- **Metr App:** 
Copy & Paste the record-**URL** (or URLs, the more the better) and write your ride weight (with gear) like this: weight=80kg // or weight=180lbs  ((just don't forget the "=" sign))
Alternatively connect iPhone to Itunes and share the .r ending Record-Logs. Also add the weight in the mail
On android phones, it can be done via the file manager. 

![image|423x283](upload://hwerLQWVIU9ohoaztcmq9YcOCgR.png) 
**macos:**
![metr%20sharing|690x425](upload://wkoTmilDYdN9WIaajBICgL02yB1.jpeg) 
**android:**
![android%20sharing|281x500](upload://uXLi6vO9vnKqWGXr8gCbyGdvdwk.jpeg) 


- **All the other Apps:** 
Attach the .csv record files to the e-mail and add the rider weight like this:  weight=80kg // or weight=180lbs  ((just don't forget the "=" sign))
![image|445x363](upload://vw7Tk7DqCMexDBTd2d8viKZPe7F.png) 


General Information: 
- GPS Data will **not** be used (just the altitude values). 
- **No email address will be stored**. Once the data is saved all the emails are instantly deleted. 
- **All will remain strictly anonymous**. 
- Although It is a German University, **the text will be written in English**. This way everyone can read it. 
- The focus will lie on street builds (**no emtb's**)
- As for anything statistical the more datasamples are analyzed the better the results get at the end :D 

I would really appreciate suggestions (if you got any). If anything was left unclear please let me know. 


Thanks for reading :) 

Best, Mathias

Edit: 

as suggested by akhlut I've added an **optional** G-Form for the board configuration. This allows to do more detailed research: 
(If you complete this form please remember to add your forum name followed by the board ID when submitting telemetry via e-Mail:
@user1 for example) 

https://goo.gl/forms/9YkOTWiBAiwp4kgi1

Edit 2: 
[quote="bevilacqua, post:29, topic:73454"]
Open Database Files: [Link](https://drive.google.com/drive/folders/1V5F6_CeHETD8KmOQ9URazU5k292Xgf0R?usp=sharing)
[/quote]
These files do not contain latitude/longitude values. So they are completely anonymus. 
More info: 
https://www.electric-skateboard.builders/t/esk8-ww-field-study-statistical-analysis-of-telemetry-data-metr-ack-eskate-vesc-etc/73454/29?u=bevilacqua
```

---
## \#2 Posted by: akhlut Posted at: 2018-11-04T22:37:10.873Z Reads: 259

```
@mods. can we sticky this?

also, given that you're doing a statistical analysis consider anaconda which is python + R.

https://www.anaconda.com/download/#linux
```

---
## \#3 Posted by: bevilacqua Posted at: 2018-11-04T22:43:31.002Z Reads: 249

```
R was the other option so anaconda sounds great :) . Thanks
```

---
## \#4 Posted by: akhlut Posted at: 2018-11-04T22:45:18.369Z Reads: 247

```
i can see using python for data cleaning and transformations and R for the heavy lifting.
```

---
## \#5 Posted by: skatardude10 Posted at: 2018-11-04T22:48:19.728Z Reads: 245

```
You might find this interesting. I'll be submitting my logs. Can you take hundreds?

Oh I forgot to make a link! One sec

https://www.electric-skateboard.builders/t/community-survey-watt-hours-per-mile-on-your-configuration-real-time-update-graph-linked-inside/55172?u=skatardude10
```

---
## \#6 Posted by: bevilacqua Posted at: 2018-11-04T22:48:51.271Z Reads: 215

```
oh yes, please send them :blush:
```

---
## \#7 Posted by: Blix Posted at: 2018-11-04T22:52:16.330Z Reads: 212

```
Just wow! I wanna do something like this one day... I am still struggling with getting the most up to date parts for a remote(ervinelin remote).
:frowning: 
A teacher I have at school that is also teacher at a FH I don't know what a FH  is called in English also suggested us to learn python as a basic language. I forgot the arguments why, sorry.
```

---
## \#8 Posted by: pjotr47 Posted at: 2018-11-04T22:53:06.531Z Reads: 206

```
Good luck! If you are ready with everything, are you willing to share your analytics with us? :slight_smile:
```

---
## \#9 Posted by: bevilacqua Posted at: 2018-11-04T22:53:49.296Z Reads: 194

```
of course, everything will be shared, even the final thesis
```

---
## \#10 Posted by: akhlut Posted at: 2018-11-04T23:06:41.188Z Reads: 188

```
would you consider collecting board profile information as well?  cell type, battery configuration, etc?  if you provide us with a key that info can be stored in a separate file and we can use that key as a way to match our boards with the logs.  it could be something as simple as our usernames here.
```

---
## \#11 Posted by: bevilacqua Posted at: 2018-11-04T23:11:02.369Z Reads: 177

```
I wanted to keep is as simple as possible. People are lazy and don't want to write. 
**But**, you are right. I could fish out the usernames (from those who want to share it) out of the email. And then prepare a G-Form to add board data. 

Does it sound like a good Idea? Or better keeping it simple?
```

---
## \#12 Posted by: akhlut Posted at: 2018-11-04T23:12:17.904Z Reads: 175

```
the more variable you have under control the smaller your error becomes.  im assuming you'll be running a series of multivariate linear regressions, and maybe some matched pairs depending on your sample size.
```

---
## \#13 Posted by: mmaner Posted at: 2018-11-04T23:20:09.740Z Reads: 166

```

```

---
## \#14 Posted by: akhlut Posted at: 2018-11-04T23:20:36.532Z Reads: 168

```
thank you @mmaner!
```

---
## \#15 Posted by: mmaner Posted at: 2018-11-04T23:21:17.582Z Reads: 167

```
Pinned globally for a week, subject to @treenutter and @onloop approval.
```

---
## \#16 Posted by: bevilacqua Posted at: 2018-11-04T23:22:40.240Z Reads: 166

```
Wow, I will do my best to keep it there. I hope this can be helpful for the entire community
```

---
## \#17 Posted by: skatardude10 Posted at: 2018-11-04T23:30:26.279Z Reads: 165

```
Ah, I forgot to link what I intended with that post...

https://www.electric-skateboard.builders/t/esk8-ww-field-study-statistical-analysis-of-telemetry-data-metr-ack-eskate-vesc-etc/73454/5?u=skatardude10
```

---
## \#18 Posted by: Jc06505n Posted at: 2018-11-04T23:31:39.852Z Reads: 156

```
Does METR and the other Apps take local weather in their data , that’s a very important factor that affects the data
```

---
## \#19 Posted by: bevilacqua Posted at: 2018-11-04T23:35:19.272Z Reads: 152

```
no, I'm afraid that accessing the weather condition via the GPS data would be way to difficult
```

---
## \#20 Posted by: bevilacqua Posted at: 2018-11-04T23:46:40.952Z Reads: 150

```
https://docs.google.com/forms/d/e/1FAIpQLSdmq7JsnFFC0qkaYMT9OAd_hsLjPJPJNvVgUuggj2GuACXsdw/viewform



@akhlut does this look ok to you?
```

---
## \#21 Posted by: akhlut Posted at: 2018-11-04T23:56:10.448Z Reads: 137

```
looks good.

id just ask for motor size instead of radio buttons.  like ive got dual 6380's, which arent selectable.

i like the idea of data validation though.

also, there are some standard boards out there that should all be the same - like lacroix, raptor 2.0, etc.

im out and about now.  lemmie check it out from a pc.
```

---
## \#22 Posted by: bevilacqua Posted at: 2018-11-04T23:57:46.301Z Reads: 137

```
I'll modify it.
edit: Motor count should be = esc count
```

---
## \#23 Posted by: akhlut Posted at: 2018-11-04T23:58:49.428Z Reads: 139

```
survey design is a field unto itself.

also, maybe create a video about how to harvest the data from the vesc, esp the motor kv.

also, maybe add an 'other' to the prebuilts and a text box for the user to fill in.
```

---
## \#25 Posted by: sk8l8r Posted at: 2018-11-05T20:22:43.507Z Reads: 104

```
Will you share the data too? I would be really interested in it also for some ML 

Would be great if you get some logs with different types of failures!
```

---
## \#26 Posted by: bevilacqua Posted at: 2018-11-05T20:47:05.373Z Reads: 107

```
I could save it in a shared Google Drive folder. Only for those who are interested. 
Just DM me your email.
```

---
## \#27 Posted by: Jalapeno Posted at: 2018-11-06T10:08:38.066Z Reads: 95

```
Great idea m8!
In the google form please add other battery Ah ratings, please. E.g. I have some 4.5Ah hobby lipos.
I'd like to see the graphs you come up with!
```

---
## \#28 Posted by: bevilacqua Posted at: 2018-11-06T10:12:46.858Z Reads: 94

```
I’ll update it 👍🏻
```

---
## \#29 Posted by: bevilacqua Posted at: 2018-11-06T19:14:13.325Z Reads: 86

```
Open Database Files: [Link](https://drive.google.com/drive/folders/1V5F6_CeHETD8KmOQ9URazU5k292Xgf0R?usp=sharing)

As @sk8l8r asked for the files I've decided to share the database logs. These are preprocessed files that have the same structure as ack./eskate vesc app .csv files. The files d**o not contain latitude/longitude values**, so they are completely anonymous.  

I'll continue updating the database.

This is the file structure: 
![image|690x18](upload://fAZ9LrHmDlX0Vgh9yjuEyITpqav.png) 
All strings are overwritten by zeros so that it can be easily opened by csvread. 
The Cell R1C19 contains the weight data. R1C17 the number of vescs. 

The name of the files is the unix-timestamp of the start-time. Metr logs have only the start and end value. 


**Please keep sharing your logs** :) , the more files the better the results will get

I know that everyone wants shiny plots, just give me some time. 


Best, Mathias
```

---
## \#30 Posted by: akhlut Posted at: 2018-11-06T19:16:03.845Z Reads: 80

```
as soon as i get home!
```

---
## \#31 Posted by: Pedrodemio Posted at: 2018-11-06T20:07:39.752Z Reads: 80

```
@bevilacqua Nice endeavor, just sent you all logs I had

Do you have a time frame for completion? My graduation thesis is to engineer a hub motor for large urethane wheel (Gummies 125mm) and small pneumatics (6,5")

I had a plan to do something similar but much simpler and only with my data, would love to reference your work for all the goals and power/torque needs
```

---
## \#32 Posted by: bevilacqua Posted at: 2018-11-06T20:09:43.628Z Reads: 79

```
I hope I can have it finished by Jan. 2019. Then I'll work on something related to it on my master's thesis.
Thanks for sending the data :)
```

---
## \#33 Posted by: Pedrodemio Posted at: 2018-11-06T20:11:17.305Z Reads: 76

```
That's great, out of curiosity, what you plan to do on your master's?

I think we can soon open a thread to share all academic works being done on the esk8 topic
```

---
## \#34 Posted by: bevilacqua Posted at: 2018-11-06T20:18:45.603Z Reads: 70

```
The idea was to obtain the optimal values for a city commuting e-skate. Not just focused on the range calculated by some ideal wh/km figure. For example, do we even use the maximum capabilities of our batteries? What would be the minimum size to commute a set distance whilst having no power limitations? etc

I'd like to do something more hardware oriented on my master's thesis. Making a hub motor sounds great!
```

---
## \#35 Posted by: Pedrodemio Posted at: 2018-11-06T20:21:41.983Z Reads: 65

```
Following your idea the optimum esk8 you could not focus on the drive system, but in the board as a whole and them build it, it can be a pain to define the goal and set the weights for each criteria to get the best board for a given use case, but the result should be great
```

---
## \#36 Posted by: bevilacqua Posted at: 2018-11-06T20:24:56.435Z Reads: 67

```
yeah, average wh/km calculation is not exactly the goal. But rather to see how the battery is used. Combining that with some research papers of battery usage  (max current/time, max pulsed charge etc)
```

---
## \#37 Posted by: bevilacqua Posted at: 2018-11-06T20:34:58.813Z Reads: 75

```
@rpasichnyk Hi Roman, could the metr app have the feature to export all the records for a set module?

Not just for the sake of sharing it here, but to keep the ride urls sored in a place that is not the app. If the app gets deleted all will be lost. 
I, for example, lost all the ride data of my older module :/
```

---
## \#38 Posted by: rpasichnyk Posted at: 2018-11-07T08:43:20.543Z Reads: 67

```
You can export / import all the records (not just the URLs, but the data too) by copying `*.r` and `*.s` files from the application directory. For Android, you can use file manager or connect to your computer and copy. For iOS, connect to your mac and use iTunes File Sharing to transfer data.
```

---
## \#39 Posted by: bevilacqua Posted at: 2018-11-07T09:58:58.994Z Reads: 68

```
Wonderful :)
```

---
## \#40 Posted by: bevilacqua Posted at: 2018-11-07T19:41:46.051Z Reads: 77

```
Easier sharing of metr logs via macOS or android. Allows to select multiple files at once: 

**android:** 
![android%20sharing|281x500](upload://uXLi6vO9vnKqWGXr8gCbyGdvdwk.jpeg)
**macos:**
![metr%20sharing|690x425](upload://wkoTmilDYdN9WIaajBICgL02yB1.jpeg)
```

---
## \#41 Posted by: skatardude10 Posted at: 2018-11-07T21:27:31.872Z Reads: 70

```
So, I have a few questions @bevilacqua 

First, I have tons of logs from my board with a ton of different configs that I can't track down exactly when things changed. 16/32, 16/36, 20/32, 20/36... Ratios from 1.6-2.0 basically... 90mm, 107mm fly's, six shooters, 10-40A battery max, all scattered. Your board form is great, but I'm afraid I can't pin down what log correlates with what config, so for now I've just made one (my latest) config and submitted only those logs. My question- are all the other random logs useful to you? Now that I think about it, I remember Ackmaniac's csv files should include all the board settings data..  edit... It does! My CSV files all include the exact board data... Wheel size, gear ratios, battery amps... Do we really need an additional form or can your scripts maybe do a check for this data and automatically process it?

Second question... If your answer is should I submit them all now?
```

---
## \#42 Posted by: bevilacqua Posted at: 2018-11-07T21:44:09.239Z Reads: 70

```
yes, exported csv files include all the data. 
The google form causes a bit of confusion... **The main goal is to analyze how the battery/power is used**. It doesn't really matter what config you are running. The assumption I am making is that everyone uses more than "enough" power on their boards, at least 90% percent of the builders. 

To sum things up, I just need raw data, and lots of it, regardless of the board configuration.
```

---
## \#43 Posted by: bevilacqua Posted at: 2018-11-07T21:45:36.376Z Reads: 68

```
the G.Form just completes, even more, this open-database.
```

---
## \#44 Posted by: kuphjr Posted at: 2018-11-08T04:17:17.979Z Reads: 67

```
This will finally give me some motivation to start tracking my eskate data using Bluetooth! I’d love to be able to help you w/ my data.
```

---
## \#45 Posted by: mtuan293 Posted at: 2018-11-08T07:02:17.897Z Reads: 71

```
I have a bunch of logs using the Xmatic app by @twan. How to share? I have access to the files since I’m jailbroken, but also I don’t want to include location of these logs. @twan can you help me out? :grin: 
![image|281x500](upload://4DQlY06RyZBy4OMEyDZcySy5wtl.jpeg)
```

---
## \#46 Posted by: bevilacqua Posted at: 2018-11-08T08:48:22.322Z Reads: 65

```
I delete the location when I preprocess the files, so that the shared ones are completely anonymous
```

---
## \#47 Posted by: Pedrodemio Posted at: 2018-11-08T13:35:50.108Z Reads: 63

```
@bevilacqua just realized that I forgot to fill the form and should have put the 1 after the username

Should I send the logs again with Pedrodemio1 user?
```

---
## \#48 Posted by: bevilacqua Posted at: 2018-11-08T14:13:44.768Z Reads: 61

```
I'll add it manually, no problem
```

---
## \#49 Posted by: sk8l8r Posted at: 2018-12-05T15:36:23.066Z Reads: 47

```
a little bump for more data :)
```

---
## \#50 Posted by: bevilacqua Posted at: 2018-12-05T15:47:44.639Z Reads: 50

```
I found a bug when preprocessing, I'll update the files in 1h and add some more personal data.
```

---
## \#51 Posted by: sk8l8r Posted at: 2019-01-10T14:53:29.411Z Reads: 52

```
did this ever get updated I don't see much data
```

---
## \#52 Posted by: bevilacqua Posted at: 2019-01-10T15:05:22.814Z Reads: 52

```
Its all I got, I belive there should be ab 200 samples, I’ll check if the ones in the shared folder are ok

Edit: you could do your part and share your rides too 😜😜
```

---
## \#53 Posted by: bevilacqua Posted at: 2019-03-11T20:03:54.647Z Reads: 46

```
Hi, 


sorry I kinda forgot to post the promised work, I had my final meeting last week, where I got green light to freely post the entire work. 

Take a look if you are interested.  

Presented is some (rather simple) statistical analysis of the collected data as well as a Esk8 focused driving cycle (similar to a US-FTP75 or a WLTC).  

If you spot any errors or have questions please let me know.


https://drive.google.com/file/d/1GpvH5mNLKNiPzZFI7Yt3GtrS2A_SXDez/view?usp=sharing
(edited the link to exclude personal data)

Thanks again to all the guys who shared their data :) :)
```

---
## \#54 Posted by: Pedrodemio Posted at: 2019-03-11T20:33:56.621Z Reads: 43

```
Will go make some popcorn and then to go read it
```

---
## \#55 Posted by: bevilacqua Posted at: 2019-03-11T20:44:35.555Z Reads: 42

```
:D hehe thanks
```

---
## \#56 Posted by: janpom Posted at: 2019-03-11T20:52:59.878Z Reads: 42

```
Reading... Enjoying it so far... :slight_smile:

Do you care about some proofreading feedback? For example, there's this:
```
The MOSFET gate driver, DRV8302 or DRV8302,
```
and you're probably missing a reference here:
```
Jäger et al. for example used smart-phones...
```
```

---
## \#57 Posted by: bevilacqua Posted at: 2019-03-11T20:55:00.527Z Reads: 43

```
sure, as well, I'll correct it in later in Latex, thanks for letting me know, there has to be an error in the citation link
```

---
## \#58 Posted by: janpom Posted at: 2019-03-11T21:00:52.897Z Reads: 41

```
I started a google document [here](https://docs.google.com/document/d/11zJ4_ZALaMU2XgZjIMHgSWvVq1nRKDKdbu7aqnO4saw/edit?usp=sharing). I'll update it as I read. It's writeable for anyone in case other people want to contribute.
```

---
## \#59 Posted by: Sn4pz Posted at: 2019-03-11T21:06:56.842Z Reads: 40

```
Neat! 

When will the cut off date be for giving metrlogs? Ill have my board done in June and would like to participate :)
```

---
## \#60 Posted by: bevilacqua Posted at: 2019-03-11T21:10:18.376Z Reads: 36

```
Its all automated, to keep the database growing there is no deadline at all. 

This "pile" of data could be helpful for other users that need it to do some cool analysis. I'll maybe create another thread just to separate it from my personal work and to keep it alive

(Note.: I have to do some minor adjustment to do to the shared database, If you want to use that data please wait 1-2 Days)
```

---
## \#61 Posted by: Pedrodemio Posted at: 2019-03-11T21:17:32.707Z Reads: 38

```
Just saying that it's already on my ever growing folder of papers used as reference for my DD build

The drive cycle approach is really good, to be honest is all that I needed, a few weeks ago I was doing some thermal simulations but the input was just one ride of my board with a really coarse approximation using a series of steps

back to reading
```

---
## \#62 Posted by: Pedrodemio Posted at: 2019-03-12T00:22:09.520Z Reads: 39

```
Well done @bevilacqua 

I was going to ask for the driving cycle data but forgot to check the appendix  

One question, would be possible to easily extrapolate from the data a driving cycle that represent the let's say top 5% of top 1% more power intensive board/riders that would still be representative? or there is too little data on that top range?

My knowledge of statics is basic at most
```

---
## \#63 Posted by: bevilacqua Posted at: 2019-03-12T07:37:35.236Z Reads: 41

```
My guess would be that the database is not big enough select such a small percentage.  I have an exam Tomorrow but after that I can take a look and see what could be done, lets discuss it Tomorrow evening. 

Don't use the DC from the appendix, I'll post the CSV file later, that way you dont have to convert it form the text. I also could prepare one with a 2hz interval to smothen the curve a bit.
```

---
## \#64 Posted by: Pedrodemio Posted at: 2019-03-12T13:38:13.643Z Reads: 35

```
Thanks a lot, no hurry

My reasoning is that while the cycle you described it’s perfect for consumption, it wouldn’t be good for doing the thermal analysis, since a motor designed to stay within a reasonable temperature for the driving cycle, would probably overheat in demanding situations

The problem is how to define what is a extrema situation and how good it should perform under those conditions, I don’t thinking saying for example that it should climb a 20% grade for 1km at 35 km/h is representative or even a valid assumption at all
```

---
## \#65 Posted by: bevilacqua Posted at: 2019-03-12T15:41:18.323Z Reads: 33

```
what you could do is select the microcycles that have a higher consumption value than a target number, say for example 20wh/km, where the motor is supposed to be stressed more. Out of those pool of microcycles, you could create an "aggressive"-DC that suits your needs. 

Super easy to implement for me, just need time to perform the selection and generate the random data.
```

---
## \#66 Posted by: Pedrodemio Posted at: 2019-03-12T16:11:38.161Z Reads: 34

```
That would be perfect, and coupled with them I could also throw some steady state long hill climbs to determine what it can take

Let’s say it’s designed to optimally perform under this aggressive cycle but also can take the stress of edge cases without melting
```

---
## \#67 Posted by: skatardude10 Posted at: 2019-03-28T00:42:45.212Z Reads: 28

```
@bevilacqua awesome report! Just read through it, man that's some detailed data and analysis! 

After seeing the report I now wish I had submitted more data... I think I might have only submitted 3 csv files or something. Great stuff!! 

It'd be awesome if we had an open source repository/website where we could just bulk upload CSV files and have it automatically integrated into all sorts of community graphs, something akin to your report but real time
```

---
## \#68 Posted by: bevilacqua Posted at: 2019-03-28T12:10:32.112Z Reads: 22

```
The creation of the repository is definitely going to happen, have to take 1-2h this weekend to plan it. I would like to move the matlab preprocessing part to some kind of python cloud computing. 

I have sadly no Idea on how to do web-page oriented programming


Thanks for the feedback :)
```

---
## \#69 Posted by: Pedrodemio Posted at: 2019-03-28T12:43:10.234Z Reads: 21

```
That would be great

How about using a google docs spreadsheet set as read only, easy to plot everything, but no idea how to make it read your database, maybe just update it offline and upload once a month
```

---
## \#70 Posted by: bevilacqua Posted at: 2019-03-28T12:55:58.282Z Reads: 20

```
yeah, I only would have to open Matlab ab. once a week, the rest would happen automaticly. Some data interactivity would be nice, otherwise there is no attraction for users to submit data. They become lazy 😴
```

---

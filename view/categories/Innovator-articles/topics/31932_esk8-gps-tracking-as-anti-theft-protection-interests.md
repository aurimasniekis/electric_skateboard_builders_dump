# ESK8 GPS tracking as Anti-Theft protection: Interests

### Replies: 18 Views: 2544

## \#1 Posted by: TehAtheist Posted at: 2017-08-31T12:54:04.631Z Reads: 268

```
Hi,

Planning to develop a tracking system for my longboard, to prevent it from getting lost if stolen.

I'd do this by using an Arduino Nano on my ESK8 with a WIFI & GPS module.

I live in Belgium and our biggest internet operator has a service that has all it's modems have free WiFi for its other customers. So I can acces internet through WiFi basically as good as anywhere in any city with just one login.

This means I could get GPS coordinates from the GPS receiver, send them to a Raspberry Pi Linux server (that I'll soon create) by sending an HTTP request with the coordinates to my server from the Nano. And there it's easy to display these coordinates on a google maps view.

Question being, is anyone interested in everything that I do to make this?
If so, I'll try to document the code I write and keep everything documented to it's reproduce-able for others.
Be warned though, this won't be an allround fancy track system ;).
```

---
## \#2 Posted by: TarzanHBK Posted at: 2017-08-31T14:08:40.062Z Reads: 250

```
we just had a discussion about GPS yesterday and  @JLabs came up with a nice link:
https://www.kickstarter.com/projects/1851162219/magpie-the-smartest-truly-global-gps-tracker-aroun
```

---
## \#3 Posted by: TehAtheist Posted at: 2017-08-31T14:25:52.714Z Reads: 242

```
I've seen that. But that'll cost you 60$ a year.

I already have a Raspberry Pi and buying the Nano, Wifi module and GPS is like 15$ total from Ali express.
Can't really beat that price, although that Magpie will have a nicer interface and doesn't need the whole WiFi situation.

At the other hand, I'll be able to send live updates regarding information of my battery and perhaps VESC later on.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2017-08-31T14:29:41.616Z Reads: 231

```
good point! Haven´t seen their monthly plan and thought that it would only cost once.
```

---
## \#5 Posted by: karma Posted at: 2017-08-31T16:25:34.317Z Reads: 213

```
Greatscott has a video on such a project.
https://www.youtube.com/watch?v=CeStrH-5Llo&t=
```

---
## \#6 Posted by: Jammeslu Posted at: 2017-08-31T16:34:05.191Z Reads: 201

```
Arent there any of those small keychain attachable trackers?
```

---
## \#7 Posted by: overint Posted at: 2017-09-01T00:59:51.808Z Reads: 182

```
[quote="Jammeslu, post:6, topic:31932, full:true"]
Arent there any of those small keychain attachable trackers?
[/quote]

They don't have GPS, someone who uses the app & has bluetooth on has to be near the tag.
```

---
## \#8 Posted by: oct0f1sh Posted at: 2017-09-01T02:18:18.042Z Reads: 177

```
I used [this $20 tracker](https://smile.amazon.com/gp/product/B01KJS55JS/ref=oh_aui_detailpage_o07_s00?ie=UTF8&psc=1) on my last board and it worked really well. The only issue is that you need a sim card for it to work but you can get one at https://hologram.io/ really cheap:
https://i.gyazo.com/49ff777e15ec6610ae31b73e42a92017.png
```

---
## \#9 Posted by: cryo Posted at: 2017-09-01T02:38:13.326Z Reads: 172

```
Just heads up for people, even if you have a thief who stole your boards home location, the police probably will not do anything once the board is inside private property. The police can't legally enter if the person refuses a search and a judge most likely will not grant a search warrant for something small like an electric skateboard. 

This is for the US, dunno about other places.
```

---
## \#10 Posted by: mmaner Posted at: 2017-09-01T02:48:22.404Z Reads: 165

```
In Alabama the police will enter to confiscate your doughnuts 😀
```

---
## \#11 Posted by: jmasta Posted at: 2017-09-01T04:24:02.171Z Reads: 164

```
Go for it!  The huge disadvantage of those bluetooth tracking squares is they aren't likely to work many places.  And the GPS trackers require monthly subscriptions.  But you've already got Wifi across all of Belgium.  Sounds like a fun project. For $15 total, why not?!
```

---
## \#12 Posted by: skslingo21 Posted at: 2017-09-01T05:16:46.253Z Reads: 162

```
I wish i had some security in place besides the 2kilogram lock hanging off the front of my board :tired_face: 
<img src="/uploads/db1493/original/3X/1/4/142f80faab0517573f8901aaf7ee6f431a9ed60b.jpg" width="375" height="500">
Its necessary anway but I'd still bug the VESC's :smirk:

And once its confirmed my board is in a thieves possesion, I'd activate the self-destruct feature and give him a surprise between the legs on startup.
```

---
## \#13 Posted by: pedr0g0mes Posted at: 2017-09-02T05:10:25.372Z Reads: 139

```
I just got a GPS tracker from eBay 6€ , pay as you go card from guff gaff, and that's it, I pay 0.05€ for everything tracking I do but it works like wonders easy,reliable and cheap :p
```

---
## \#14 Posted by: TehAtheist Posted at: 2017-09-05T18:38:12.205Z Reads: 127

```
I've started the project and ordered everything that I need. I'll update this topic in the future with the results!
```

---
## \#15 Posted by: jmasta Posted at: 2017-09-07T03:25:09.851Z Reads: 126

```
Saw this on a bookface ad and it reminded me of this project.  Apparently it's a free SIM card service in the US.  Only $0.99 for the SIM card, and the free tier has 200 MB data per month, which would be plenty for GPS tracking only.  If it's legit, we could use @TehAtheist 's project here in the US too 

https://s3.amazonaws.com/images.freedompop.com/SEM+Assets/US_SIMVOICE_ZMP/USSVA+Ext_092017.png


I ponied up the $0.99, so we shall see if it works.  They accepted PayPal and had free super saver shipping, so very low risk.  What's the catch though????
```

---
## \#16 Posted by: jmasta Posted at: 2017-09-07T03:43:39.125Z Reads: 121

```
**Update:** Found the catch

They automatically enroll you in a trial of the "Premiere" account (2GB/month).  So you need to cancel the trial before it ends, or you get slapped with 6 months of service charges (~$100).  FYI...


.

<img src="/uploads/db1493/original/3X/d/4/d49716ccb7e4feaac95bd7f64d126f6861cd2b96.png" width="690" height="283">

.



Also:   Trial begins once it has shipped, and it takes up to 10 days to ship....

> **"REMINDER, your subscription start date begins once your device has shipped."**
...
>**Shipping Time: In some cases, orders may take up to 10 days to ship from our warehouse.**


**Update 2:**  Noticed they also charged me a second payment of $0.01, which seems harmless but it is actually authorization for a recurring payment.  Cancel this in your pre-approved PayPal payments, and then they won't be able to charge you extra later on
```

---
## \#17 Posted by: TehAtheist Posted at: 2017-09-07T09:16:46.279Z Reads: 114

```
That's a nice find :). I do hate how that website is made just to trick people into higher costs...
But if you can avoid it, then why not ;).
```

---
## \#18 Posted by: pixelsilva Posted at: 2017-09-16T05:51:00.683Z Reads: 103

```
<img src="/uploads/db1493/original/3X/2/e/2e9366f47be4688ee1cc7a1deeffaf2cefe3b361.jpg" width="675" height="450">
```

---

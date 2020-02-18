# No HTTPS (SSL certificate)?

### Replies: 30 Views: 2107

## \#1 Posted by: rmrf Posted at: 2016-10-31T14:45:04.179Z Reads: 137

```
I wonder why there is no option to visit this site through https (encrypted connection). I do not want airports to inject ads in the webpage and I definitely don't like the possibility of sniffing my password or private data.

SSL certificate is free these days https://letsencrypt.org
```

---
## \#2 Posted by: evoheyax Posted at: 2016-10-31T15:44:27.234Z Reads: 134

```
yea, I second that. I use lestencrypt to encrypt my sites, for example: https://www.rocketboards.club/

SSL is completely necessary these days...
```

---
## \#3 Posted by: JLabs Posted at: 2016-10-31T15:47:16.492Z Reads: 131

```
I also have an SSL on https://electric-skateboard.market

It is not totally necessary, and I am not sure if Discourse servers will allow @onloop to add it.
```

---
## \#4 Posted by: IDVert3X Posted at: 2016-10-31T15:54:38.272Z Reads: 125

```
Discourse allows you to use SSL...
But I just don't understand why anyone would use Discourse servers and not host it on an own one.
There are so many **affordable** options: Amazon web services, M$ Azure, Google Cloud, Digital Ocean...
Not only it's cheaper, but you have pretty much unlimited options in terms of software.
```

---
## \#5 Posted by: evoheyax Posted at: 2016-10-31T15:57:05.004Z Reads: 114

```
[quote="JLabs, post:3, topic:12200"]
It is not totally necessary
[/quote]


If you want any sort of privacy, it is. Otherwise, everything your sending via the internet is easy to read if intercepted (which is really when the NSA intercepts it, not if).

For sites like this, since were not using using credit cards here, it's less so important. But I'm sure a lot of private info is sent through PMs here that we wouldn't want out in the public domain...

@IDVert3X I use DreamHost. Extremely reliable and professional hosting. Not the cheapest (~$120 a year), but it's well worth the price (they use ssd in their servers now).
```

---
## \#6 Posted by: rmrf Posted at: 2016-11-02T12:58:35.750Z Reads: 86

```
Are you sure @onloop uses discourse hosting? https://payments.discourse.org/buy/ this? Looks kinda expensive. Considering that the only thing they do is deploy it on 5$/month digital ocean droplet. Total ripp-off.

I hope for such a price they at least install security updates for you. Not sure what else they do.
```

---
## \#7 Posted by: JLabs Posted at: 2016-11-02T13:27:38.929Z Reads: 84

```
Yes I am sure, it is hosted by discourse and imo this is the best forum I have visited, which you have to pay for.
```

---
## \#8 Posted by: rmrf Posted at: 2016-11-02T13:51:22.659Z Reads: 76

```
Discourse is free. You don't have to pay for it. You can install it for any purpose wherever you want. On any hosting. But the team behind it provides luxury service of installing it for you
```

---
## \#10 Posted by: mmaner Posted at: 2017-04-02T18:56:03.511Z Reads: 59

```
I have about had it with people that do nothing but bitch and cry about people that do something.

You don't have to be here, catch the fuck out if you don't like it.
```

---
## \#11 Posted by: flatsp0t Posted at: 2017-04-02T19:00:55.736Z Reads: 59

```
A bit harsh words for your third post on this forum.
But what would we expect, your first and second one were not that valuable either.
```

---
## \#12 Posted by: mmaner Posted at: 2017-04-02T19:04:02.991Z Reads: 55

```
He someone else's alt, to much of a coward to say what he wants without hiding.
```

---
## \#13 Posted by: makevoid Posted at: 2017-04-02T19:22:18.393Z Reads: 53

```
there is a drawback of http only - and that's the s in https - security

without https passwords and personal infos (pms) are transmitted w/o being encrypted so if you log in from a public wifi you can get people's password potentially just by listening to the wifi signal stream - that's why people that use this forum shouldn't use the same password on other websites (that's a good thing you should do in general btw) and/or shouldn't use pms as really private messages, because the information travels in clear

it would be nice to have https 

a single domain (ssl) certificate costs money usually (20$ year - only a standard certificate, no installation / configuration costs) but there's one free from letsencrypt.com - still the web-server (and/or the forum app, discord) has to be configured to use ssl (https) - here's the link to a  [guide](https://meta.discourse.org/t/setting-up-lets-encrypt/40709) / [guide-docker](https://meta.discourse.org/t/allowing-ssl-https-for-your-discourse-docker-setup/13847) - as you can see is quite a bit of work but it would be cool - if somebody is very interested in this feature and can, probably should contribute economically to it as Jason is paying for maintainance and hosting of this forum I guess
```

---
## \#14 Posted by: UserName0 Posted at: 2017-04-02T19:27:13.929Z Reads: 52

```
My posting history has nothing to do with the topic, since the posts about this are very old generalizing as careless is completely accurate. Incompetence can be argued since Enerions website has it.

pointing out this and getting attacked for it is stupid. Yes I am new here so when I see that its not HTTPS I saw posts and people asleep at the wheel I said something. The issue is not going away.
```

---
## \#15 Posted by: flatsp0t Posted at: 2017-04-02T19:36:19.653Z Reads: 52

```
Well, as it is hosted, it may be easier.

@UserName0 
[quote="UserName0, post:14, topic:12200"]
pointing out this
[/quote]

Well, if that is your way of pointing something out, you will be a very welcome user at this forum for sure.

Or to say it in your words:

Seriously.... WTF
Unkindliness & social incompetence (Sorry, did not find a single word for that.)
```

---
## \#16 Posted by: UserName0 Posted at: 2017-04-02T19:54:19.475Z Reads: 50

```
[quote="flatsp0t, post:15, topic:12200"]
Seriously.... WTFUnkindliness & social incompetence (Sorry, did not find a single word for that.)
[/quote]

Guilty.. I read more post less

Doesn't change anything about the topic. I am in on a group buy here (your analysis didn't pick that up from my post count) so considering things like this topic are of concern and should be for others. Just general internet usage.
```

---
## \#17 Posted by: flatsp0t Posted at: 2017-04-02T20:05:13.760Z Reads: 49

```
Well, yes this is an important topic, you are correct in that point.

 It's not what you say, but how you say it.
```

---
## \#18 Posted by: mmaner Posted at: 2017-04-02T21:59:15.279Z Reads: 44

```
I'm aware of the plications of HTTPS, I'm a systems engineer with 37 certifications and 2 degrees.   I've been a systems engineer for 25 years...So I dig it.

The issue is someone coming here that's made absolutely no contribution to community throwing around "Incompetence & carelessness".  

If he wants to help then offer to buy the certificate.  If not, catch out.  

Now, to be constructive.  If you want alleviate the concerns about pilfered passwords and someone capturing your personal passwords by doing a capture on open traffic, then get a personal VPN service.  I use one everytime  on the internet u less I'm on my home or corp network.
```

---
## \#19 Posted by: mmaner Posted at: 2017-04-02T22:05:36.213Z Reads: 45

```
[quote="UserName0, post:14, topic:12200"]
Incompetence can be argued since Enerions website has it.
[/quote]

Wrong.

If you don't like it, don't visit.  @onloop has no legal or moral obligation to secure your http requests.  Since you know so much, you should know that securing your internet traffic is your responsibility.  That's why anti-virus and anti-malware are billion dollar businesses. 

Personally, I think it was a dick move to say "Incompetence & carelessness" about someone who has never asked you for anything, is actively doing you a favor by hosting and maintaining this site and made the group buy your in (that for some reason makes you legit???) possible.

If it was up to me I'd comb the Apache logs and match up your logins to the WAN IP addresses they originate from and BAN them as well as your account for the sole reason that your a mooch and a dick...very unlucrative combination.
```

---
## \#20 Posted by: UserName0 Posted at: 2017-04-02T22:14:45.116Z Reads: 46

```
your way over the top 

IP ban lol ok.. 

looks for ignore button
```

---
## \#21 Posted by: mmaner Posted at: 2017-04-02T22:17:22.989Z Reads: 45

```
[quote="UserName0, post:20, topic:12200"]
IP ban lol ok..
[/quote]

You think it can't happen?  I do it weekly in my network.  Be glad to help @onloop learn how to do it as well. 

[quote="UserName0, post:20, topic:12200"]
looks for ignore button
[/quote]

Need help finding it?  Hint, start with alt+f4.
```

---
## \#22 Posted by: UserName0 Posted at: 2017-04-02T22:20:58.071Z Reads: 44

```
go ban 127.0.0.1 or something your funny
```

---
## \#23 Posted by: onloop Posted at: 2017-04-03T01:07:38.942Z Reads: 41

```

since you asked so nicely I'll look into adding a ssl


also, try not to be a dick & try not to start fights on here please....
```

---
## \#24 Posted by: UserName0 Posted at: 2017-04-03T01:21:09.045Z Reads: 42

```
The first post from months back mentioned a free automated service.
```

---
## \#25 Posted by: onloop Posted at: 2017-04-03T01:24:22.463Z Reads: 41

```
it's not really automated, you still need access to the server, I don't host this site so don't really have the access. I don't have time to fuck around with maintaining this website so I pay people to do that shit for me, i have asked them to install one.
```

---
## \#26 Posted by: rwxr Posted at: 2017-04-03T06:17:04.630Z Reads: 31

```
HTTPS works now. However a redirect from HTTP -> HTTPS seems to be missing.
```

---
## \#27 Posted by: flatsp0t Posted at: 2017-04-03T06:22:57.327Z Reads: 31

```
Doesnt everyone use HTTPS Everywhere anyways?
```

---
## \#28 Posted by: flatsp0t Posted at: 2017-04-03T06:23:59.139Z Reads: 30

```
Thank you. :thumbsup:
```

---
## \#29 Posted by: rwxr Posted at: 2017-04-03T06:37:01.068Z Reads: 30

```
Most people do. But cached links and old bookmarks will still use http :)
```

---
## \#30 Posted by: flatsp0t Posted at: 2017-04-03T06:40:25.122Z Reads: 32

```
Sorry to be Unclear, i meant the [HTTPS-Anywhere](https://www.eff.org/HTTPS-Everywhere) browser Plugin.
```

---
## \#31 Posted by: laurnts Posted at: 2017-04-03T08:28:39.866Z Reads: 28

```
If you want to use public wifi without being monitored use VPN sevice. If you want ip hopping use Tor browser instead. If you use both, https doesnt matter so much.

Https does encrypt communication to a certain level. Encrypt content, validate companies, etc but if you want safe browsing. Vpn is the way to go.
```

---

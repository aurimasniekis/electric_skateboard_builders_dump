# Prices - with or without VAT?

### Replies: 33 Views: 411

## \#1 Posted by: DavidBanner Posted at: 2019-03-19T18:23:21.877Z Reads: 142

```
A recent discussion got me to thinking about how to display prices on product pages.

My thinking is that it is better to include the VAT on prices on the product page for retail customers as it feels more honest and upfront, so that is the way I have set up things on the Street Wing website. 

The potential problem with this is that if other sites are only adding the VAT at checkout it makes the prices seem higher than they really are when customers are comparing prices unless they get as far as the checkout page on all of the sites they are looking at.

But I would really welcome your thoughts on this.

[poll type=regular results=always public=true]
* Product page should include prices WITHOUT VAT
* Product page should include prices INCLUDING VAT
[/poll]
```

---
## \#2 Posted by: Klaerke91 Posted at: 2019-03-19T18:24:59.139Z Reads: 136

```
there are ways of having both if your users can have accounts. Needed to be supported by the website of course
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-03-19T18:26:15.179Z Reads: 131

```
I always liked the 3Dservisas approach to it
![image|371x255](upload://rOwUx2GgTbiAUiSkj4b7zchKBsE.png)
```

---
## \#4 Posted by: DavidBanner Posted at: 2019-03-19T18:26:52.018Z Reads: 127

```
[quote="Sn4pz, post:3, topic:87655, full:true"]
I always liked the 3Dservisas approach to it
[/quote]
that is pretty cool! it's all very clear and upfront
```

---
## \#5 Posted by: banjaxxed Posted at: 2019-03-19T19:32:49.203Z Reads: 113

```
I think there is legislation to have vat inc prices where appropriate ie business to person scenario, of course you are welcome to make a clearly indicated vat ex price, like most uk sites
```

---
## \#6 Posted by: High-roller Posted at: 2019-03-19T20:00:43.862Z Reads: 104

```
I don't understand why this is still a thing?? 
Since the customer is going to pay the VAT either way it only makes sense to include it in the price from the beginning. I'm actually more likely to cancel an order if I see a "surprise" VAT charge tacked on at the last minute. Just tell me what total is from the outset, and I'll decide if I want to spend that much.
C'mon USA, this is just ridiculous.
```

---
## \#7 Posted by: DavidBanner Posted at: 2019-03-19T20:56:14.454Z Reads: 94

```
[quote="High-roller, post:6, topic:87655"]
Since the customer is going to pay the VAT either way it only makes sense to include it in the price from the beginning.
[/quote]
that is the way I think and "best guess" as to what customers may think. Of course not everyone is doing it that way and Street Wing is being accused of "HIGH margins" when the final price is actually cheaper than other sites in the EU.

And now I have found potential a new bug with the site where it's displaying the +VAT figure for non-EU customers on the product page.

Can any non EU people please confirm the price is £124 (as it should be ex-vat_ for them on the product page: https://street-wing.com/product/enertion-focbox-vesc-x/

I tried using a proxy but am not sure it's working as expected
```

---
## \#8 Posted by: BoostedBuilder Posted at: 2019-03-19T21:33:38.173Z Reads: 75

```
Yes, it's £124 for me
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-03-19T21:36:23.450Z Reads: 72

```
Yep its 124 pounds.
```

---
## \#10 Posted by: Sn4pz Posted at: 2019-03-19T23:23:25.398Z Reads: 71

```
![image|525x500](upload://6SJsTIhUdotVVjnwsj9UtiBtvQw.png) 

124 pound
```

---
## \#11 Posted by: DavidBanner Posted at: 2019-03-20T14:30:51.858Z Reads: 62

```
@BoostedBuilder @AlanZhou @Sn4pz   thanks for checking, looks like the geo location script  is working :)
```

---
## \#12 Posted by: Gerrycorrado Posted at: 2019-03-20T15:08:57.306Z Reads: 62

```
I must say I found it very "annoying" to look at the price. I did not really know why.
Until I looked at a site mentioning VAT inc and ex VAT in between (). -> looks normal and professional.
I would really hesitate to buy from a site not mentioning the 2. (my personal 2cents, ah yes, I live in europe, maybe more comon)
```

---
## \#13 Posted by: DavidBanner Posted at: 2019-03-20T18:39:42.781Z Reads: 56

```
thanks for all the feedback everyone.

this is what I've implemented:
![image|690x330](upload://hYWXBADdtdJG6VoPurGX0lrZ7Ad.png)
```

---
## \#14 Posted by: Sn4pz Posted at: 2019-03-20T18:43:32.565Z Reads: 56

```
Looks good. Maybe highlight the price relative to if the country theyre loading the webpage from to reflect the price they would pay?

I dont know how this works, the above people made it seem like both prices need to be reflected, but making the correct one catch the users eye might be an worthy addition
```

---
## \#15 Posted by: DavidBanner Posted at: 2019-03-20T18:45:08.982Z Reads: 55

```
[quote="Sn4pz, post:14, topic:87655"]
aybe highlight the price relative to if the country theyre loading the webpage from
[/quote]
the site uses geolocation for users, the big price will include VAT for EU users and will be exclusive of VAT for those outside the EU
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-03-20T18:57:10.628Z Reads: 52

```
I suppose it works, but for someone in the USA who doesnt know how you want it to work, I think they might assume that the price is still with vat, and push them to contact you... extending the process and taking away from the function of the feature

![image|489x500](upload://5YfzlsLkSCwceeCIYGbeToPuY7T.png) 

![david%20ver%201|690x330](upload://gvdWvO8kBK7SDt6hpckf0DI3Oik.png) 


![david%20ver%202|690x330](upload://aAfnCKRn1xPlqvx1soQHZe8ptws.png) 
this is what i mean

or even this

![david%20ver%203|690x330](upload://88Hfls2ZjyWbPzKVWgQ1ATqYjAN.png)
obviously with the euro symbol... im lazy.
```

---
## \#17 Posted by: Blitz Posted at: 2019-03-20T19:21:03.362Z Reads: 47

```
I hate when companies list prices without vat.
or first show without vat and then with.
```

---
## \#18 Posted by: Chrisjarram Posted at: 2019-03-21T07:28:15.880Z Reads: 45

```
There's no such legislation no - so long as the VAT is declared separately on the invoice that's all that is required.
```

---
## \#19 Posted by: taz Posted at: 2019-03-21T07:41:51.429Z Reads: 46

```
Actually there is:

http://www.legislation.gov.uk/uksi/2008/1277/regulation/5/made

Check 5(4)g
```

---
## \#20 Posted by: banjaxxed Posted at: 2019-03-21T07:46:39.091Z Reads: 46

```
http://www.legislation.gov.uk/uksi/2004/102/contents/made

Edit. Same
```

---
## \#22 Posted by: taz Posted at: 2019-03-21T10:15:44.809Z Reads: 39

```
A lot of the example mentioned did/do not provide any information as to the inclusion of additional taxes.

That is misleading and therefore illegal in most EU countries.
```

---
## \#23 Posted by: Chrisjarram Posted at: 2019-03-21T10:18:52.799Z Reads: 37

```
That's correct yes
```

---
## \#24 Posted by: Chrisjarram Posted at: 2019-03-21T10:21:19.035Z Reads: 37

```
Yep what I meant was you don’t have to explicitly provide the calculation on the listing page; you do have to state ‘prices exclude vat’, but there is no specific legislation that requires the prices be listed inclusive of vat for B2C sales… just that you include it along with your VAT number (if registered) on the invoice.
```

---
## \#25 Posted by: taz Posted at: 2019-03-21T10:21:59.207Z Reads: 36

```
Agreed.
10 char
```

---
## \#26 Posted by: banjaxxed Posted at: 2019-03-21T11:01:15.624Z Reads: 32

```
Hey on the upside pretty soon all non domestic sales will be vat ex 😂

Sorry unresistable
```

---
## \#27 Posted by: DavidBanner Posted at: 2019-03-21T11:16:55.637Z Reads: 32

```
[quote="banjaxxed, post:26, topic:87655"]
Hey on the upside pretty soon all non domestic sales will be vat ex
[/quote]
LOL! 

Well maybe, I don't think anyone has any idea what is actually going to happen.

Man what a complete clusterfuck this whole brexit thing has turned into...
```

---
## \#28 Posted by: banjaxxed Posted at: 2019-03-21T11:40:34.262Z Reads: 28

```
Must be the last hurrah of the scrote daily mail brigade twinned with the surviving Alf Garnett’s & some confused blue rinsers. Basically anyone who doesn’t have to go out and actually make a living in this world.

Shocking it came to this, I always thought of the UK as quite swish and multicultural 

Just remembered I must put in for this years EU grant & print off some ☘️ passports busy busy
```

---
## \#29 Posted by: DavidBanner Posted at: 2019-03-21T11:51:05.475Z Reads: 29

```
[quote="banjaxxed, post:28, topic:87655"]
Shocking it came to this, I always thought of the UK as quite swish and multicultural
[/quote]
The problem is the people who sit in parliament may as well be a different species to the rest of us. Most of them are millionaires through inheritance, educated at private schools and have no idea what it's like to be a "normal person". They play the system to benefit themselves and from what I can see seem to not care in the slightest about the damage they inflict.

These are not normal people, let's face it you would have to have something very wrong with you to be sitting on millions and never needing to work but choosing to be a politician. I would need to be forced at gunpoint to do that job and if I was sitting on that sort of money with a phonebook full of the sort of contacts they have I would spend the limited time I have on earth in a much better way.

Not one of the politicians in this country own an electric skateboard, which tells you everything you need to know right there :)
```

---
## \#30 Posted by: briman05 Posted at: 2019-03-21T15:48:28.167Z Reads: 21

```
I dont understand the whole VAT thing.
```

---
## \#31 Posted by: DavidBanner Posted at: 2019-03-21T16:13:27.982Z Reads: 22

```
VAT is a sales tax, businesses who are VAT registered must charge this on top of the total of the order (including shipping) and then pay that to the government or they come round and poke you with sharp sticks and take your stuff.

Customers who are outside of the EU do not get charged VAT on their orders.
```

---
## \#32 Posted by: briman05 Posted at: 2019-03-21T16:56:03.396Z Reads: 21

```
See in the US most states have a sales tax but you can only charge the sales tax if you have a presence in the state. Thus the reason you get charged tax for a Amazon order but not for a ebay order.  I think there are like 3 states that dont have a sales tax.  I just find it so weird that it is every country in the EU that has that.  You could always become a sovereign citizen.
```

---
## \#33 Posted by: DavidBanner Posted at: 2019-03-21T17:17:42.343Z Reads: 20

```
[quote="briman05, post:32, topic:87655"]
You could always become a sovereign citizen.
[/quote]

and miss out on all the fun of being forced to collect taxes on behalf of the government without being paid for it?
```

---
## \#34 Posted by: briman05 Posted at: 2019-03-21T20:40:21.355Z Reads: 16

```
https://media1.tenor.com/images/4f13be73444567507a0e690214a5270f/tenor.gif?itemid=3327538
```

---

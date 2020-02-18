# Heat treatment of aluminium (T4, T5, T6, &hellip;. total confusion)

### Replies: 22 Views: 3310

## \#1 Posted by: Schulerbible Posted at: 2018-04-30T10:52:17.388Z Reads: 124

```
Hi,

Anybody here who has some knowledge about heat treatment of aluminium, specifically AL6061? I would like to take advantage of an online service to machine a few parts out of Al6061. Unfortunately, the specification on the source material is quite sparse, and hence I would like to know what the common process is to achieve the T6 temper? So, do I have to heat treat the material afterwards or how does it usually work?

Thx
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-04-30T11:38:33.591Z Reads: 110

```
“This involves two steps—solution heat treating and aging. Solution heat treatment is done by raising the alloy temperature to about 980 degrees F and holding it there for about an hour. ... This heat treatment is called aging, which results in material with a T6 temper.“
```

---
## \#3 Posted by: L3chef Posted at: 2018-04-30T11:45:13.975Z Reads: 102

```
You want to treat the material befor manufacturing your part[s]
@GrecoMan is right on the process
```

---
## \#4 Posted by: Schulerbible Posted at: 2018-04-30T11:51:20.307Z Reads: 98

```
So, then I assume the company who provides the service uses the heat treated material already? But what temper is it, T4 or T6? Also, ....

> So we have a solid solution of magnesium, silicon, and other elements in aluminum at room temperature. This is called the T4 temper. If we take this material and heat treat it at a temperature between 325 and 400 degrees F, the alloying elements begin to form ordered arrays of atoms in the aluminum matrix. These arrays are called GP zones, and they strengthen the aluminum considerably. This heat treatment is called aging, which results in material with a T6 temper.
> 
> Three commonly used time/temperature cycles are used for aging—one hour at 400 degrees F; five hours at 350 degrees F; and eight hours at 325 degrees F. All are equally effective.
> 
> The question, however, is whether you can perform this yourself. There is no doubt that the result will be 6061-T6 properties if you do it properly. The main difficulty is that the component usually distorts quite a bit during quenching and requires significant mechanical straightening before aging.

(Source: https://www.thefabricator.com/article/aluminumwelding/achieving-t6-designation-for-6061)

Bit worried about the "usually distorts quite a bit" bit ....
```

---
## \#5 Posted by: Ronny_CTS Posted at: 2018-04-30T12:18:04.644Z Reads: 72

```
You should buy a block of material that is already heat treaded and then machine your parts out of it. Or else you will get part distortion due to the high temps of the treatment process.
```

---
## \#6 Posted by: LukePL Posted at: 2018-04-30T12:29:10.108Z Reads: 70

```
For milling use T6. For example if you want to make a bike frame than you use T4 for bending and welding because it's softer. Welding will bend the material so you'll have to make mechanical correction to have all correct measurements. After that you put those into big owen and do heat treatment and maybe after that you will require slight correction again but much less than before. Same is with extruded profiles. They are all T4 after pressing them and goes for the treatment. Never heard about need of correcting them after that (not sure if it's possible even). There's also T66 which is better than T6 :slight_smile:
What do you want to do and what process you want to use?
```

---
## \#7 Posted by: Schulerbible Posted at: 2018-04-30T12:30:55.894Z Reads: 70

```
The thing is, I just can't buy the material and then send it to 3D hubs to machine my parts.
```

---
## \#8 Posted by: Schulerbible Posted at: 2018-04-30T12:32:29.972Z Reads: 71

```
Milling parts out of Al6061 through 3Dhubs:

https://www.3dhubs.com/cnc-machining
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-04-30T12:36:29.533Z Reads: 68

```
because i’m a nosy fucker, what you makin?
```

---
## \#10 Posted by: Schulerbible Posted at: 2018-04-30T12:37:22.425Z Reads: 66

```
Maybe my truck hangers. How do you do it?
```

---
## \#11 Posted by: LukePL Posted at: 2018-04-30T12:37:53.794Z Reads: 62

```
Just use T6 as stock material. I would suggest to use 6082 alloy which is not much more expensive but stronger than 6061. For hanger I would go with 7075 ;)
```

---
## \#12 Posted by: Schulerbible Posted at: 2018-04-30T12:46:14.938Z Reads: 60

```
Ok, I found this: 

https://www.3dhubs.com/knowledge-base/heat-treatments-cnc-machined-parts#author
```

---
## \#13 Posted by: GrecoMan Posted at: 2018-04-30T12:47:36.749Z Reads: 59

```
just something to keep in mind - the actual 3dhubs final prices are higher than the initial quote they give you
```

---
## \#14 Posted by: Schulerbible Posted at: 2018-04-30T12:55:09.702Z Reads: 59

```
Hmm, they differ actually widely from quote to quote. Some day my quote is $200 cheaper for the exact same part compared to a few days earlier (might be a bug in the system).  In general, my quotes are appox. $30-50 more expensive as I have some tolerances in the 2d drawing. Also, when I submit the actual *.ipt file rather than a STEP file, the online calculator gives me a more accurate offer.
```

---
## \#15 Posted by: Schulerbible Posted at: 2018-04-30T13:04:35.038Z Reads: 54

```
My local anodizer doesn't like 7075 since:

![image|690x70](upload://cAUUEsGkZjTofQtv4STOXJKI61k.png)
```

---
## \#16 Posted by: Schulerbible Posted at: 2018-04-30T15:16:31.086Z Reads: 49

```
Got a reply from 3Dhubs, just in case somebody wants to know:

![image|690x46](upload://vDoNPDmueFDPmeHFkFCsPqzu5uf.png)

I assume 8082 = 6082 :slight_smile:
```

---
## \#17 Posted by: LukePL Posted at: 2018-05-01T08:32:08.093Z Reads: 39

```
Yes probally 6082 ;) So you have all you need. I just hope that price won't kill you ;)
```

---
## \#18 Posted by: Minim Posted at: 2018-05-01T10:26:49.944Z Reads: 36

```
If my customers demand it I order my stock materials with material certificate showing all needed info about the stock. I tested it once but never used the certificate.. I would assume that this is possible everywhere. I’m just starting out in the cnc business and this far my customers have been satisfied with me signing off that I use (as an example) 6061. I guess bigger more important ones demand a certificate :)
```

---
## \#19 Posted by: Schulerbible Posted at: 2018-05-01T11:51:58.444Z Reads: 34

```
It will be expensive but I got only one board, so why not putting all the $$$$ into one 😀
```

---
## \#20 Posted by: GrecoMan Posted at: 2018-05-01T21:07:10.626Z Reads: 31

```
you should send me 1 to compare to my hangers 😉
```

---
## \#21 Posted by: chuttney1 Posted at: 2018-05-02T01:38:09.033Z Reads: 24

```
[quote="Schulerbible, post:16, topic:53916"]
I assume 8082 = 6082
[/quote]


8082 /= 6082 from an alloy composition and material's properties point of view. Unless this was about price point.
```

---
## \#22 Posted by: Schulerbible Posted at: 2018-05-02T03:07:52.756Z Reads: 23

```
Yeah, don't you think I would know that? Also, 3Dhubs offer 6061, 6082, 7075 and 5083 only. Hence, clearly a typo.
```

---

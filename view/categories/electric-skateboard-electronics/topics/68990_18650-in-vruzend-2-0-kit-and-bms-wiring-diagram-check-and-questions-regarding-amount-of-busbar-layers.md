# 18650 in vruzend 2.0 kit and BMS wiring diagram check and questions regarding amount of busbar layers

### Replies: 19 Views: 1238

## \#1 Posted by: Joris Posted at: 2018-09-23T18:57:11.747Z Reads: 144

```
Hi!

So this is my first build. Before Im going to assemble the battery using Vruzend 2.0 kit and 18650 samsung 30Q 3Ah cells I visuealized the connections in a powerpoint (and the subsequent image below). I have a few questions regarding the diagram / connections. 

- So the 18650 cells are placed in the Vruzend Kit 2.0. These are connected with busbars. The advise on the website is to use an extra busbar for the series connection for the amount of parallel cells. So a 3p connection to a 3p should have 3 busbars. My question is: do the parallel connections also need 3 busbars. I can't seem to understand how this theoretically works :/ 
- Is this the best layout for the cells? It fits exactly in an Ikea Stodja in this configuration and to me it seems the best layout. I'm wondering if there are any other suggestions.
- Any comments on the wiring diagram?

thanks!

![build%20layout|690x345](upload://4YSaTWRJUgadhQOpQA1vUY4cgJP.jpeg)
```

---
## \#2 Posted by: Andy87 Posted at: 2018-09-23T19:06:22.129Z Reads: 131

```
I thought I read something here that this vruzend holders not a good solution for our purposes of esk8ing... it was because they can’t handle the current or because they became lose from vibration
```

---
## \#3 Posted by: ethel Posted at: 2018-09-23T19:07:46.614Z Reads: 131

```
If you do a search query on this battery pack build, you will find useful information on the pros/cons. One of the issues is how do these packs hold up on vibration from the esk8. 

I don’t see balance wires from pack to BMS in your drawing.

This video helped me learn more about this process:

https://m.youtube.com/watch?v=1D90heZ8z4s
```

---
## \#4 Posted by: Andy87 Posted at: 2018-09-23T19:14:08.722Z Reads: 124

```
Here is the thread to it
https://www.electric-skateboard.builders/t/vruzend-battery-diy-kit-questions/37259/17?u=andy87

24a max they say. With your 3p pack you could be able to output 60a if you would want.
```

---
## \#5 Posted by: Benjamin899 Posted at: 2018-09-23T19:52:24.264Z Reads: 115

```
24A per Cell.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-09-23T20:01:41.019Z Reads: 113

```
And what with the serial connections?
For them you use bigger copper or wires?
I didn’t read in deep in this topic so i‘m just interested.
I mean it can’t add up 24a with every cell you add in your pack. 
If you have a 3p pack the max current you can get out of your pack it’s 60a or 20a per cell in every serial pack but through every serial connection it will flow 60a...
```

---
## \#7 Posted by: Benjamin899 Posted at: 2018-09-23T20:09:15.114Z Reads: 102

```
the tabs are also made out of copper to carry more amps.
```

---
## \#8 Posted by: Andy87 Posted at: 2018-09-23T20:12:19.086Z Reads: 98

```
I thought the taps out of copper can handle 24a.
Than there is still the question how the serial packs connected? Can you add for them extra layers of copper?
```

---
## \#9 Posted by: ethel Posted at: 2018-09-23T20:12:33.433Z Reads: 98

```
@Benjamin899

Did you build a back with these?
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-09-23T20:19:18.840Z Reads: 97

```
the busbars are made out of copper and sure you can stack them.
@ethel no i went with NESE since i wanted to build a 10s4p pack. It was a better choice and i am very happy with it.
```

---
## \#11 Posted by: Joris Posted at: 2018-09-24T06:19:41.492Z Reads: 92

```
@ethel thx, I put numbers on where the balance leads go, as it was otherwise to messy a diagram :stuck_out_tongue:

@Andy87 On the concern of the vibrations: I'm aware. This might be a problem. I'm just going to use a lot of tie wraps, hot glue and heat shrink to keep the pack together. Also if there is room I'm covering them with something extra to hold it together. Then see if it works :slight_smile:

 So if i understand correctly I also need to beef up the parallel connetions.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-09-24T06:26:03.178Z Reads: 86

```
the serial connectiones.
in parallel the current will divided through your cell count so the 24a copper strip should be enough. 
but in serial all current flows through that one connection from your parallel pack1 to parallel pack2, so in this point i would say it´s recommended to add up the copper strips.
```

---
## \#13 Posted by: Joris Posted at: 2018-09-24T06:54:42.467Z Reads: 83

```
great thanks for the advice. I'm still puzzling on how this theoretically works, but at least i know this is enough. Back to the physics-book i guess :p
```

---
## \#14 Posted by: mishrasubhransu Posted at: 2018-09-24T07:14:15.503Z Reads: 81

```
If you haven't already bought the modules, I strongly recommended getting the NESE module instead.
```

---
## \#15 Posted by: Joris Posted at: 2018-09-24T07:15:16.144Z Reads: 81

```
thx, but i already have the modules. so first trying it like this :expressionless:
```

---
## \#16 Posted by: ethel Posted at: 2018-09-24T07:37:23.701Z Reads: 78

```
You could always make a sick ebike triangle battery pack
https://m.youtube.com/watch?v=clawhNsORts
```

---
## \#17 Posted by: Faceplant Posted at: 2019-05-04T09:52:00.035Z Reads: 38

```
How did that work out for ya?
```

---
## \#18 Posted by: Joris Posted at: 2019-05-04T19:11:41.552Z Reads: 34

```
Ah yes, I completely forgot to post anything on this forum about this as building te eboard took quite some time longer then expected haha. But it is finished with the vruzend 2.0 kit. 
Put some extra foam around it as shock-absorbers, hot-glued all the parts & tie-wraps. 

Only thing I did not think of before and really annoyed me was the size the battery pack gets when using this kit.

I've used the board for about 20km now (only riding in good, dry weather and the board is finished a couple of weeks ago) without any problems. Will do an update in a couple of months if the thing is still working.I'll also post a small piece about my build and the problems with it.
```

---
## \#19 Posted by: HarryForks Posted at: 2020-01-23T21:53:40.560Z Reads: 8

```
Any update on this Vruzend kit? How's it holding up? Still going strong or did it cause problems further down the line?

I'm looking to purchase 2x the V2.1 kit (with joining barrels bolts) soon for my 12s5p project.

I would go with the NESE kit, but I want to keep my options open for the future, in case i decide to add more cells in parallel.
```

---

# Battery Calculator Spreadsheet

### Replies: 14 Views: 5351

## \#1 Posted by: lox897 Posted at: 2017-01-16T10:27:41.908Z Reads: 196

```
You've always wanted to find the best cell for your DIY eBoard Battery right? Well now you can! Simply enter your cells in series and parallel and the spreadsheet will compare almost all cells on the market currently. All the data of the cells is from Battery Bro. If you find something you think is wrong, please don't hesitate to tell me.

Here is a picture of the spreadsheet: (it's not pretty I know)
<img src="/uploads/db1493/original/3X/f/d/fda9d88646fd3fad8d925baebc05bfe918998471.png" width="690" height="347">

And the download link:
http://www.mediafire.com/file/8ak2a7bc0mp94d2/eBoard_Battery_Calculator.xlsx

Google Spreadsheet (not editable, you will need to make a copy):
https://docs.google.com/spreadsheets/d/1vCsmoLAl89ldv8s-otPhf5xYKzKQtj65u36sjIKdYpc/edit?usp=sharing
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-01-16T11:52:53.464Z Reads: 141

```
We should add something like voltage sag for the cells. Because there are good and bad 20A cells.Or like the 30Q which is rated as a 15A cell but performs better at 20A as the most other 20A cells.
```

---
## \#9 Posted by: lox897 Posted at: 2017-01-16T12:08:24.474Z Reads: 133

```
Maybe I will include links to battery tests?

To do list:
1. Add prices from different battery vendors
2. Add battery link tests

Any other suggestions?
```

---
## \#10 Posted by: PXSS Posted at: 2017-01-16T12:47:46.621Z Reads: 125

```
Thats a good start but as Ackmaniac pointed out, just because some cells are rated to high currents doesn't mean they perform well. I use Sanyo GA cells which are only rated to 10A continuous vs Samsung 25R that are rated at 20A continuous but sanyo cells perform just as well up to 20A (Actually slightly better) because they dont sag as much which in turn means higher power output at lower current and better endurance. 

I would link over to henriks tests (lygte-info.dk), but a lot of this goes right over people's head as they don't understand how to use the graphs.
```

---
## \#11 Posted by: lox897 Posted at: 2017-01-16T12:48:59.654Z Reads: 117

```
I will add tests from Mooch and Henrik
```

---
## \#12 Posted by: Maxid Posted at: 2017-01-16T13:21:12.478Z Reads: 112

```
just had a look at the homepage and the graphs and information is amazing.
I kind of regret getting the 25rs now instead of the HE2 or 30Q.
However I don't see the Sanyo GA graph for 20A. Even for 15A he had to abort the test due to heat - which was not the case for the 25rs even at 30A. Am I missing something?
```

---
## \#13 Posted by: PXSS Posted at: 2017-01-16T14:33:40.677Z Reads: 102

```
I have my own data for these cells. Cant share since it's work related. In short. You can run them up to 20A  for a couple of minutes, for eskate this doesn't happen longer than 30secs
```

---
## \#14 Posted by: Ackmaniac Posted at: 2017-01-16T14:46:21.345Z Reads: 109

```
I totally agree. And to show that, i bought a temperature sensor that i will attach to my battery and make some videos so that we can see how the battery temperature goes up. And i think my Battery's are a good example because they are laptop batteries and i stress them way above their limits. But i will also make some videos with high discharge batteries.

Also my app will show in the next version the average amp draw from the battery and to the motors during the ride. So it will be possible that everybody can analyse it's own ride. I think that will be really interesting.

And i would love to see the app connected to a EMTB on the street and offroad.
```

---
## \#15 Posted by: PXSS Posted at: 2017-01-16T15:33:34.157Z Reads: 101

```
Here is a good comparison between 25Rs and GA cells. 
Each curve is the voltage vs Wh discharged for a specific current. As you can see for 25Rs at an average of 10A/cell you get 7.75Wh/cell while for the GA cells you get 10.2Wh/cell. 

<img src="/uploads/db1493/original/3X/d/c/dc643ced218cdcbab478cd04ff127548453651b8.PNG" width="690" height="387">
<img src="/uploads/db1493/original/3X/7/b/7b72574056010fd17e5bfb6b8f2d7dd07b220b52.PNG" width="690" height="387">
```

---
## \#17 Posted by: lox897 Posted at: 2017-01-16T20:27:34.126Z Reads: 82

```
@TarzanHBK 30Q has been added
```

---
## \#18 Posted by: scottkellum Posted at: 2017-01-16T20:36:02.564Z Reads: 83

```
I think I’m gonna build a web app front end to this, awesome data!
```

---
## \#20 Posted by: lox897 Posted at: 2017-01-16T21:41:11.771Z Reads: 79

```
Please use the Excel Sheet if all you want to do is find the best battery. If you want to see prices, the google spreadsheet has prices from li-ion warehouse but the cells are spaced out more to fit the prices, so it's a bit harder to find the cell.
```

---
## \#21 Posted by: lox897 Posted at: 2017-01-16T21:57:48.968Z Reads: 76

```
All prices from li ion warehouse for available cells have been added
```

---
## \#22 Posted by: lox897 Posted at: 2017-01-16T21:58:52.772Z Reads: 73

```
Total price for each cell x your total cells will be added soon
```

---

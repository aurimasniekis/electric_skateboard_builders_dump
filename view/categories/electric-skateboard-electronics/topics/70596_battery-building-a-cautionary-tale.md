# Battery Building - A Cautionary Tale

### Replies: 1 Views: 316

## \#1 Posted by: chsknight Posted at: 2018-10-08T20:24:27.685Z Reads: 102

```
Well... Here we are again..  Another thread on the dangers of building a DIY battery pack.

This was the 2nd pack I made, which itself was a rebuild a the 1st pack I ever made.  The original pack was an 8s3p which was then upgraded to a 10s3p.  The cells used were LG HG2's.  This pack was used in its current state for amount 6 months before I decided to open it up for maintenance.  I was noticing that on some days my board would beast through my test track and some some days it was slouching.

Here is what I uncovered...

Top and Bottom shots of the pack after taking off the primary heatshrinking.  Nothing out of the ordinary so far. 
![20180613_172855|375x500](upload://ylAsd04qKZM1u8x7qoMNW6dtOTV.jpeg) ![20180613_172859|375x500](upload://cjH58hgrFzurIlaoTT63xFXTyA1.jpeg) 

Then I found this issue.  Through the kapton tape you can see burn marks in the top right and bottom left of the connections. 
![20180613_172905|375x500](upload://g7tPNZ9vRBZuIiJZDhMqcYetkgM.jpeg) 

After taking of the tape, it seems this doesnt look too bad.  But it got worst
![20180613_173407|375x500](upload://jQ6c0INDFIT77pdluYpZdzEuVUS.jpeg) 

Looks like my Nickel on Nickel welds were no where near strong enough.  I was able to peal back the strip with no resistance.  Now you can actually see burns marks that occurred.
![20180613_173436|375x500](upload://aO07XvcNRfPKioQhsXb9FzxyFlP.jpeg) 

Kinda hard to tell but you can see some burn marks just underneath the balance cable.
![20180613_173511|375x500](upload://m0zzFs7x8bHemNucZcvopn1CzO1.jpeg) 

Turns out the force applied by the balance cable was the only thing keeping this battery running as this strip also pealed back with no resistance.  Note, you can see burns on the heat shrink due to the strip heating up as most of the current was going through this one strip.

The right most strip is already taken off in this photo but was loose on the top right cell.  This explains the burn marks on the earlier photo.
![20180613_173835|375x500](upload://8cOpOpplcw4JUZO7JlHBjKHGMXK.jpeg) 

And with everything removed we get a good look at fishpaper doing its job. 
![20180613_174126|375x500](upload://75367OWkd1CCQS5r3wTmOZNGbMS.jpeg) 

So what happened?
1) My guess is the loose connections on strips 1 and 3 were causing sparks to form which accounts for the burn marks.
2) The center strip was intact due to friction but carried most of the load which is why the fishpaper burned there the most.

Takeaways:
1)  USE INSULATION CIRCLES!!   Without that extra layer of protection, this could have easily ended with fire.
2)  Test you nickel on nickel welds.  I have made many adjustments since this battery but its always good to do a sanity check.
3)  Check your battery! I now use clear heatshrink for this one reason.  Anytime you open you board, you can do a quick check.  Its kinda like how amusement parks check the rollercoasters everyday.
4)  Insulate or protect you balance cables.  I can see how these lower quality cables can melt and short when getting to close to a connection.

Well thats all for now. Hope this could help some of you out there.  FYI...This battery was cleaned up and put back into service.
```

---

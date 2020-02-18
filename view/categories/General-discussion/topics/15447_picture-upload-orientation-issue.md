# Picture upload orientation issue

### Replies: 5 Views: 662

## \#1 Posted by: AndyPG Posted at: 2016-12-31T14:20:36.970Z Reads: 96

```
Hope everyone had a good Christmas and best wishes for the new year.

I have an issue uploading pictures.
About 50% of the time the orientation of the picture changes once uploaded.
I've done a bit of Googling and I think I understand the hidden tagging that causes it.
Is there an easy fix within the forum to rotate them?

Andy.
```

---
## \#2 Posted by: lox897 Posted at: 2017-01-01T03:56:36.492Z Reads: 72

```
Weird... i've never had an issue with rotation of pictures. When you upload, there is a HTML line starting with <img>. There may be rotation settings in that. What device are you using?
```

---
## \#3 Posted by: IDVert3X Posted at: 2017-01-01T09:10:44.869Z Reads: 60

```
It's a Chrome bug ( or feature? ).

It displays the orientation properly when opened as an image, but once the image is embedded in the website, it ignores the metadata telling in which orientation the picture was taken.

The best solution is to rotate the image so the horizontal line is on the x axis ( width*height ), not leaving it in a wrong orientation ( height*width ) and then using metadata to tell the app how to rotate it ( which may or may not work ).

Cell phones usually use metadata instead, so that might be the issue.
```

---
## \#4 Posted by: leroy Posted at: 2017-01-01T09:26:08.970Z Reads: 49

```
It most likely the meta data in the image, some programs use it for orientation and some don't.
 Open images in The Gimp, it does use the data, and it will prompt you to change if the orientation and data are not in agreement. 
Do y'all know The Gimp?

http://gimp.org

It's free as in beer.
```

---
## \#5 Posted by: AndyPG Posted at: 2017-01-01T11:30:20.424Z Reads: 48

```
Thanks for the advise guys.
I've been taking pictures with a Windows phone and I do indeed use Chrome as my browser.
I have now found that if I open the image in a photo editing program or even Windows Paint and then save, the orientation is then tagged correctly for further use.

Happy New Year guys.
```

---

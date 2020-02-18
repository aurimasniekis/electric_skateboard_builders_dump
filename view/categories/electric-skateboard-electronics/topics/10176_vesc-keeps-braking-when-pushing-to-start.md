# VESC keeps braking when pushing to start

### Replies: 5 Views: 885

## \#1 Posted by: jesser722 Posted at: 2016-09-26T18:32:04.271Z Reads: 109

```
I recently installed my VESC and when I try to push to start it, it does these short quick brakes until I stop pressing the trigger. If I press the throttle before I start then it works just fine. Has anyone else had this problem? Thanks!
```

---
## \#2 Posted by: Mrmoonlight Posted at: 2016-09-26T18:48:59.782Z Reads: 104

```
What's your setup? and what VESC are you using?
```

---
## \#3 Posted by: jesser722 Posted at: 2016-09-26T19:25:39.089Z Reads: 92

```
I have the space cell pro 4 , enertion esc and a turnigy motor
```

---
## \#4 Posted by: mattdig Posted at: 2016-09-26T19:37:29.663Z Reads: 86

```
You probably have the brake parameters setup so zero throttle (or 50% depending on your controller) is brake, when that should be coast (no brake). It should only be braking below 0 or 50%.
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2016-09-27T12:19:56.418Z Reads: 62

```
This should help you...

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244
```

---

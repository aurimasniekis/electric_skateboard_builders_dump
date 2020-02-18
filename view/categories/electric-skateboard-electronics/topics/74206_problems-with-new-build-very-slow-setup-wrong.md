# Problems with new build - very slow - setup wrong?

### Replies: 8 Views: 166

## \#1 Posted by: Fulabi Posted at: 2018-11-10T21:59:43.114Z Reads: 59

```
Hi everyone,

I've just finished my first build but I'm having problems. The board feels very slow and doesn't have much torque. My spec is...

- FocBox
- Single 192kv SK3 6374: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
- 10s3p battery from here (with 30q cells): https://pwrboards.com/collections/battery-parts/products/batteri?variant=4137258745887

I've setup my Mini Remote, otherwise I'm using default focbox settings. I've screen shot my settings from BLDC tool.

Any recommendations?

![1|690x376](upload://1fJny1BzdDRsfNtvMfw6ZK6TpSF.png) ![2|690x378](upload://5mAX18BuQmi22YbbjcPDI5AZen7.png) ![3|690x376](upload://uzJLG7kC9gBWjLY4XagYkUqg9iQ.png)
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-11-10T22:01:18.369Z Reads: 56

```
You can safely up your battery max to 45 and get quite a bit more torque.

And up your motor max and motor min to 80/-80

I'd limit your erpm to 60k instead of 100k

Also make sure your remote is showing 100% when full throttle in bldc tool when you are mapping your pulsewidth... Otherwise you will never get full throttle
```

---
## \#3 Posted by: Andy87 Posted at: 2018-11-10T22:03:35.986Z Reads: 56

```
What @skatardude10 said
Plus motor amps to 60a 
Take out the „limit max erpm with negativ torque“
If you let it ticked your focbox will break when reached max erpm.
```

---
## \#4 Posted by: Andy87 Posted at: 2018-11-10T22:08:25.571Z Reads: 53

```
It’s single drive. I would start with motor max 60a and look how hot the motor get.
With my single drive I had issues with motor max at 80a. Became hot very fast.
```

---
## \#5 Posted by: Grozniy Posted at: 2018-11-10T22:15:54.607Z Reads: 45

```
Also check if your battery is fully charged. Might be obvious but it's simple to forget :sweat_smile:
```

---
## \#6 Posted by: Fulabi Posted at: 2018-11-10T22:16:44.837Z Reads: 47

```
Thanks for your help guys.

Does this look better / safe?


![Better%3F|690x383](upload://kvgnf0CLBR75m8lgm6eF2bimz2n.png)
```

---
## \#7 Posted by: Andy87 Posted at: 2018-11-10T22:27:05.215Z Reads: 41

```
You can limit your erpm to +-60 000
But with 190kV and 10s you anyhow will not reach the limit.
For me your settings look good now.
Take a look at the first rides if your motor or focbox becomes too warm. If no than you can rise up your motor max slowly till 80a.
Battery max i wouldn’t rise up more than 50a.
```

---
## \#8 Posted by: Fulabi Posted at: 2018-11-10T22:31:40.226Z Reads: 40

```
Thanks all, will let you know how I get on.
```

---

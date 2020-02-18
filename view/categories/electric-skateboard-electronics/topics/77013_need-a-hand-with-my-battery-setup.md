# Need a hand with my battery setup

### Replies: 5 Views: 311

## \#1 Posted by: SpeedyGornzallez Posted at: 2018-12-04T11:04:06.250Z Reads: 69

```
I need a hand with my battery setup, I’m making a 10s3p setup and it’s my first battery, the cells I’m using are Samsung INR18650-25R 2500mAh - 20A 

https://eu.nkon.nl/rechargeable/18650-size/samsung-18650-inr18650-25r.html

My idea was 10 cells lined up in series and then the 3 rows connected in parallel like shown in this ![image|375x500](upload://mxW7PUZhLm6OY89JIoYoteOwxTJ.jpeg) ![image|375x500](upload://pamQ5GwSmqaFTyYLPhTnPKAu0Hu.jpeg) 

If anyone can confirm this is a good setup or how to improve it, any help would be appreciated
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-04T11:30:50.299Z Reads: 64

```
it would be better if you make 10 pack with each 3 cells in parallel and those 10 than to wire up in series.
the reason behind
you can easily install a bms to balance charge (and discharge if needed) your pack
serial connections need to be more strong than parallel connections (more layers of nickle or addtional 10-12AWG silicon wire) 
As all current flows over the serial connection but will be shared under the parallel connections. 
Because of it, it would be more easy to change the layout to 3p x10
```

---
## \#3 Posted by: Andy87 Posted at: 2018-12-04T11:33:09.553Z Reads: 63

```
you can also get some inspiration from here
https://www.electric-skateboard.builders/t/please-review-my-battery-pack-so-i-dont-make-a/70102?u=andy87

please just from the positive examples shown in there :sweat_smile:
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-12-04T11:41:30.002Z Reads: 55

```
Doing it that method would result in 3 seperate 10S1P batteries. If you want to be able to use one charger with a balance port, or use a BMS, you'll need each group of 3 cells connected in parallel, then 10 of those groups in series.
```

---
## \#5 Posted by: SpeedyGornzallez Posted at: 2019-02-08T12:03:35.489Z Reads: 17

```
I’ve finally finished my basic assembly of the battery and it’s come to the stage of connecting them in serial and I’m just curious as to how is best to do this, the nickel strip I’m using is rated at 40A and this battery will draw 60A if I’m right in saying so, will I need to double up on nickel strip or will it be alright? ![image|375x500](upload://hDT7tGUNkMkeOuE0HHoSM9Dnxvx.jpeg) 
I’m thinking just do strips to connect them in series and same for the other lot of batteries I have ready (I just used one row of 5 for demonstration purposes)
```

---

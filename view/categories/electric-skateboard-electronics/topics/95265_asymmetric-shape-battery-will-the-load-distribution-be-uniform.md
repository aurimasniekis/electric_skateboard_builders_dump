# Asymmetric shape battery. Will the load distribution be uniform?

### Replies: 4 Views: 212

## \#1 Posted by: Drom Posted at: 2019-05-28T10:15:20.748Z Reads: 92

```
I want to make a 12S6P 30Q asymmetric shape battery. Not like on the picture below, just easier to consider it on the example of 6S4P.

Will these two batteries work equally well? I'm not sure if cells in battery B will be discharged/charged evenly.

![configuration1|594x500](upload://eW0G98qRWCFdGPnqrbQblSZ5f0m.jpeg)
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-05-28T10:29:39.667Z Reads: 88

```
Current sharing between the cells is strongly affected by the resistance of the interlinks - the lower the resistance, the better the cells will share current. So if you've got a highly asymmetrical pack, the interlinks need to be very low resistance to compensate.

You can also get clever and cheat a bit by lowering the resistance of the interlinks farther away from the current path, to compensate.
```

---
## \#3 Posted by: Drom Posted at: 2019-05-28T11:50:13.358Z Reads: 66

```
Resistance should be equal between the parallel connected cells (green interlinks) or between each cells?
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-05-28T12:27:18.149Z Reads: 61

```
Ideally the resistance between the place the current leaves a cell group, and each cell in that group should be equal - E.G. If you have four cells in a row , A, B, and C, and your series connection is coming off of A, and A is connected to B, etc, then the last cell, C, will be supplying the least current because it's two interlinks away from the series connection.

If, however, you draw from B, then both A and C will only be 1 interlink away, and thus will share the current better.

B will still be supplying more than A or C, but it'll be less drastic.


You can do clever things to match the resistance of different configurations, like using more layers of  nickel strip on longer runs than shorter ones, etc.![cell%20layout|556x500](upload://p9HHE0kJapsAQB898vKy4YKpoUg.png)
```

---

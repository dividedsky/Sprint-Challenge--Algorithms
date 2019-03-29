Add your answers to the Algorithms exercises here.

## Exercise I

* a: This one's kind of tricky because it's cubing n, but there are not nested for loops. I _think_ this snippet would still run in O(n^3) time, as we cube n and then run the while loop that many times.

* b: This snippet would run in O(n^3) time. The i loop, j loop, and k loop all depend on the size on input n. I don't think the l loop counts, as that will only run 10 times and is therefore constant.

* c: This snippet would run in O(n) time. It's only going to run the function n times.

## Exercise II
Start at floor 0. While your current floor is less than n _and_ the egg you drop does not break, keep climbing one floor. If the egg breaks, you are on floor f.

```
for i in range(n + 1):
  drop egg
  if egg breaks:
    you're on floor f
```

This would run in O(n) time. In the worst-case scenario, floor f == n, so you have to climb to the top of the building.

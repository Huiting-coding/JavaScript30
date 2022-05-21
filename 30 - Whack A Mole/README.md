 Useful notes:

 1-setTimeout
 2-Math.random()

https://stackoverflow.com/questions/1527803/generating-random-whole-numbers-in-javascript-in-a-specific-range

Math.random() returns a Number between 0 (inclusive) and 1 (exclusive). So we have an interval like this:

[0 .................................... 1)
Now, we'd like a number between min (inclusive) and max (exclusive):

[0 .................................... 1)
[min .................................. max)
We can use the Math.random to get the correspondent in the [min, max) interval. But, first we should factor a little bit the problem by subtracting min from the second interval:

[0 .................................... 1)
[min - min ............................ max - min)
This gives:

[0 .................................... 1)
[0 .................................... max - min)
We may now apply Math.random and then calculate the correspondent. Let's choose a random number:

                Math.random()
                    |
[0 .................................... 1)
[0 .................................... max - min)
                    |
                    x (what we need)
So, in order to find x, we would do:

x = Math.random() * (max - min);
Don't forget to add min back, so that we get a number in the [min, max) interval:

x = Math.random() * (max - min) + min;
That was the first function from MDN. The second one, returns an integer between min and max, both inclusive.

## Logarithms

We've encountered some of the most common complexities: O(1), O(n), O(n^2)

Sometimes big O expressions involve more complex mathematical expressions

One that appears more often than you might like is the logarithm!

## Wait, what's a log again?

log<sub>2</sub>(8)= 3 → 2^3 = 8

log<sub>2</sub>(value) → 2^exponent = value

We'll omit the 2.

log === log<sub>2</sub>

## Wut.

This isn't a math course, so here's a rule of thumb.

The logarithm of a number roughly measures the number of times you can divide that number by 2 before you get a value that's less than or equal to one.

## Examples

![image](https://user-images.githubusercontent.com/88057912/222980514-66091274-f880-41f1-a979-f87264d66045.png)

## Logarithm Complexity

Logarithmic time complexity is great!

![image](https://user-images.githubusercontent.com/88057912/222980550-dccca485-1e1f-417f-aacb-7c889f049278.png)

## Who Cares?

Certain searching algorithms have logarithmic time complexity.

Efficient sorting algorithms involve logarithms.

Recursion sometimes involves logarithmic space complexity.

...and more!

## Recap

- To analyze the performance of an algorithm, we use Big O Notation
- Big O Notation can give us a high level understanding of the time or space complexity of an algorithm
- Big O Notation doesn't care about precision, only about general trends (linear? quadratic? constant?)
- The time or space complexity (as measured by Big O) depends only on the algorithm, not the hardware used to run the algorithm
- Big O Notation is everywhere, so get lots of practice!

## An Example

Suppose we want to write a function that calculates the sum of all numbers from 1 up to (and including) some number n.

```
function addUpTo(n) {
  let total = 0;
  for (let i = 1; i <= n; i++) {
    total += i;
  }
  return total;
}
```

```
function addUpTo(n) {
  return n * (n + 1) / 2;
}
```

Which one is better?

## What does better mean?

- Faster?
- Less memory-intensive?
- More readable?

### Timing:

```
var time1 = performance.now();
addUpTo(1000000000);
var time2 = performance.now();
console.log(`Time Elapsed: ${(time2 - time1) / 1000} seconds.`)
```

#### The Problem with Time

- Different machines will record different times
- The same machine will record different times!
- For fast algorithms, speed measurements may not be precise enough

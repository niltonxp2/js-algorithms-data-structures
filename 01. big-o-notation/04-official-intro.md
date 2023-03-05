## Introducing....Big O

Big O Notation is a way to formalize fuzzy counting

It allows us to talk formally about how the runtime of an algorithm grows as the inputs grow

We won't care about the details, only the trends

## Big O Definition

We say that an algorithm is O(f(n)) if the number of simple operations the computer has to do is eventually less than a constant times f(n), as n increases

f(n) could be linear (f(n) = n)
f(n) could be quadratic (f(n) = n )
f(n) could be constant (f(n) = 1)
f(n) could be something entirely different!

## Example

Always 3 operations O(1)

```js
// constant
function addUpTo(n) {
  return (n * (n + 1)) / 2;
}
```

Number of operations is (eventually) bounded by a multiple of n (say, 10n) O(n)

```js
// linear
function addUpTo(n) {
  let total = 0;
  for (let i = 1; i <= n; i++) {
    total += i;
  }
  return total;
}
```

```js
// linear
function countUpAndDown(n) {
  console.log('Going up!');
  for (let i = 0; i < n; i++) {
    console.log(i);
  }
  console.log('At the top!\nGoing down...');
  for (let j = n - 1; j >= 0; j--) {
    console.log(j);
  }
  console.log('Back down. Bye!');
}
```

O(n) operation inside of an O(n) operation.

$$
O(n * n) = O(n^2)
$$

```js
// quadratic
function printAllPairs(n) {
  for (var i = 0; i < n; i++) {
    for (var j = 0; j < n; j++) {
      console.log(i, j);
    }
  }
}
```

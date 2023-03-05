## Simplifying Big O Expressions

When determining the time complexity of an algorithm, there are some helpful rule of thumbs for big O expressions.

These rules of thumb are consequences of the definition of big O notation.

## Constants Don't Matter

$$
O(2n) = O(n)
$$

$$
O(500) = O(1)
$$

$$
O(13n^2) = O(n^2)
$$

## Smaller Terms Don't Matter

$$
O(n + 10) = O(n)
$$

$$
O(1000n + 50) = O(n)
$$

$$
O(nˆ2 + 5n + 8) = O(n^2)
$$

## Big O Shorthands

- Analyzing complexity with big O can get complicated
- There are several rules of thumb that can help
- These rules won't ALWAYS work, but are a helpful starting point

1. Arithmetic operations are constant
2. Variable assignment is constant
3. Accessing elements in an array (by index) or object (by key) is constant
4. In a loop, the the complexity is the length of the loop times the complexity of whatever happens inside of the loop

## A Couple More Examples

```js
// O(n)
function logAtLeast5(n) {
  for (var i = 1; i <= Math.max(5, n); i++) {
    console.log(i);
  }
}
```

```js
// O(1)
function logAtMost5(n) {
  for (var i = 1; i <= Math.min(5, n); i++) {
    console.log(i);
  }
}
```

# Graph

![image](https://user-images.githubusercontent.com/88057912/222976658-3658189e-294d-4923-aba2-f2224f559753.png)

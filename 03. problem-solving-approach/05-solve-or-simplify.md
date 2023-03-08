## SOLVE THE PROBLEM

If you can't...

SOLVE A SIMPLER PROBLEM!

## SIMPLIFY

- Find the core difficulty in what you're trying to do
- Temporarily ignore that difficulty
- Write a simplified solution
- Then incorporate that difficulty back in

Write a function which takes in a string and returns counts of each character in the string.

```js
function charCount(str) {
  let result = {};

  for (let i = 0; i < str.length; i++) {
    const char = str[i].toLowerCase();

    if (result[char] > 0) {
      result[char]++;
    } else {
      result[char] = 1;
    }
  }

  return result;
}

console.log(charCount('Hello World!'));
```

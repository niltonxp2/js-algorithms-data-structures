## countUniqueValues

Implement a function called countUniqueValues, which accepts a sorted array, and counts the unique values in the array. There can be negative numbers in the array, but it will always be sorted.

```js
countUniqueValues([1, 1, 1, 1, 1, 2]); // 2
countUniqueValues([1, 2, 3, 4, 4, 4, 7, 7, 12, 12, 13]); // 7
countUniqueValues([]); // 0
countUniqueValues([-2, -1, -1, 0, 1]); // 4
```

## My solution

```js
function countUniqueValues(values) {
  let left = 0;
  let right = values.length - 1;
  let count = 0;
  const obj = {};

  while (left < right) {
    if (!obj[values[left]]) {
      obj[values[left]] = true;
      count++;
    }
    if (!obj[values[right]]) {
      obj[values[right]] = true;
      count++;
    }

    ++left;
    --right;
  }

  return count;
}
```

## Solution

```js
function countUniqueValues(arr) {
  if (arr.length === 0) return 0;
  let i = 0;
  for (var j = 1; j < arr.length; j++) {
    if (arr[i] !== arr[j]) {
      i++;
      arr[i] = arr[j];
    }
  }
  return i + 1;
}
```

## ARRAYS (Ordered lists!)

```js
let names = ['Michael', 'Melissa', 'Andrea'];
let values = [true, {}, [], 2, 'awesome'];
```

## WHEN TO USE ARRAYS

- When you need order
- When you need fast access / insertion and removal (sort of....)

## Big O of Arrays

Insertion - It depends.  
Removal - It depends.  
Searching - O(N).  
Access - O(1).

Let's see what we mean by that!

**pop and push are always faster then shift and unshift because if you make an insertion/removal
at the very beginning all the elements will be reindexed**

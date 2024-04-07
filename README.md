# Algorithms

## Insertion Sort

```bash
// Pseudocode
for j=2 to A[n]
  key=A[j]
  i=j-1
  while i>0 and A[i]>key
    A[i+1]=A[i]
    i=i-1
  A[i+1]=key
```

```js
// Javascript implementation
function insertionSort (array) {
    for (let j = 1; j < array.length; j++) {
        let key = array[j];
        let i = j - 1;
        while (i >= 0 && array[i] > key) {
            array[i + 1] = array[i];
            i = i - 1;
        }
        array[i + 1] = key;
    }
    return array;
};
```

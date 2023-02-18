# The Big O of Arrays

## Arrays

- Arrays are ordered lists
- The order can come at a cost re: performance
- Each element in an array has an index (numeric value that corresponds to position of element in array)
- Zeroth item, First item, Etc

- When you need order!
- Elements' positions in Array - v. important

### Performance

- Insertion - It depends
- Removal - It depends
- Searching - O (N)
- Access - O (1)

- Access is very fast!

            let names = ["Giovanni", "Maria", "Lorenzo", "Chiara", "Alessandra"];

- Constant Time to access "Chiara"
- "If I ask for the 9000th Element, I am providing the index, so I'm jumping immediately to the data as it is ordered"

### Insertion Methods and Performance

- Insertion, depends on where in the array
- push() will result in O (1) / constant time /
- unshift() will re-index the ENTIRE array; O (N)

### Removal Methods and Performance

- Removing from beginning of array, also re-indexes entire array; O (N)
- shift(); woof
- pop(); not as bad

## Built-in Methods and Performance

- push() - O (1)
- pop() - O (1)
- shift() - O (N)
- unshift() - O (N)
- concat() - O (N)
- slice() - O (N)
- splice() - O (N)
- sort() - O (N \* log N)

- forEach() - O (N)
- map() - O (N)
- filter() - O (N)
- reduce() - O (N)

### Reminder:

- O (N) - linear time
- O (1) - constant time

- O (N \* log N) - loglinear complexity // common in recursive sorting, binary tree sorting, etc
- Sorting is very slow!

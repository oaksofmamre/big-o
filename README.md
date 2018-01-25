# big-o

Assessing the time-complexity of operations on some data structures in JavaScript

### Instructions

Determine the big O of the following (and ideally explain briefly why):

1. Accessing an item by index in an array

```
An array item is targeted precisely by an index. Thus the time-complexity is constant time, or O(1).
```

2. Unshifting a new item into the beginning of an array

```
To unshift an array is to add items to the beginning of the array. This requires each element to scoot over to make room. The amount of scooting over depends on the number of elements. Thus the time-complexity is linear time, or O(n).
```

3. Pushing an item onto the end of an array

```
Assuming that the array has already been allotted space in memory for it to grow, it is then trivial to push an item onto the memory. Thus the time-complexity is constant time, or O(1). However, consider the scenario where the array space needs to be reallocated in memory, which is more likely, in order to rebuild that array with the new element pushed onto it. Then time-complexity is now linear time, or O(n). In summary, we take the worst-case scenario in big O notation, ending up with O(n) in the final analysis.
```

4. Upcasing a String

```
To upcase a string, each character needs to be traversed to make the switch. Thus the time-complexity is linear time, or O(n).
```

5. Reversing a String

```
Similarly, to reverse a string, each character needs to be traversed. The time-complexity is again linear time, or O(n).
```

6. Finding the max of an array

```
To find the max of an array, each element needs to be traversed to note the next new max value. The time-complexity is linear time, or O(n).
```

7. splitting a String

```
Using the split() function finds the string in its argument, then creates an array for each resulting element. For example, given:

	var str = "How are you doing today?";
	var res = str.split(" ");

We are looking for " " in str. The whole str needs to be traversed. That has a time-complexity of linear time, or O(n). Then for every occurance of " ", there is an operation to insert that into the array. Since constants are omitted, the time-complexity of O(n) remains.
```

8. Inserting a value to an Object

```
Objects in JavaScripts are implementations of associative arrays. Under the hood they are hash-tables. Inserting a value into an object then starts with an input into the hash-function, yielding the relevant index, which has a time-complexity of O(1). Subsequently an insertion into the hash-table, is the linked-list, and without needing to sort, the insertion can be simply at the head or the tail. This operation also has a time-complexity of O(1). Thus in the final analysis we're looking at constant time, or just simply O(1).
```

9. Retrieving the keys of an Object ({ foo: "bar" }.keys)

```
Similarly, the input into a hash-function is the same as working with an array with a time-complexity of O(1). However retrieving the keys of an object requires potentially traversing through the whole linked-list. This has a time-complexity of linear time, or O(n).
```

by Dennis C

:hamburger:

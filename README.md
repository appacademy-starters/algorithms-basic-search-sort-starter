# Intro to Searches and Sorts Project

Clone the project from the [starter] and install packages with `npm install`.

## Learning Goals

* Understand the complexity of a `binary search` and how its performance
    differs from that of a `linear search`.
* Explain the complexity of and write a function that performs `bubble sort` on
    an array of numbers.
* Explain the complexity of and write a function that performs `selection sort`
    on an array of numbers.
* Explain the complexity of and write a function that performs `insertion sort`
    on an array of numbers.

## Part 1: Comparing Linear vs Binary Search

Open up `binary-search.js`. Your first task is to implement a linear search:

```js
linearSearch([2,4,6,8], 6);  // 2
linearSearch([2,4,6,8], 10);  // -1
```

This returns the index of the target if it is contained in the array, and `-1`
otherwise. You should be able to solve it in one line of code.

Run tests by typing `mocha test/search-specs.js`.

Once the linear search is passing, fill out `binarySearch` which should work
the same way: returns the index of the target if it is contained in the array,
and `-1` otherwise.

```js
binarySearch([2,4,6,8], 6);  // 2
binarySearch([2,4,6,8], 10);  // -1
```

The key difference between the linear and binary searches is in the
performance tests. You should be able to search through an array with 1
million items roughly 1000 times per second with a linear search, and 500000
times per second with binary search.

(Specs will pass with 500 linear and 100000 binary searches so don't worry if
your computer is slow.)

Be sure to follow the pseudocode provided.

## Part 2: Implementing Basic Sorting Algorithms

Next, you will be implementing some basic sorting algorithms: _bubble_,
_selection_ and _insertion_ sorts. You will do so both in-place (mutate the
original array) and out-of-place (return a new array without changing the
original).

For each of these problems, take time to understand the provided pseudocode,
then translate the pseudocode to JavaScript.

Run tests by typing `mocha test/sort-specs.js`.

Since each sort returns the same output regardless of the internal algorithm,
this exercise makes use of `console.log` to make sure that your
implementations of each algorithm is correct. Note each intermediate state of
the arrays in `test/sort-specs.js`.

If you follow the pseudocode, your `console.log` outputs will match the order
in the specs.

[starter]: https://github.com/appacademy-starters/algorithms-basic-search-sort-starter

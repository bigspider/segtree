# segtree
A simple implementation of a fixed-length segment tree for range sums. See for example http://www.geeksforgeeks.org/segment-tree-set-1-sum-of-given-range/.

NOTE: the name "segment tree" is used in literature for different structures used in computational geometry. Here we refer to a data structure that provides random access to an array, augmented with efficient range queries.

The SumSegmentTree class stores an array A of size n, providing access with three methods:

- get(i): returns the element at index i
- set(i, x): set the element at index i to x
- sum(i, j): return the sum of all the elements between indexes i and j (inclusive)

The complexity of get is O(1); the complexity of set and sum is O(log n)

With easy modifications, the structure can be easily adapted to other kinds of range queries for example: minimum, maximum, product, and so on. More generally, range queries for any associative binary operator can be implemented in O(log n).

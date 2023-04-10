### Deterministic Quicksort
1. Pick first element in list as a pivot.
2. left are less than pivot
3. right are greater or equal to pivot.
4. Recursively call the algorithm until everything is sorted
Worst case is when all elements are always in one part of the sublist (a.k.a sorted list)
runtime is $O(n^{2})$
(Imagine we take the median and sublists are always equal)
Best case is $O(n\lg(n))$
### Randomized Quicksort
Same as quicksort but pivot at each step is random.

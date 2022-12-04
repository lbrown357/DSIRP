QUESTIONS:

1. What is the order of growth of  n^3+n^2 ? What about 1000000n^3 + n^2? What about n^3 + 1000000n^2?

2. What is the order of growth of (n^2+n)⋅(n+1)? Before you start multiplying, remember that you only need the leading term.

3. If f is in O(g), for some unspecified function g, what can we say about af + b, where a and b are constants?

4. If f1 and f2 are in O(g), what can we say about f1 + f2?

5. If f1 is in O(g) and f2 is in O(h), what can we say about f1 + f2?

6. If f1 is in O(g) and f2 is in O(h), what can we say about f1 ⋅ f2?

7. What is a "comparison sort?" What is the best worst-case order of growth for a comparison sort? What is the best worst-case order of growth for any sort algorithm?

8. What is the order of growth of bubble sort, and why does Barack Obama think it is "the wrong way to go?"

9. What is the order of growth of radix sort? What preconditions do we need to use it?

10. What is a stable sort and why might it matter in practice?

11. What is the worst sorting algorithm (that has a name)?

12. What sort algorithm does the C library use? What sort algorithm does Python use? Are these algorithms stable? You might have to Google around to find these answers.

13. Many of the non-comparison sorts are linear, so why does Python use an  O(nlog(n))  comparison sort?

ANSWERS:

1. All of these have the same order of growth: O(n^3)

2. O(n^3)

3. af + b is in O(g)

4. f1 + f2 is in O(g)

5. f1 + f2 is in either O(g) or O(h) (depending on which one is "worse")

6. f1 ⋅ f2 is in O(gh)

7. Sorts data with no more than 2 elements using a comparison operator. The best and worst casenario for a comparison sort is n and n^2 respectively. Same is true for all sorts, except the worse casenario possible is n^2 * k.

8. Bubble sort involves taking every adjacent pair of data and swapping them if the first piece of data is larger than the second. Best case scenario, this will never happen and only n - 1 steps are required. Worse case scenario, this has to be done for every single pair, requiring n^2 - 2n - 1 steps. Not ideal for enormous amounts of data.

9. LSD radix sort has an order of growth of O(n * k), but requires the data to be stable. MSD radix sort does not require that, but the sorting will be unstable.

10. A stable sort will not sort two numbers if they are of the same size. in practice, this may save time when the sort is frequently running into the same number right next to each other.

11. bogosort just randomly sorts stuff and hopes for the best. This makes it the worst sorting algorithm.

12. Python uses Timsort, which is stable. C uses a variant of quicksort, which isn't stable.

13. Timsort, the sort used by python, is stable. Despite having a somewhat high order of growth compared to other sorts, other sorts often are unstable.

Order of growth names:
- Constant
- Logarithmic
- Linear
- Linearithmic
- Quadratic
- Cubic
- Exponential
# CMPS 2200 Reciation 5
## Answers

**Name:**___Emma Jones_____


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
performance is influenced by how the elements are distributed within the list. If the
list is already sorted, Quicksort with a fixed pivot might demonstrate better
performance because it capitalizes on the pre-sorted nature of lists, which aligns
with its selection strategy. However, Quicksort with a random pivot may encounter
worst-case scenarios where the randomly selected pivot partitions the array unevenly.
In the case of a reverse-sorted list, Quicksort with a fixed pivot may perform
reasonably well, but selecting the pivot as the first or last element may not yield
optimal results. Conversely, Quicksort with a random pivot might exhibit superior
performance in reverse-sorted lists since it's less likely to choose a pivot from the
extremes.


Sorted List:
|      n |qsort-fixed-pivot(ms)|qsort-random-pivot(ms)|timsort(ms)|
|--------|---------------------|----------------------|-----------|
|    100 |               0.077 |                0.214 |     0.054 |
|    200 |               0.086 |                0.342 |     0.091 |
|    500 |               0.104 |                1.198 |     0.087 |
|   1000 |               0.194 |               42.881 |     0.097 |
|   2000 |               0.252 |                4.705 |     0.108 |
|   5000 |               0.583 |               22.558 |     0.105 |
|  10000 |               1.005 |               78.310 |     0.158 |
|  20000 |               2.189 |              114.577 |     0.313 |
|  50000 |               5.999 |              374.949 |     0.884 |
| 100000 |              11.793 |              985.816 |     1.465 |

Random List:
|      n |qsort-fixed-pivot(ms)|qsort-random-pivot(ms)|timsort(ms)|
|--------|---------------------|----------------------|-----------|
|    100 |               0.261 |                0.256 |     0.075 |
|    200 |               0.671 |                0.474 |     0.123 |
|    500 |               1.092 |                1.415 |     0.111 |
|   1000 |               2.037 |                2.221 |     0.182 |
|   2000 |               4.689 |                4.597 |     0.336 |
|   5000 |              11.021 |               70.320 |     0.878 |
|  10000 |              24.016 |               94.420 |     1.947 |
|  20000 |             130.491 |              190.174 |     4.398 |
|  50000 |             406.376 |              473.544 |    11.824 |
| 100000 |            1005.399 |              992.076 |    82.722 |

- **1c.**
as input size grows, timsort is most efficient followed by fixed-pivot
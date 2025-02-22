# Bubble Sort
## pseudo code
```pseudo
Step 1: Initialize an array A and its length n.
Step 2: Iterate over the array with an outer loop from i = 0 to n-1:
          a. Iterate with an inner loop from j = 0 to n-1-i:
             i. If A[j] > A[j + 1], swap A[j] and A[j + 1].
Step 3: Print the sorted array.
Step 4: Terminate the algorithm.
```
```
BubbleSort(A)
1.  n ← length(A)
2.  for i ← 0 to n - 2 do
3.      for j ← 0 to n - i - 2 do
4.          if A[j] > A[j + 1] then
5.              swap(A[j], A[j + 1])
```

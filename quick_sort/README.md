# Quick Sort
## pseudo code
```
QuickSort(A, low, high)
1.  if low < high then
2.      pivotIndex ← Partition(A, low, high)
3.      QuickSort(A, low, pivotIndex - 1)
4.      QuickSort(A, pivotIndex + 1, high)

Partition(A, low, high)
1.  pivot ← A[high]
2.  i ← low - 1
3.  for j ← low to high - 1 do
4.      if A[j] ≤ pivot then
5.          i ← i + 1
6.          swap(A[i], A[j])
7.  swap(A[i + 1], A[high])
8.  return i + 1
```

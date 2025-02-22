# Insertion Sort
## pseudo code
```
InsertionSort(A)
Step 1.  for i ← 1 to length(A) - 1 do
Step 2.      key ← A[i]
Step 3.      j ← i - 1
Step 4.      while j ≥ 0 and A[j] > key do
Step 5.          A[j + 1] ← A[j]
Step 6.          j ← j - 1
Step 7.      A[j + 1] ← key
```

## Code
```cpp
#include <iostream>
using namespace std;

void printArray(int array[], int size) {
  for (int i = 0; i < size; i++) {
    cout << array[i] << " ";
  }
  cout << endl;
}

void insertionSort(int array[], int size) {
  for (int step = 1; step < size; step++) {
    int key = array[step];
    int j = step - 1;
    while (j >=0 && key < array[j]) {
      array[j + 1] = array[j];
      --j;
    }
    array[j + 1] = key;
  }
}

int main() {
  int data[] = {9, 5, 1, 4, 3};
  int size = sizeof(data) / sizeof(data[0]);
  insertionSort(data, size);
  cout << "Sorted array in ascending order:\n";
  printArray(data, size);
}

```

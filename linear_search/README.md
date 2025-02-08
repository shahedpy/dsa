# Linear Search

## Code
```cpp
#include <iostream>

using namespace std;

int linear_search(int array[], int size, int x) {
    for (int i = 0; i < size; i++) {
        if (array[i] == x) {
            return i;
        }
    }
    return -1;
}

int main() {
    int array[] = {1, 2, 3, 4, 5, 6, 7, 8, 9};
    int size = sizeof(array) / sizeof(array[0]);
    int target = 5;

    int index = linear_search(array, size, target);

    if (index != -1) {
        cout << "Target found at index: " << index << endl;
    } else {
        cout << "Target not found in the array." << endl;
    }

    return 0;
}
```

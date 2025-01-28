# Binary Search

## Code
```cpp
#include <iostream>
#include <algorithm> // For sort()
using namespace std;

int main() {
    int array_size;
    cout << "Enter the size of the array: ";
    cin >> array_size;

    int data[array_size];

    cout << "Enter " << array_size << " elements (in sorted order or will be sorted):" << endl;
    for (int i = 0; i < array_size; i++) {
        cin >> data[i];
    }

    // Sort the array to ensure it is in ascending order
    sort(data, data + array_size);

    int target;
    cout << "Enter the target element to search: ";
    cin >> target;

    int left = 0, right = array_size - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;

        if (data[mid] == target) {
            cout << "Target found at position " << mid + 1 << " (1-based index)" << endl;
            return 0;
        }

        if (data[mid] < target) {
            left = mid + 1; // Search in the right half
        } else {
            right = mid - 1; // Search in the left half
        }
    }

    cout << "Target not found in the array." << endl;
    return 0;
}

```

# Linear Search

## Code
```cpp
#include <iostream>
using namespace std;

int main() {
    int array_size;
    cout << "Enter the size of the array: ";
    cin >> array_size;

    int data[array_size];

    cout << "Enter " << array_size << " elements:" << endl;
    for (int i = 0; i < array_size; i++) {
        cin >> data[i];
    }

    int target;
    cout << "Enter the target element to search: ";
    cin >> target;

    for (int i = 0; i < array_size; i++) {
        if (data[i] == target) {
            cout << "Target found at position " << i + 1 << endl;
            return 0;
        }
    }

    cout << "Target not found in the array." << endl;
    return 0;
}

```

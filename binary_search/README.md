# Binary Search

## Code
```cpp
#include <iostream>

using namespace std;

int binary_search(int array[], int x, int low, int high){
    if(high >= low){
        int mid = low + (high-low)/2;

        if (x == array[mid])
            return mid;

        if (x > array[mid])
            return binary_search(array, x, mid+1, high);

        return binary_search(array, x, low, mid-1);
    }
}

int main(){
    int array[] = {1,2,3,4,5,6,7,8,9};

    int target = 5;

    cout << "Target found at index: " << binary_search(array, target, 0, 8);
    return 0;
}
```

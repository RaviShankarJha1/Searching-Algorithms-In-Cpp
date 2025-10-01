# Aim  
To study and implement Searching Algorithms in C++  

# Software Required  
Visual Studio  

# Theory  
Searching algorithms are essential in computer science to locate specific items in a collection of data. The two common algorithms based on array type are:  

- **Linear Search** – Used for unsorted arrays. Compares each element sequentially. Time Complexity: **O(n)**.  
- **Binary Search** – Used for sorted arrays. Compares middle element and narrows search interval by half. Time Complexity: **O(log n)**.  

**Linear Search – O(n) Time, O(1) Space**  
Checks each element sequentially until the target is found or the array ends.  

**Binary Search – O(log n) Time, O(1) Space**  
Divides the search interval repeatedly to locate the target efficiently.  

# Implementation  
The following programs demonstrate the two searching algorithms:  
- Linear Search  
- Binary Search  

# Algorithms  

### Binary Search using Class  

1. Start  
2. Define a class `SearchArr` with:  
   - Private function `binarysearch(arr, target)` performing binary search.  
   - Public function `search(arr, target)` that calls `binarysearch`.  
3. Binary Search (`binarysearch`):  
   - Initialize `low = 0` and `high = arr.size() - 1`.  
   - While `low <= high`:  
     - Compute `mid = low + (high - low) / 2`.  
     - If `arr[mid] == target`, return `mid`.  
     - Else if `arr[mid] < target`, set `low = mid + 1`.  
     - Else, set `high = mid - 1`.  
   - If element not found, return `-1`.  
4. In `main()`  
   - Create object `obj` of class `SearchArr`.  
   - Initialize array/vector `arr = {-1, 0, 3, 5, 9, 12}`.  
   - Set `target = 9`.  
   - Call `obj.search(arr, target)`.  
   - Print result (index if found, otherwise `-1`).  
5. End  

### Linear Search  

1. Start  
2. Declare integer array `arr[5]`.  
3. Prompt user: *"Enter Array elements"* and read 5 integers into `arr`.  
4. Display the entered array.  
5. Prompt user: *"Enter the element to be searched"* and read into variable `key`.  
6. For each index `i` from `0` to `4`:  
   - If `arr[i] == key`, print *"Element found at index i"* and exit.  
7. If loop ends without finding, print *"Element not found"*.  
8. End  

# Conclusion  
Through the above programs, both **Linear Search** and **Binary Search** techniques were explored and implemented in C++.

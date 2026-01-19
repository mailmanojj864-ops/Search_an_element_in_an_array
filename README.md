# Search_an_element_in_an_array
A beginner-friendly program that demonstrates how to search for an element in an array using basic c programming concepts
# Search an Element in an Array (C Program)

## 📌 Description
This project is a simple C program that checks whether a given element exists in an array or not.

The program:
- Takes the size of the array and the element to be searched as input
- Stores array elements
- Searches for the given element using a `for` loop
- Prints **YES** if the element is found
- Prints **NO** if the element is not found

This is a beginner-level program and helps in understanding **arrays, loops, and conditional statements** in C.

---

## 🛠️ Concepts Used
- Arrays
- `for` loop
- Conditional statements (`if-else`)
- Flags (using a variable to track result)
- Standard input/output (`stdio.h`)

---

## 🧾 Program Code
```c
#include <stdio.h>

int main() {
    int N, X;
    scanf("%d %d", &N, &X);
    
    int arr[N];
    
    for(int i = 0; i < N; i++) {
        scanf("%d", &arr[i]);
    }
    
    int found = 0;
    
    for(int i = 0; i < N; i++) {
        if(arr[i] == X) {
            found = 1;
            break;
        }
    }
    
    if(found)
        printf("YES");
    else
        printf("NO");
        
    return 0;
}

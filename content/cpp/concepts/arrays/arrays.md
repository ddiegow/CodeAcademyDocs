---
Title: 'Arrays'
Description: 'Like a vector, an array is a data structure used in C++ to store a sequential collection of elements. Unlike vectors, its size cannot be changed. Being able to store multiple pieces of related information in the same structure is very useful when writing C++ programs. When creating an array, have to be kept in mind: The type of data to be store inside it and hoow many items it should be able to hold (its size). An array can be created a lot like how normal variables are created: by specifying the data type, giving it a descriptive name, and also specifying its size'
Subjects:
  - 'Computer Science'
  - 'Game Development'
Tags:
  - 'Arrays'
  - 'Vectors'
CatalogContent:
  - 'learn-c-plus-plus'
  - 'paths/computer-science'
---

Like a vector, an **array** is a data structure used in C++ to store a sequential collection of elements. Unlike vectors, its size cannot be changed.

Being able to store multiple pieces of related information in the same structure is very useful when writing C++ programs.

## Creating an Array

When creating an array, two pieces of information have to be kept in mind:

- The type of data to be store inside it.
- How many items it should be able to hold (its size).

An array can be created a lot like how normal variables are created: by specifying the data type, giving it a descriptive name, and also specifying its size:

```cpp
int favoriteNums[4];
```

In the above code example, an array is created with a size of `4`, meaning it can hold four integers (all four elements will initially have the default `int` value of `0`).

In many cases, what data needs to go in the array will not be known until after it's created , but if the contents of the array are known ahead of time, it can be initialized with custom values upfront:

```cpp
int favoriteNums[] = {7, 9, 15, 16};
```

This array would also have a size of 4, but it does not need to be explicitly specifed when initialized this way.

## Array Indices

Like vectors, each element in an array is assigned a specific index starting at zero. To access or modify an element in the array it may be refered to by its index and operated on accordingly.

```cpp
char vowels[] = {'a', 'e', 'i', 'o', 'u'};
//      indexes:  0    1    2    3    4

std::cout << vowels[0];
// Output: a

vowels[0] = 'r';

std::cout << vowels[0];
// Output: r
```

In the case above, an array of `chars` was initialized with all the vowels, and then the first element in the array at index 0 was printed out. Then the element at index `0` was modified by being assigned a new value of `'r'`, which got printed out below.

Arrays in C++ have a set size, meaning elements can not be added or removed once the array has been created. Only existing elements may be modified without changing the total size or shape of the structure.

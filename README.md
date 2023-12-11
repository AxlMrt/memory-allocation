# Dynamic Memory Manager

This code represents a simplified dynamic memory manager, providing basic functions for memory allocation and deallocation. The aim of this project is to enhance understanding of programming languages and memory management mechanisms.

## Usage Instructions

### Including Necessary Files

```cpp
#include <cstdint>
#include <iostream>
#include <pthread.h>
```

### Code functions

`void *malloc(size_t size)`
Allocates a block of memory of the specifies size and returns a pointer to that allocated area.

`void free(void *block)`
Frees a previously allocated block of memory

`void *calloc(size_t num, size_t nsize)`
Allocates memory for an array of size `num` with each element of size `nsize` and initializes the allocated memory to zero.

### Additional functions

`void *sbrk(intptr_t incr)`
Adjusts the end of memory pointer.

`header_t *get_free_block(size_t size)`
Searches for a sufficiently large free block of memory to fulfill the request.

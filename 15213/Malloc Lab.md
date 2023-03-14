Functions we will implement
```c
bool mm_init(void); 
void *malloc(size_t size); 
void free(void *ptr); 
void *realloc(void *ptr, size_t size); 
void *calloc(size_t nmemb, size_t size); 
bool mm_checkheap(int);
```
```mm.c```: A fully-functional implicit-list allocator. We recommend that you use this code as your starting point. Note that the provided code does not implement [[block coalescing]]. The absence of this feature will cause  [[external fragmentation]] to be very high, so you should implement [[coalescing]]. We strongly recommend considering all cases you need to implement before writing code for coalesce_block; the lecture slides should help you identify and reason about these cases. Make sure to be on the lookout for [[internal fragmentation]] as well.
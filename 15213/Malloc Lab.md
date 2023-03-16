Functions we will implement
```c
bool mm_init(void); 
void *malloc(size_t size); 
void free(void *ptr); 
void *realloc(void *ptr, size_t size); 
void *calloc(size_t nmemb, size_t size); 
bool mm_checkheap(int);
```
`payload[0]` This means that size of payload is controlled by the programer/application.

```mm.c```: A fully-functional implicit-list allocator. We recommend that you use this code as your starting point. Note that the provided code does not implement [[block coalescing]]. The absence of this feature will cause  [[external fragmentation]] to be very high, so you should implement [[coalescing]]. We strongly recommend considering all cases you need to implement before writing code for coalesce_block; the lecture slides should help you identify and reason about these cases. Make sure to be on the lookout for [[internal fragmentation]] as well.

Performance Goals
1. #Throughput - Handle lots of requests per second
2. #Utilization - Using available memory wisely
	Tend to clash against each other. Either Just allocate next block (no utilization) or try to look back at freed memory (slows down speed).
1. Minimize #Ovehead - Fraction of heap space NOT used for program data
	1. Ideal : $O_K = (H_k/max_{i\leq k}P_i) - 1.0$
### Aggreate payload $P_k$
- 
- malloc(p) results in a block with a #payload of p bytes
- Aggregate payload $P_k$ is the sum of currently allocated payloads
- Peak agregate payload $max_{i\leq k}P_i$ is the maximum aggregate payload at any point in the sequence up to request.
Assume heap only grows when allocator uses sbrk and never shrinks.

Poor memory utilization comes from bad fragmentation
1. [[internal fragmentation]]
2. [[external fragmentation]]
### Implementation Issues
- How do we know how much memory to free given just a pointer?
	- [[How much to Free?]]
- How do we keep track of the free blocks?
	- [[Keep track of Free Block]]
- What do we do with extra space when allocating a structure that is smaller than the free block it is placed in?
- How do we pick a block to use for allocation -- many might fit?
- How do we reuse a block that has been freed?


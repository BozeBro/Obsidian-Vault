We have a prologue since we have a header of a word, and then the payload is 2 word aligned, following rule #Rule-Payload-2word-aligned . We have an epilogue to know where the heap is supposed to end without having a number storing the length (wasteful!)

```c
bool mm_init(void) {

// Create the initial empty heap

word_t *start = (word_t *)(mem_sbrk(2 * wsize));

  

if (start == (void *)-1) {

return false;

}

  

/*

* TODO: delete or replace this comment once you've thought about it.

* Think about why we need a heap prologue and epilogue. Why do

* they correspond to a block footer and header respectively?

*/

  

start[0] = pack(0, true); // Heap prologue (block footer)

start[1] = pack(0, true); // Heap epilogue (block header)

  

// Heap starts with first "block header", currently the epilogue

heap_start = (block_t *)&(start[1]);

  

// Extend the empty heap with a free block of chunksize bytes

if (extend_heap(chunksize) == NULL) {

return false;

}

  

return true;

}
```
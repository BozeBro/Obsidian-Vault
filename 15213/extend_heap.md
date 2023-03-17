```c
static block_t *extend_heap(size_t size) {

void *bp;

  

// Allocate an even number of words to maintain alignment

size = round_up(size, dsize);

if ((bp = mem_sbrk((intptr_t)size)) == (void *)-1) {

return NULL;

}
/*

* TODO: delete or replace this comment once you've thought about it.

* Think about what bp represents. Why do we write the new block

* starting one word BEFORE bp, but with the same size that we

* originally requested?

*/

// Initialize free block header/footer

block_t *block = payload_to_header(bp);

write_block(block, size, false);

// Create new epilogue header

block_t *block_next = find_next(block);

write_epilogue(block_next);

// Coalesce in case the previous block was free

block = coalesce_block(block);

return block;

}
```
We ensure we can allocate how much we are asked to extend the heap by.

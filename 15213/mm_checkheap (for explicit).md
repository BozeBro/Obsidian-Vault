1. Check the heap is allocated
2. Check that each allocated block (head is set to 1) is not in the explicit list
3. Check each free block is in the explicit list.
4. Headers are word aligned
5. Memory allocated only comes from free blocks
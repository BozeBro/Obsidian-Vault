![[Screen Shot 2023-03-15 at 8.21.22 PM.png]]

Remember that a #payload is 16 byte aligned, and a block is 16 byte aligned.
We use 1 word to say if a block is allocated or free. and in that block, we say how much 2
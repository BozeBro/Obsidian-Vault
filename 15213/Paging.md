A.k.a Swapping.
Inefficient since we use part of the disk as RAM. RAM is much faster than disk, but disk is bigger. 

Works due to locality since we ensure that we miss very rarely. 

if working set of virtual pages < main memory size -> good performance.
Else we might have thrashing, where the program is so slow that its like we freeze. 
#Swap-Space Substtitute for RAM space when running short on memory. 
Stores memory on disk (Paging) instead of directly in memory.  
We do [[copy-on-write-comparison.excalidraw]] sharing when starting a new [[Process]], 

Technique for quickly duplicating stuff from parent [[Process]] to child [[Process]]
In new process, 
1. Duplicate page tables [[Page Table]]
2. Mark each page as read only
3. Copy only on write faults.
	1. when writing to memory, then we copy (the speedup is here)
See [[Comparison.excalidraw]]

#interprocedural-analysis
1. No context sensitivity
	one context per function. Track only the function being called
2. Limited contexts
	create contexts for functions, but after a certain number have been made, all future calls are merged into a single context. Precision is lost but allows for good performance.
3. Call strings
Track the call site, its call site, etc. 
Full context sensitivity. Not guaranteed to terminate. Very similar to standard context analysis where we make a summary and use dataflow information.

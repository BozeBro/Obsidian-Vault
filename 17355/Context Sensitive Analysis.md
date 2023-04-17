When analayzing function calls, have analysis results reflect different analysis results that are passed in.

Inlining can work since it keeps the context but only for non recursive functions

**Solution #1**, build a summary for each possible input

Problems when there is recursion since inputs will change, since we can have no termination if we Top propogates or not be able to create a summary that terminates. If we treat recursion as a loop, than we can do analysis accurately.


![[Screen Shot 2023-03-15 at 1.00.35 PM.png]]![[Screen Shot 2023-03-15 at 1.00.28 PM.png]]![[Screen Shot 2023-03-15 at 1.00.16 PM.png]]

For function calls, if multiple return statements, results are joined together.
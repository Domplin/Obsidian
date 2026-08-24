
Dynamic programming is a method used to solve complex problems by breaking them into smaller overlapping subproblems and storing their results to avoid recomputation. It is an optimization technique that transforms recursive solutions with exponential time into efficient ones with polynomial time. 


- The core idea behind DP is to store solutions to subproblems so that each is solved only once 
- To Solve DP problems we first write a recursive solution in a way that there are overlapping subproblems in the recursion tree
- To make sure that a recursive value is computed only once, we store the results of the recursive calls
- There are two ways to store the results, one is top down (memoization) or bottom up (tabulation).



**When to Use Dynamic Programming**
1) Optimal Structure:
	1) The property optimal substructure means we use the optimal results of subproblems to achieve the optimal result of the bigger problem
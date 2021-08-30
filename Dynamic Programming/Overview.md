# Dynamic Programming

### Description
Dynamic programming essentially means breaking down an optimization problem into simpler sub-problems, and storing the solution to each sub-problem so that each sub-problem is only solved once. 

Generally a DP problem will have the two following qualities:
- Optimal Substructure: An optimal solution can be constructed from optimal solutions of its subproblems. So the optimal solution of a problem of size `n` is based on an optimal solution to the same problem when considering `n' < n` elements
- Overlapping Subproblems: A problem is said to have Overlapping Subproblems if the problem can be broken down into subproblems which are reused **several** times or a recursive algorithm for the problem solves the same subproblem over and over rather than generating **new** subproblems. 

From these qualities it is clear that storing the solutions for these subproblems would decrease algorithmic complexity, as they do not have to be recalculated multiple times. 

### Implementation
There are two basic approaches that one can use.
- Tabulation (Bottom Up) : Start from the bottom and accumulate answers to the top. If dp[n] is the goal state, you want to start with dp[0] and work your way there. Generally this works because you have a base case that is easy to calculate, and consequent problems can be calculated from that one(s).

> // Tabulated version to find factorial x.
int dp[MAXN];
>
// base case
int dp[0] = 1;
for (int i = 1; i< =n; i++)
{
    dp[i] = dp[i-1] * i;
}

- Memoization (Top Down): Start from the destination state dp[n] and work way down to base case. As subproblems are calculated they get "memoized" or saved for easy reference. 

>// Memoized version to find factorial x.
// To speed up we store the values
// of calculated states
>
// initialized to -1
int dp[MAXN]
>
// return fact x!
int solve(int x)
{
 >   if (x\==0)
   >     return 1;
  >  if (dp[x]!=-1)
  >      return dp[x];
  >  return (dp[x] = x * solve(x-1));
>}


### Fibonacci Sequence
The Fibonacci Sequence is an excellent candidate for Dynamic Programming, as a recursive implementation will call values multiple times. Implementing DP reduces the time complexity from exponential `O(2^n)` to linear `O(n)`
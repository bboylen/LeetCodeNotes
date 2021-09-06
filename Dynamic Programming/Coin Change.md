# Coin Change

Coin change is a classic DP problem. 

### Problem Statement
You are given an integer array `coins` representing coins of different denominations and an integer `amount` representing a total amount of money.

Return the fewest number of coins that you need to make up that amount. If that amount of money cannot be made up by any combination of the coins, return `-1`.

You may assume that you have an infinite number of each kind of coin.

### Approach
If you know the optimal solution for lower amounts of money, you know the optimal solution for the given `amount`. 

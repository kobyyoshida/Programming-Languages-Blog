Example Problem I Found Online

Divisible Sum Pairs

Video:
https://www.youtube.com/watch?v=NcUNN_tSmyE&t=208s

In the video linked above, we look at a practice problem in Haskell. This problem asks to return Divisible Sum Pairs given an array of integers and a positive integer. 

Question:
https://www.hackerrank.com/challenges/divisible-sum-pairs/problem

You are given an array of n integers, ar = [ar[0], ar[1], ... ar[n-1]] , and a positive integer, k. 
Find and print the number of (i,j) pairs where i < j  and ar[i] + ar[j] is divisible by k.

I challenge you to find a solution without the video or solution guide below. 


Solution (From the video):

solve :: [Int] -> Int
solve(k:xs) = length [undefined | (i, xi) <- zip [0..] xs, 
                (j,xj) <- zip [0..] xs,
                i < j
                (xi + xj) 'mod' k==0]
Analysis:

We start with list comprehension. The line [(i, j) | i <- [1 .. 10], j <- [1 .. 10]] creates an array of (i,j) pairs, matching every i to every j to create a cartesian product.
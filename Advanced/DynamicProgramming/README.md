# Dynamic Programming Problems:

## Problem 1: Solve Fibonnaci Problem using Memoization.

Fibonnaci Formula: f(n) = f(n-1) + f(n-2) if n>2 && f(1) = 1, f(2)=1
This problem is self descriptive.
You should be able to explain the memoization in comments.

_Command/Script to Run Problem 1: _Fibonnaci problem using memoization is top down approach of recursion 
fibb(n):
if (n<2)     __check if top down approach
   return n   
   else
   return fibb(n-1) + fibb(n-2) ___store and return
   _______________ (Fill this in when submitting)_

## Problem 2: Find Longest Common SubSequence in two strings.

    Given two strings find the longest common subsequence exisiting between
    those strings.

    Example:

        LCS for input Sequences “ABCDGH” and “AEDFHR” is “ADH” of length 3.

        LCS for input Sequences “AGGTAB” and “GXTXAYB” is “GTAB” of length 4.

    Command/Script to Run Problem 2: ________________ (Fill this in when submitting)
X: ABCDGH
Y: AEDFHR
The length of the LCS is 3
#include <iostream>
#include <string>
using namespacestd;
  int LCSLength (string X , string Y, int n, int m)
    {
      if(m==0 || n==0)
    { return 0;
    }
    if( X[m-1] == y[n-1])
    {
    return  LCSLength(X,Y,m-1,n-1) +1;}
    return max(LCSLength(X,Y,n-1,m), LCSLength(X,Y,m-1,n));
    }
    int main()
    {
     string X = "ABCDGH" , Y = "AEDFHR";
     cout << " The length of the LCS is " <<
     LCSLength(X, Y, X.length(), Y.length());
       return 0;
    }
    
    

# Greedy Algorithms:

## Problem 1: Find Minimum Absolute Difference of Adjacent Elements In An Array.

    Given an array of elements find the minimum absolute difference
    between adjacent elements in an array.

    Example:
        Input : arr[] = {10, 12, 13, 15, 10}

        Output : 0
        Explanation: |10 - 10| = 0 which is the
        minimum possible.

        Function Description

        Complete the function findAbsMin with following details:

        findAbsMin has the following parameter(s):
        int a[n]: the array of elements

        Returns
        int a': Minimum Absolute Difference


    Command/Script to Run Problem 1:
    #include <iostream.h>
    usingnamespace std;
    void minAdjDifference (int arr[] , int n){
    if(n<2)
    return;
    int new = abs(arr[1]- arr[0])
    for (int i=2; i<n; i++)
    new=min(new, abs(arr[i] - arr[i-1]));
    cout<<" Min Difference="<<new;
    }
    int main()
    {
      int a[] = {10,12,13,15,10};
      int n=min(a)/min(a[0]);
      minADJDifference(a,n);
      return0;
      }
      


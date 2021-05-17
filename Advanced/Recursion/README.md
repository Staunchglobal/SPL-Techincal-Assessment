# Recursion Problems:

## Problem 1: Calculate Mean of An Array using Recursion.

    Given an array of elements find the mean of the elements
    in that array using recursion.

    Example:
        Input : arr[] = {10, 12, 14, 16, 18}
        Output : 14
        Function Description

        Complete the function calMean with following details:

        calMean has the following parameter(s):
        int a[n]: the array of elements

        Returns
        int a': Mean of the elements


    Command/Script to Run Problem 1: ________________ (Fill this in when submitting)
#include<iostream.h>
#include<stdio.h>
using namespace std;
float findMean(inta[], int n)
{
if (n==1)
return (float) a [n-1];
else 
   return ((float) (findMean(a, n-1)*(n-1) + a[n-1])/n);
 }
 int main()
 {
 float Mean =0;
 int a[] = {10,12,14,16,18]
 int n = size(a)/size(a[0]);
 printf("%.2f\n",findMean(a,n));
 return 0;
 }
 
 

# iecse-task
leetcode problems

Problem Statement : Pascals Traingle
Given an integer numRows, return the first numRows of Pascal's triangle.
In Pascal's triangle, each number is the sum of the two numbers directly above it. 

Logic : 

or each next row, the number is the sum of previous row j and j-1 values, and first and last element is 1 for all. hence 2 loops r running one for number of rows and one to traverse each row. first we get the previous row and then add the 2 elements in j and j-1 position and then add it in the current row and return it. 

Problem Statement : Word Break
Given a string s and a dictionary of strings wordDict, return true if s can be segmented into a space-separated sequence of one or more dictionary words.
Note that the same word in the dictionary may be reused multiple times in the segmentation.

Logic: 

 in this i have firs ttaken an array dp whose length is 1 more than string length and all values r false except 0th pos value since every null string is considered true, hence dp[0] is true, after that ive used 2 loops one which runs from 0 to string length and one who runs for each word in the dictionary. 3 coniditions ive checked in which include; the length of string should be greater than word length, substring should be equal to word and dp[i-len] should be true. this will be i-len because if we break the string for example leetcode, when leet is already checked, for code we check if till leet everything is present.

 Probelem Statement: Maximum Product SubArray

Given an integer array nums, find a subarray that has the largest product, and return the product.
The test cases are generated so that the answer will fit in a 32-bit integer.
Note that the product of an array with a single element is the value of that element.

Logic : 

the subarray with max sum is sually max product, unless the signs are negative coz a very small negative number can be huge if multiplied with negative number. for each loop, we calc both max and min values and when negative we swap it. because when we swap and the next number is negative then we get the maximum product. we continue with swapping and then reinitialising the max, min and answer using math.min and math.max to get the subarray with max product

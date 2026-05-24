# iecse-task
leetcode problems
Problem Statement : 
Given an integer numRows, return the first numRows of Pascal's triangle.
In Pascal's triangle, each number is the sum of the two numbers directly above it. 
Logic : 
or each next row, the number is the sum of previous row j and j-1 values, and first and last element is 1 for all. hence 2 loops r running one for number of rows and one to traverse each row. first we get the previous row and then add the 2 elements in j and j-1 position and then add it in the current row and return it. 

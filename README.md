Algorithm Analysis System: Sorting and Searching

A. Project Overview
This project implements and compares the performance of fundamental algorithms: Insertion Sort, Merge Sort, and Binary Search. 
The goal is to analyze how input size and data structure affect execution time.

B. Algorithm Descriptions
Insertion Sort (Basic): A simple comparison sort that builds the final sorted array one item at a time. It is efficient for small data sets or nearly sorted data.  
Merge Sort (Advanced): A divide-and-conquer algorithm that divides the array into halves, sorts them, and merges them back together.
Binary Search: An efficient search algorithm that finds the position of a target value within a sorted array by repeatedly dividing the search interval in half.


C. Experimental Results
The following performance data was collected using System.nanoTime() on a Windows-based Java environment.

Array Size,          Insertion Sort (Basic),       Merge Sort (Advanced)
Small (10),            7,000 ns,                    7,300 ns
Medium (100),          69,800 ns,                   52,100 ns
Large (1000),         2,532,400 ns,                164,000 ns


Array Size,      Execution Time (ns)
Small (10),       3,100 ns
Medium (100),     1,500 ns
Large (1000),     1,900 ns

Which sorting algorithm performed faster? Why
1.Merge Sort performed significantly faster on large datasets. This is because its O(nlogn)complexity grows much slower than Insertion Sort's O(n^2)  

2.How does performance change with input size?
As size increases, Insertion Sort's execution time grows quadratically. Doubling the input size roughly quadruples the time. Merge Sort stays relatively stable and efficient even as n grows.  

3.How does sorted vs. unsorted data affect performance?
Insertion Sort is much faster on already sorted data O(n)  because it doesn't need to shift elements. Merge Sort's performance remains consistent regardless of initial order.

4.Do the results match Big-O complexity?
Yes. The nano-second measurements show the exponential growth predicted by O(n^2) for Insertion Sort and the logarithmic efficiency of Binary Search.  

5.Which searching algorithm is more efficient? Why?
Binary Search is more efficient than Linear Search  because it eliminates half the remaining data with every comparison.  

6.Why does Binary Search require a sorted array?
Because it relies on the logic that if the target is greater than the middle element, it must be in the right half. If the data is unsorted, this logic fails. 

D.screenshots
![img.png](docs/img.png)
![img_1.png](docs/img_1.png)



E.Reflection

This assignment demonstrated that algorithm efficiency is the most critical factor in software performance.It showed that Big O notation isn't just some abstract math it actually does a great job of predicting how a program will slow down as you feed it more data. 
My biggest problem was the timing. Using System.nanoTime() taught me how noisy a computer can be.   
# DSA-Solutions
2181. Merge Nodes in Between Zeros
. /*
Problem: Merge Nodes in Between Zeros (LeetCode #2181)
Link: https://leetcode.com/problems/merge-nodes-in-between-zeros/

Description:
You are given the head of a linked list that contains sequences of integers 
separated by nodes with value 0 (the list starts and ends with 0).
Your task is to merge the values between each pair of 0s into a single sum 
and return a new linked list containing these sums.

Example:
Input: 0 -> 3 -> 1 -> 0 -> 4 -> 5 -> 2 -> 0
Output: 4 -> 11
Explanation:
- Between first and second 0: sum = 3 + 1 = 4
- Between second and third 0: sum = 4 + 5 + 2 = 11

Approach:
- Traverse the linked list while keeping a running sum.
- When you encounter a 0:
  - If the sum is non-zero, create a new node with that sum and append it to the result list.
  - Reset the sum to 0.
- Skip the first 0 and stop at the last 0.

Time Complexity: O(n) — each node is visited once.
Space Complexity: O(1) — only a few pointers and variables used.
*/



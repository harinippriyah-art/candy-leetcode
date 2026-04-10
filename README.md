Candy - Java Solution
An efficient implementation of the Candy problem using a Two-Pass Greedy approach in Java.
Problem Description
There are n children standing in a line. Each child is assigned a rating value. You must distribute candies such that each child has at least one candy and children with a higher rating get more candies than their neighbors.
Solution Approach
This solution uses a Greedy algorithm to achieve O(n) time complexity.
It first assigns one candy to every child.
Forward Pass: Iterates from left to right; if a child has a higher rating than their left neighbor, they get one more candy than that neighbor.
Backward Pass: Iterates from right to left; if a child has a higher rating than their right neighbor, their candies are updated to max(current, neighbor + 1).
Complexity
Time Complexity: O(n)
Space Complexity: O(n)

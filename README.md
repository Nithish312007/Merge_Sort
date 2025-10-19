# 🧩 LeetCode 88 - Merge Sorted Array

## 📘 Problem Description
You are given two integer arrays **nums1** and **nums2**, both sorted in non-decreasing order, along with two integers **m** and **n**, representing the number of elements in each array.

The goal is to **merge nums2 into nums1** as one sorted array **in-place**.  
The final sorted array should be stored inside `nums1` without returning anything.

## 🧠 Example

### Example 1:
```python
Input:
nums1 = [1,2,3,0,0,0], m = 3
nums2 = [2,5,6], n = 3

Output:
[1,2,2,3,5,6]
Example 2:
python
Copy code
Input:
nums1 = [1], m = 1
nums2 = [], n = 0

Output:
[1]
Example 3:
python
Copy code
Input:
nums1 = [0], m = 0
nums2 = [1], n = 1

Output:
[1]
⚙️ Approach
This solution uses the two-pointer technique, starting from the end of both arrays.
By comparing and inserting the larger element at the end of nums1, we can efficiently merge without using extra space.

Steps:
Initialize three pointers:

i → last element of nums1's valid part (m - 1)

j → last element of nums2 (n - 1)

k → last index of nums1 (m + n - 1)

Compare elements from the back:

Place the larger one at position k.

Move pointers accordingly.

Copy remaining elements from nums2 if any.


🧮 Complexity Analysis
Complexity	Description

⏱ Time	O(m + n)
💾 Space	O(1)

🏷️ Topics
Array

Two Pointers

In-place Algorithm

Sorting

🧑‍💻 Author
Nithish Venkatesh
💡 “Code. Learn. Evolve.”


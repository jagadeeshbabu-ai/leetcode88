# LeetCode 88 - Merge Sorted Array

## Problem Statement

You are given two integer arrays `nums1` and `nums2`, sorted in non-decreasing order, and two integers `m` and `n`.

Merge `nums1` and `nums2` into a single array sorted in non-decreasing order.

The final sorted array should be stored inside `nums1`.

---

## Example

### Input

```python
nums1 = [1,2,3,0,0,0]
m = 3

nums2 = [2,5,6]
n = 3
```

### Output

```python
[1,2,2,3,5,6]
```

---

## Solution

```python
class Solution(object):
    def merge(self, nums1, m, nums2, n):

        for i in range(n):
            nums1[m+i] = nums2[i]

        nums1.sort()
```

---

## Approach

1. Copy all elements of `nums2` into the empty positions of `nums1`.
2. Sort the updated `nums1` array.
3. Since sorting is done in-place, no extra array is required.

---

## Complexity Analysis

### Time Complexity

```text
O((m+n) log(m+n))
```

Sorting dominates the overall execution time.

### Space Complexity

```text
O(1)
```

No additional data structures are used.

---

## Result

- ✅ Accepted on LeetCode
- ✅ Passed 59/59 Test Cases
- ✅ Runtime: 0 ms
- ✅ Language: Python

---

## Learning Outcomes

- Array Manipulation
- In-Place Operations
- Sorting Techniques
- Time Complexity Analysis
- LeetCode Problem Solving

---



LeetCode Problem #88 - Merge Sorted Array

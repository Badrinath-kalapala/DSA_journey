# 217. Contains Duplicate ✅

## Problem Statement
Given an integer array `nums`, return `true` if any value appears **more than once** in the array, and `false` if every element is distinct.

---

## Examples

**Example 1:**
Input: nums = [1, 2, 3, 3]
Output: true

**Example 2:**
Input: nums = [1, 2, 3, 4]
Output: false


---

## Approach
- Use a **Counter** (hashmap) to count frequencies of each element.
- If any frequency > 1, return `True`.
- Otherwise, return `False`.

---

## Code (Python)
```python
from collections import Counter
from typing import List

class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
        d = Counter(nums)
        for i in d.values():
            if i > 1:
                return True
        return False
---

## Complexity
Time Complexity: O(n) — iterates through the array once.
Space Complexity: O(n) — for storing counts in the Counter.

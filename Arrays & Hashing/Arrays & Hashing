# 242. Valid Anagram ✅

## Problem Statement
Given two strings `s` and `t`, return `true` if `t` is an anagram of `s`, and `false` otherwise.

---

## Examples

**Example 1:**
Input: s = "anagram", t = "nagaram"
Output: true

**Example 2:**
Input: s = "rat", t = "car"
Output: false

---
## Complexity
Time Complexity: O(n) — where n is the length of the strings, since Counter iterates once.

Space Complexity: O(1) — because we only store counts of 26 lowercase letters.

---

## Constraints
- 1 <= s.length, t.length <= 5 * 10⁴  
- `s` and `t` consist of lowercase English letters.  

---

## Approach
- Use Python’s `Counter` to count character frequencies in both strings.  
- If the two counters are equal → strings are anagrams.  
- Otherwise → not anagrams.  

---

## Code (Python)
```python
from collections import Counter

class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        return Counter(s) == Counter(t)


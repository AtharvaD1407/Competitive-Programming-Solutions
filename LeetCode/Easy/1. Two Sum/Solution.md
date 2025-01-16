# Approach

---

# Python
```python
class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        seen = {}
        i = 0  
        for num in nums:
            diff = target - num
            if diff in seen:
                return [seen[diff], i]
            seen[num] = i
            i += 1
```
---

# C++
```cpp
```

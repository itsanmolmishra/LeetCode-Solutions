# LeetCode-Solutions
My LeetCode problem solutions with detailed explanations

## Problem 1: Two Sum

**Difficulty:** Easy  
**Status:** ✅ Solved  
**Date:** November 18, 2025

### Problem Statement
Given an array of integers `nums` and an integer `target`, return indices of the two numbers such that they add up to `target`.

### Solution Approach
- Used a **Hash Map** for O(n) time complexity
- Single pass through the array
- Efficient lookup for complement values

### Implementation (JavaScript)

```javascript
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    // Create a hash map to store number and its index
    const map = new Map();
    
    // Loop through the array
    for (let i = 0; i < nums.length; i++) {
        // Calculate the complement needed
        const complement = target - nums[i];
        
        // Check if complement exists in map
        if (map.has(complement)) {
            return [map.get(complement), i];
        }
        
        // Store current number and its index
        map.set(nums[i], i);
    }
    
    // Return empty array if no solution found
    return [];
};
```

### Results
- ✅ All 63 test cases passed
- ⚡ Runtime: 4 ms (Beats 54.47%)
- 💾 Memory: 56.49 MB (Beats 50.96%)

### Key Takeaways
Hash maps are powerful for solving array problems that require pair finding or lookups! This solution achieves O(n) time complexity compared to the brute force O(n²) approach.

---

<!---LeetCode Topics Start-->
# LeetCode Topics
## Array
|  |
| ------- |
| [0001-two-sum](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0001-two-sum) |
## Hash Table
|  |
| ------- |
| [0001-two-sum](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0001-two-sum) |
## String
|  |
| ------- |
| [0006-zigzag-conversion](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0006-zigzag-conversion) |
| [0020-valid-parentheses](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0020-valid-parentheses) |
## Math
|  |
| ------- |
| [0007-reverse-integer](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0007-reverse-integer) |
## Stack
|  |
| ------- |
| [0020-valid-parentheses](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0020-valid-parentheses) |
## Bracket Sequences
|  |
| ------- |
| [0020-valid-parentheses](https://github.com/itsanmolmishra/LeetCode-Solutions/tree/master/0020-valid-parentheses) |
<!---LeetCode Topics End-->
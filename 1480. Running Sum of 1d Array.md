
### Problem 
https://leetcode.com/problems/running-sum-of-1d-array/description/
```
Given an array nums. We define a running sum of an array as runningSum[i] = sum(nums[0]…nums[i]).
Return the running sum of nums.
```

 ### Example
```
Example 1:

Input: nums = [1,2,3,4]
Output: [1,3,6,10]
Explanation: Running sum is obtained as follows: [1, 1+2, 1+2+3, 1+2+3+4].
Example 2:

Input: nums = [1,1,1,1,1]
Output: [1,2,3,4,5]
Explanation: Running sum is obtained as follows: [1, 1+1, 1+1+1, 1+1+1+1, 1+1+1+1+1].
Example 3:

Input: nums = [3,1,2,10,1]
Output: [3,4,6,16,17]
```
---
### Solution
```
class Solution {
    public int[] runningSum(int[] nums) {
        int[] result = new int[nums.length];
        for(int i=0; i<nums.length;i++){
            if(i==0){
                result[i]=nums[i];
            }else{
                result[i]=result[i-1]+nums[i];
            }
        }
        return result;
    }
}
```
---
### Suggestions for Improvement

#### 1.Space Complexity Optimization
Instead of allocating a new array for the result, you can transform the input array nums in place:
This approach uses only O(1) extra space, since you’re updating nums directly rather than creating a separate output array.

```
public int[] runningSum(int[] nums) {
    for (int i = 1; i < nums.length; i++) {
        nums[i] += nums[i - 1];
    }
    return nums;
}
```

#### 2 Null Check (Interview vs. Production Code)

Interview context: It’s generally acceptable to omit null checks when coding on a whiteboard or during a live‐coding session, as long as you mention edge cases verbally.
Production code: You should guard against nums being null to avoid a NullPointerException. For example:
```
if (nums == null) {
    return new int[0];
}
```



### Problem
```
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.
```

### Example
```
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].
Example 2:

Input: nums = [3,2,4], target = 6
Output: [1,2]
Example 3:

Input: nums = [3,3], target = 6
Output: [0,1]
```

### Constraints
```
2 <= nums.length <= 104
-109 <= nums[i] <= 109
-109 <= target <= 109
Only one valid answer exists.
```

---
### Solution A
```
import java.util.HashMap;

class Solution {
    public int[] twoSum(int[] nums, int target) {
        int[] output = new int[2];
        HashMap<Integer, Integer> checkMap = new HashMap<>();
        for(int i=0;i<nums.length;i++){
            int num = nums[i];
       
             if(checkMap.containsKey(target-num)){
                output =  new int[]{i,checkMap.get(target-num)};
            }   
            checkMap.put(num, i);                   
        }
        return output;
    }
}
```
### Solution B
```
import java.util.Map;
import java.util.HashMap;
class Solution {
    public int[] twoSum(int[] nums, int target) {
        int[] result = new int[2];
       Map<Integer, Integer> checkMap = new HashMap<>(); 
       for(int i=0;i<nums.length; i++){
            if(checkMap.containsKey(target-nums[i])) {
                return new int[]{i, checkMap.get(target-nums[i])};
            }
            checkMap.put(nums[i], i);
       }
        //Exception!!
        throw new IllegalArgumentException("No two sum solutions");
    }
}
```

✅ It would be better to throw an exceiption (Solution B)

🚩 "Solution A code works because the problem guarantees a valid solution. 
But in production, it's better to throw an exception in case no pair is found, to avoid returning incorrect default values."

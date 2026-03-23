TWO SUM :-
CODE 
class Solution {
    public int[] twoSum(int[] nums, int target) {
        java.util.HashMap<Integer, Integer> map = new java.util.HashMap<>();
        for (int i = 0; i < nums.length; i++) {
            int complement = target - nums[i];
            if (map.containsKey(complement)) {
                return new int[]{map.get(complement), i};
            }
            map.put(nums[i], i);
        }
        return new int[]{};
    }
}
    
<img width="1917" height="979" alt="{4471DE7A-9759-4846-8DE5-FAC10F1AA56C}" src="https://github.com/user-attachments/assets/4cddbe48-fb5d-4417-8c77-e3a7a96f5591" />

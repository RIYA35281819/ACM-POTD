class Solution {
    public void moveZeroes(int[] nums) {
        int j = 0;
        
        for (int i = 0; i < nums.length; i++) {
            if (nums[i] != 0) {
                int temp = nums[i];
                nums[i] = nums[j];
                nums[j] = temp;
                j++;
            }
        }
    }
}
<img width="1819" height="971" alt="{A20CB791-EA41-46B9-BCF7-7AAA63BEE30E}" src="https://github.com/user-attachments/assets/566ffe4d-cf24-4cec-b5a4-abd3aee402b4" />

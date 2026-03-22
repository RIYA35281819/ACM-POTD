Given an integer array nums sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once. The relative order of the elements should be kept the same.

Consider the number of unique elements in nums to be k​​​​​​​​​​​​​​. After removing duplicates, return the number of unique elements k.

The first k elements of nums should contain the unique numbers in sorted order. The remaining elements beyond index k - 1 can be ignored.
class Solution {
    public int removeDuplicates(int[] nums) {
        int i =0;
        for(int j =0 ;j<nums.length;j++){
            if(nums[i]!=nums[j]){
                nums[i+1]=nums[j];
                i++;
            }
        }
        return i+1;
    }
}

<img width="1920" height="981" alt="{E23A60A9-2546-4933-88EE-8118E9D2FC88}" src="https://github.com/user-attachments/assets/e5880632-c1bf-465a-b57d-7983960fed7b" />


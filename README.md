# Missing-Number
# An array containing n distinct numbers taken from 0, 1, 2, ..., n, find the one that is missing from the array.
class Solution {
    public int missingNumber(int[] nums) {
        int expectedSum = nums.length*(nums.length + 1)/2;
        int actualSum = 0;
        for (int num : nums) actualSum += num;
        return expectedSum - actualSum;
    }
}

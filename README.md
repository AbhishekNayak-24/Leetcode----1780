# Leetcode----1780
Check if Number is a Sum of Powers of Three
//code in java 
class Solution {
    public boolean checkPowersOfThree(int n) {
        while (n > 0) {
            int remainder = n % 3;
            if (remainder == 2) return false; // If we find '2', it's not possible
            n /= 3;
        }
        return true;
    }
}

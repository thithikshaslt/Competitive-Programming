## [Check If Array is Sorted and Rotated](https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/description/)

**Level** : Easy

---

### **Naive Approach**
1. perform nums.size() number of rotations and each time check if it is sorted, if yes return true, else return false.
(surprisingly the code was accepted)

Time Complexity : O(n^2) (for inside while)

[submission](https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/submissions/1471879531/)

---

### O(n) Approach
If the array is sorted, no matter rotated by how much, at exactly one point nums[i] will be grater than nums[i+1]. So set a variable and keep a count of this condition. Handle the case to check if the last elt is greater than than the 1st elt. If greater than 1, return false, else true.

Time Complexity : O(n) (one for loop)

[submission](https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/submissions/1458375015/)

---
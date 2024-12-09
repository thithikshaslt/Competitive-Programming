## [Remove duplicates from sorted array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/)

**Level** : Easy

---

### **Two pointer approach**
1. have a variable j, assign it to 1. another for loop from i=1 to size.

2. then in the loop check if nums[i] and nums[i-1] are equal, if equal do nothing, just let the for loop proceed. 

3. if they are unequal, then assign nums[j] to nums[i], i.e. the next non duplicate elt. increment j.

4. return j, and now all the unique elements are the first k elts in the array.

Time Complexity : O(n) (one for loop)

[submission](https://leetcode.com/problems/remove-duplicates-from-sorted-array/submissions/1474374933/)
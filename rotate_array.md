## [Rotate Array](https://leetcode.com/problems/rotate-array/)

**Level** : Medium

---

### **Naive Approach**

1. pop the last elt, insert it at the first index. repeat until specified number of times

Time Complexity : O(n) (one while loop)

[submission](https://leetcode.com/problems/rotate-array/submissions/1474384741/)

---

### **Optimal Approach**

this approach is not at all intuitive and not something that you would think of in the first instant, but anyways here's how it goes:

1. so reverse the entire list, then until k and after k reverse them separately.

For example, 

1 2 3 4 5 6 7 , k = 3

7 6 5 4 3 2 1

5 6 7 | 1 2 3 4

Time Complexity : O(n) (reverse function)

Also pay attention to the case where the number of rotations is greater than the length of the list (modulo it)

[submission](https://leetcode.com/problems/rotate-array/submissions/1474394213/)
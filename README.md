# LEETCODE-Bit-Manipulation-2914
### Code Explanation
The `minChanges` function counts the minimum number of changes required so that every two consecutive characters in the string `s` are the same. For every pair of characters `(i, i+1)`, if the characters differ, it increments the `ans` counter by one, indicating a change is needed to make them the same.

### Example Dry Run
Let's dry-run with an example input:

```java
String s = "101010";
```

1. **Initialization:**
   - `ans = 0`
   
2. **Iteration Steps:**
   - **First Iteration (i = 0):**
     - Characters: `s.charAt(0)` = '1', `s.charAt(1)` = '0'
     - Since `s.charAt(0) != s.charAt(1)`, increment `ans` by 1.
     - `ans` becomes 1.
   
   - **Second Iteration (i = 2):**
     - Characters: `s.charAt(2)` = '1', `s.charAt(3)` = '0'
     - Since `s.charAt(2) != s.charAt(3)`, increment `ans` by 1.
     - `ans` becomes 2.
   
   - **Third Iteration (i = 4):**
     - Characters: `s.charAt(4)` = '1', `s.charAt(5)` = '0'
     - Since `s.charAt(4) != s.charAt(5)`, increment `ans` by 1.
     - `ans` becomes 3.
   
3. **End of Loop:** 
   - The loop ends as `i + 1` reaches the length of the string.
   
4. **Return Value:** 
   - The method returns `ans`, which is 3.

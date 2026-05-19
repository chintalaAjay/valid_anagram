# Valid Anagram - LeetCode

## Problem Statement
Given two strings `s` and `t`, return `true` if `t` is an anagram of `s`, and `false` otherwise.

An Anagram is a word or phrase formed by rearranging the letters of another word using all the original letters exactly once.

## Example

### Input
```java
s = "anagram"
t = "nagaram"
Output
true
Approach
Convert both strings into character arrays.
Sort both arrays using Arrays.sort().
Convert arrays back to strings.
Compare both strings using .equals().

If both sorted strings are equal, then the strings are anagrams.

Java Solution
import java.util.Arrays;

class Solution {
    public boolean isAnagram(String s, String t) {
        char ch1[] = s.toCharArray();
        char ch2[] = t.toCharArray();

        Arrays.sort(ch1);
        Arrays.sort(ch2);

        String a = new String(ch1);
        String b = new String(ch2);

        return a.equals(b);
    }
}
Time Complexity
O(n log n)
Space Complexity
O(n)
Concepts Used
Strings
Character Arrays
Sorting
Arrays.sort()
String Comparison
LeetCode Problem Link

https://leetcode.com/problems/valid-anagram/

Author

Ajay Chintala

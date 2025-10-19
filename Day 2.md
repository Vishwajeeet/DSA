# Recursion Problems 


Q.1 Power of 2
**Problem Statement:** Given an integer n, write a function to determine if it is a power of two. An integer n is a power of two, if there exists an integer x such that n == 2^x.

**Approach** 

```
class Solution {
public:
    bool isPowerOfTwo(int n) {  
        if (n==1) return true;           
        if (n<=0) return false ;
        if (n%2 != 0)  {
            return false;
        }
        return isPowerOfTwo(n/2);
    }
};
```
**Time Complexity** : O(log n) 
**Space Complexity**  : O(log n) (recursion stack space)

Q.2 Reverse String
**Problem Statement:** Write a function that reverses a string. The input string is given as an array of characters s.
**Approach** 

```
class Solution {
public:
    void reverseString(vector<char>& s) {
        helper (s, 0 , s.size()-1);
        
    }
    void helper(vector<char>& s, int left, int right){
        if (left>=right) return ;

        swap(s[left],s[right]);

        helper(s, left+1 , right-1);
    }
};
```
**Time Complexity** : O(n) 
**Space Complexity**  : O(n) (recursion stack space)
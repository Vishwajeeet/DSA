# Day 3: Recursion

Q.1. Sum of n natural nos. using recursion 

**Approach** 

```
f(i,sum){
    if(i<1){
        print sum;
        return;
    }
    f(i-1,sum+i);
}
main(){
    {
        n,
        f(n,0);
    }
}

```
**Time Complexity** : O(n) 
**Space Complexity**  : O(n) (recursion stack space)

Another Approach (Using formula) 

```
f(n){
    if(n==0){
        return 0;
    }
    return n + f(n-1);
}
```
Q.2. Factorial of a number using recursion

**Approach**
```
f(n){
    if(n==0{
        return 1;

    })
    return n * f(n-1);
}
```

Q.2. Reverse a string using recursion using 1 pointer

**Approach**

```
f(i){
    if(i>=arr.size()/2){
        return;
    }
    swap(arr[i], arr[n-i-1]);
    f(i+1);
}
main(){
    arr,
    f(0);
}
```

Q.3 Palindrome Check

**Problem Statement:** Given a integer x, check if it is a palindrome using recursion.

**Approach**

```
class Solution {
public:
    bool isPalindrome(int x) {
        if (x<0) return false;

        string s = to_string(x);
        return checkifPalindrome(s, 0 , s.size()-1);
    }
    bool checkifPalindrome(string &s, int left, int right){
        if(left >= right) return true;
        if (s[left] != s[right]) return false;
        return checkifPalindrome(s, left+1 , right-1);
    }
};
```

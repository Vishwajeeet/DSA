# Recurcison Problems

Q.1 Fibonacci numbers 

**Problem Statement:** The Fibonacci numbers, commonly denoted F(n) form a sequence, called the Fibonacci sequence, such that each number is the sum of the two preceding ones, starting from 0 and 1. That is, F(0) = 0, F(1) = 1, and F(n) = F(n-1) + F(n-2) for n > 1.

**Approach** 

```
class Solution {
public:

    int solveusingrecc(int n ){
        if(n==0){
           return 0;
        }
        if(n==1){
           return 1;
        }
        int sum = solveusingrecc(n-1)+ solveusingrecc(n-2 );

        return sum ;
    }



    int fib(int n) {
        return solveusingrecc(n);
    }
};

```

**Time Complexity** : O(2^n) 
**Space Complexity**  : O(n) (recursion stack space)


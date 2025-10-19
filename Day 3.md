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

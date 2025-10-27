#Day 4 ARRAY BASICS


Q.1. **Problem Statement:** Find maximum element in an array
**Approach**

```
class Solution {
public:
    int largestElement(vector<int>& nums) {
        int largest = nums[0];
        for(int num : nums){
            if (num > largest){
                largest = num ;
            }
        }
        return largest ;

    }
};
``` 
Q.2 Second Largest Element

**Problem Statement:** Given an array of integers nums, return the second-largest element in the array. If the second-largest element does not exist, return -1.

**Approach**

```
class Solution {
public:
    int secondLargestElement(vector<int>& nums) {
        int largest = INT_MIN;
        int secondLargest = INT_MIN;

        for (int num : nums) {
            if (num > largest) {
                secondLargest = largest; // old largest becomes second largest
                largest = num;
            } else if (num > secondLargest && num != largest) {
                secondLargest = num; 
            }
        }

        // If secondLargest was never updated, return -1
        return (secondLargest == INT_MIN) ? -1 : secondLargest;
    }
};
```

Q.3. Linear Search in C

**Problem Statement:** Given an array, and an element num the task is to find if num is present in the given array or not. If present print the index of the element or print -1.

**Approach**

```
int search(int arr[],int n,int num)
{
    int i;
    for(i=0;i<n;i++)
    {
        if(arr[i]==num)
        return i;
    }
    return -1;
}
```





## Day 8
Link :- https://twitter.com/zbAnq81/status/1777233307538739526

## Code:

###

```python

#


class Solution:
     def maxSubArray(self, arr):
         n= len (arr)
         summ= arr[0]
         ans = 0
        sum2 = arr[0]
         for i in range(1, n):
             summ += arr[i]
             if summ<0:
                 sum2 = max (sum2, arr[i])
                 summ=0
             ans = max (ans, summ)
         if ans==0:
             return sum2
         else:
             return ans


```

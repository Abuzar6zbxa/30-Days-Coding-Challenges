
## Day 9
Link :- https://twitter.com/zbAnq81/status/1777621254440091829

## Code:

###

```python

# Rain water trapped problem


class Solution:
	# @param A : tuple of integers
	# @return an integer
	def trap(self, A):
        if not A:
            return 0
        
        left_max =[0] * len(A)
        right_max = [0] * len (A)
        
        left_max[0] = A[0]
        for i in range(1, len(A)):
            left_max[i] = max(left_max[i - 1], A[i])
            
        right_max[-1] = A[-1]
        for i in range(len(A) -2, -1, -1):
            right_max[i] = max(right_max[i +1], A[i])
            
        water_trapped = 0
        for i in range(len(A)):
            water_trapped += min(left_max[i], right_max[i]) - A[i]
            
        return water_trapped
	    


```

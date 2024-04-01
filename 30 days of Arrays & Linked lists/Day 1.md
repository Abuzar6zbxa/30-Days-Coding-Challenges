## Day 1
Link: (https://twitter.com/zbAnq81/status/1774731457526702469)

### Code:
```python
class Solution:
    # @param A : list of integers
    # @return an integer
    def solve(self, A):
        max_of_A = max(A)
        output = 0
        for i in A:
          if i ! = 0:
              output = max(output, i % max_of_A)
        return output
```

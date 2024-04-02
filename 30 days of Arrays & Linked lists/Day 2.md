## Day 2
Link: (https://twitter.com/zbAnq81/status/1775060156419600649)

### Code:
```python
# Return the count of such elements which have strictly smaller and greater elements

class Solution:
    # @param A : list of integers
    # @return an integer
    def solve(self, A):
        count = 0
        n = len(A)
        if n< 3:
            return count
        min_val = min(A)
        max_val = max(A)
        for ele in A :
            if ele > min+val and ele < max_val:
        return count

```

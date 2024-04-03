## Day 3
Link: (https://twitter.com/zbAnq81/status/1775415810388816304)

### Code:
```c++
# Minimum elements to be removed so that adjacent elements difference is even


int Solution::solve(vector<int> &A) {
    int even = 0, odd = 0;
    for (auto i:A){
        if (i%2) odd++;
        else even++;
        
    }
    return min(even,odd);
}


```

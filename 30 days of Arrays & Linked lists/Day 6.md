## Day 6
Link :-  https://twitter.com/zbAnq81/status/1776502041461858693

## Code:



```c++

# Kth row of pascal triangle


vector<int> Solution::getRow(int A) {
    vector<int> ans;
    int p=1;
    ans.push_back(p);
    for(int i=1;i<=A;i++){
        int c=(p*(A-i+1))/i;
        ans.push_back(c);
        p=c;
    }
    return ans;
}


```

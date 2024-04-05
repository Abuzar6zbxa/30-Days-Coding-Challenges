## Day 5
Link: (https://twitter.com/zbAnq81/status/1776230285207556387)

### Code:

# Best time to buy and sell stocks

```c++
int Solution::maxProfit(const vector<int> &A) {
    if(!A.size())
        return 0;
    int mini=A[0];
    int j=0;
    for(int i=1;i<A.size();i++){
        if(A[i]<mini){
            mini=A[i];
        }
        j=max(j,A[i]-mini);
    }
    return j;
}



```

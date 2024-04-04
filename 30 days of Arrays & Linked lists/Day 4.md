## Day 4
Link: (https://twitter.com/zbAnq81/status/1775784799409439192)

### Code:

#
```c++
int Solution::solve(vector<int> &A) {
    int ans = 0;
    int n = A.size();
    vector<int> v(n);
    int even = 0, odd = 0;
    for(int i = n-1; i>=0; i--){
        if(A[i]%2){
            v[i] = v[even] +1;
            ans = max(ans,v[i]);
            odd = i;
        }
        else{
            v[i] = v[odd] +1;
            ans = max(ans,v[i]);
            even = i;
        }
    }
    return ans;
}


```

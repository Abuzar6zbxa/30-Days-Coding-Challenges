## Day 2
Link: (https://twitter.com/zbAnq81/status/1775060156419600649)

### Code:
```c++
int Solution::solve(vector<int> &A) {
    int a=0;
    sort(A.begin(),A.end());
    for(int i=1;i<A.size()-1;i++){
        if(A[i]>A[0] && A[i]<A[A.size()-1])
            a++;
    }
    return a;
}
```

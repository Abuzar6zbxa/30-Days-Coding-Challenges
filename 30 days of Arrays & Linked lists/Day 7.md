## Day 7
Link :-  https://twitter.com/zbAnq81/status/1776877530726678665

## Code:

###

```c++
# Rotation of matrix by 90 degree


void Solution::solve(vector<vector<int> > &A) {
    for(int i=0;i<A.size();i++){
        for(int j=i+1;j<A[i].size();j++){
            swap(A[i][j],A[j][i]);
        }
        reverse(A[i].begin(),A[i].end());
    }
}


```

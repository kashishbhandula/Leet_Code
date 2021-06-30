#include <bits/stdc++.h>
using namespace std;
#define ll long long int
#define in int
#define repf(i, j, k) for (in i = j; i < k; i++)
#define repb(i, j, k) for (in i = j; i > k; i--)
#define endl "\n"
class Solution {
public:
    int minKBitFlips(vector<int>& nums, int k) {
       
        in n=nums.size();
        vector<in>temp(n+2);
        in flip=0;
        in ans=0;
        repf(i,0,n)
        {
            
            flip+=temp[i];
            if(flip&1) 
            {
                nums[i]=1-nums[i];
            }
            if(i+k-1<n)
            {
                if(!nums[i])
                {
                    flip++;
                    temp[i+k]=-1;
                     ans++;
                }
                
            }
            else
            {
                if(!nums[i]) return -1;
            }
            
          
        }
          return ans;
    }
};

class Solution:
    def lengthOfLongestAP(self, A, n):
        ans=0
        maxval=0
        for i in range(n):
            maxval=max(A[i],maxval)
        dp = [[0 for i in range(n)] for j in range(2*maxval+1)]
        for i in range(n):
            for j in range(i):
                dif=A[i]-A[j]+maxval
                dp[dif][i]=dp[dif][j]+1
                ans=max(ans,dp[dif][i])
        return ans+1

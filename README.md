# DSA-learnings

1. O(nsquare)>o(nlogn)
2. Binary search- array shuld be sorted- TC-O(logn)

Best time to buy and sell stock
class Solution {
    public int maxProfit(int[] prices) {
        int i, n=prices.length, maxprofit=0, maxprice=prices[n-1];
        for(i=n-1; i>=0; i--)
        {
            maxprice=Math.max(maxprice, prices[i]);
            maxprofit=Math.max(maxprofit,  maxprice-prices[i]);
        }
        return maxprofit;
    }
}

Sort them inplace means- without using extra space

Dutch National Flag algorithm
“I can do it in one pass using 3 pointers (Dutch National Flag approach).”
Say this clearly:
“I’ll divide array into 3 regions
left → 0s, middle → 1s, right → 2s”
low → boundary for 0
mid → current index
high → boundary for 2
[2, 1, 2, 0, 1, 0]


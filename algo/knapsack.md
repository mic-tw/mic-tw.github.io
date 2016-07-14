Knapsack Problem

最近寫到幾題背包問題的題目，但每次都要重新想過一遍，可見對於之前並沒有完全理解。所以一邊練習/複習一邊寫下筆記，看能不能檢視是否已經理解。

情境:
將一堆物品裝進包包中。每個物品都有各自的重量及價值。背包有承重限制。要求在限制內最大化裝入物品的總價值。




### 範例1
題目:給你一串數字，每個數字都可以重複挑選。以總合<= k的前提，求最大總合。
Ref: https://www.hackerrank.com/challenges/unbounded-knapsack

#### 轉化：
背包承重限制 => k
物品價值 => 數值
物品重量 => 數值

#### 解法：
如果我們知道在總合上限X，每項的數字最大總合(必定<=X)為多少(0 <= X <= k-1)。那麼總合上限為k時，最大總合(k) == Max( 最大總合(k - Number_i) + Number_i  ) for Number_i = all numbers available。

題外話：我先想過幾種DP的方法，考慮最久的是二維DP，一維是數字種類，一維是個數。當然這是失敗的D&C。







### Algo Ref
http://www.csie.ntnu.edu.tw/~u91029/KnapsackProblem.html

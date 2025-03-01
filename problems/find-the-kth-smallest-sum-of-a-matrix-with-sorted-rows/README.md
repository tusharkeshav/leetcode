<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit "Longest Continuous Subarray With Absolute Diff Less Than or Equal to Limit")
　　　　　　　　　　　　　　　　
[Next >](../evaluate-boolean-expression "Evaluate Boolean Expression")

## [1439. Find the Kth Smallest Sum of a Matrix With Sorted Rows (Hard)](https://leetcode.com/problems/find-the-kth-smallest-sum-of-a-matrix-with-sorted-rows "有序矩阵中的第 k 个最小数组和")

<p>You are given an&nbsp;<code>m&nbsp;* n</code>&nbsp;matrix,&nbsp;<code>mat</code>, and an integer <code>k</code>,&nbsp;which&nbsp;has its rows sorted in non-decreasing&nbsp;order.</p>

<p>You are allowed to choose exactly 1 element from each row to form an array.&nbsp;Return the Kth <strong>smallest</strong> array sum among all possible arrays.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,3,11],[2,4,6]], k = 5
<strong>Output:</strong> 7
<strong>Explanation: </strong>Choosing one element from each row, the first k smallest sum are:
[1,2], [1,4], [3,2], [3,4], [1,6]. Where the 5th sum is 7.  </pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,3,11],[2,4,6]], k = 9
<strong>Output:</strong> 17
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,10,10],[1,4,5],[2,3,6]], k = 7
<strong>Output:</strong> 9
<strong>Explanation:</strong> Choosing one element from each row, the first k smallest sum are:
[1,1,2], [1,1,3], [1,4,2], [1,4,3], [1,1,6], [1,5,2], [1,5,3]. Where the 7th sum is 9.  
</pre>

<p><strong>Example 4:</strong></p>

<pre>
<strong>Input:</strong> mat = [[1,1,10],[2,2,9]], k = 7
<strong>Output:</strong> 12
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>m == mat.length</code></li>
	<li><code>n == mat.length[i]</code></li>
	<li><code>1 &lt;= m, n &lt;= 40</code></li>
	<li><code>1 &lt;= k &lt;= min(200, n ^&nbsp;m)</code></li>
	<li><code>1 &lt;= mat[i][j] &lt;= 5000</code></li>
	<li><code>mat[i]</code> is a non decreasing array.</li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Binary Search](../../tag/binary-search/README.md)]
  [[Heap (Priority Queue)](../../tag/heap-priority-queue/README.md)]
  [[Matrix](../../tag/matrix/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Save all visited sums and corresponding indexes in a priority queue. Then, once you pop the smallest sum so far, you can quickly identify the next m candidates for smallest sum by incrementing each row index by 1.
</details>

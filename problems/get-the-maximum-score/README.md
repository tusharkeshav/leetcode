<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../minimum-swaps-to-arrange-a-binary-grid "Minimum Swaps to Arrange a Binary Grid")
　　　　　　　　　　　　　　　　
[Next >](../guess-the-majority-in-a-hidden-array "Guess the Majority in a Hidden Array")

## [1537. Get the Maximum Score (Hard)](https://leetcode.com/problems/get-the-maximum-score "最大得分")

<p>You are given two <strong>sorted</strong> arrays of distinct integers <code>nums1</code> and <code>nums2.</code></p>

<p>A <strong>valid<strong><em> </em></strong>path</strong> is defined as follows:</p>

<ul>
	<li>Choose&nbsp;array nums1 or nums2 to traverse (from index-0).</li>
	<li>Traverse the current array from left to right.</li>
	<li>If you are reading any value that is present in <code>nums1</code> and <code>nums2</code>&nbsp;you are allowed to change your path to the other array. (Only one repeated value is considered in the&nbsp;valid path).</li>
</ul>

<p><em>Score</em> is defined as the sum of uniques values in a valid path.</p>

<p>Return the maximum <em>score</em> you can obtain of all possible&nbsp;<strong>valid&nbsp;paths</strong>.</p>

<p>Since the answer&nbsp;may be too large,&nbsp;return it modulo&nbsp;10^9 + 7.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<p><strong><img alt="" src="https://assets.leetcode.com/uploads/2020/07/16/sample_1_1893.png" style="width: 538px; height: 163px;" /></strong></p>

<pre>
<strong>Input:</strong> nums1 = [2,4,5,8,10], nums2 = [4,6,8,9]
<strong>Output:</strong> 30
<strong>Explanation:</strong>&nbsp;Valid paths:
[2,4,5,8,10], [2,4,5,8,9], [2,4,6,8,9], [2,4,6,8,10],  (starting from nums1)
[4,6,8,9], [4,5,8,10], [4,5,8,9], [4,6,8,10]    (starting from nums2)
The maximum is obtained with the path in green <strong>[2,4,6,8,10]</strong>.
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> nums1 = [1,3,5,7,9], nums2 = [3,5,100]
<strong>Output:</strong> 109
<strong>Explanation:</strong>&nbsp;Maximum sum is obtained with the path <strong>[1,3,5,100]</strong>.
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> nums1 = [1,2,3,4,5], nums2 = [6,7,8,9,10]
<strong>Output:</strong> 40
<strong>Explanation:</strong>&nbsp;There are no common elements between nums1 and nums2.
Maximum sum is obtained with the path [6,7,8,9,10].
</pre>

<p><strong>Example 4:</strong></p>

<pre>
<strong>Input:</strong> nums1 = [1,4,5,8,9,11,19], nums2 = [2,3,4,11,12]
<strong>Output:</strong> 61
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= nums1.length &lt;= 10^5</code></li>
	<li><code>1 &lt;= nums2.length &lt;= 10^5</code></li>
	<li><code>1 &lt;= nums1[i], nums2[i] &lt;= 10^7</code></li>
	<li><code>nums1</code> and <code>nums2</code> are strictly increasing.</li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Two Pointers](../../tag/two-pointers/README.md)]
  [[Dynamic Programming](../../tag/dynamic-programming/README.md)]
  [[Greedy](../../tag/greedy/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Partition the array by common integers, and choose the path with larger sum with a DP technique.
</details>

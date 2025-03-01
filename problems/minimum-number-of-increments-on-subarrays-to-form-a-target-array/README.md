<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../number-of-good-ways-to-split-a-string "Number of Good Ways to Split a String")
　　　　　　　　　　　　　　　　
[Next >](../patients-with-a-condition "Patients With a Condition")

## [1526. Minimum Number of Increments on Subarrays to Form a Target Array (Hard)](https://leetcode.com/problems/minimum-number-of-increments-on-subarrays-to-form-a-target-array "形成目标数组的子数组最少增加次数")

<p>Given an array of positive integers <code>target</code> and an array <code>initial</code> of same size with all zeros.</p>

<p>Return the minimum number of operations to form a <code>target</code> array from <code>initial</code>&nbsp;if you are allowed to do the following operation:</p>

<ul>
	<li>Choose <strong>any</strong> subarray from <code>initial</code>&nbsp;and increment each value by one.</li>
</ul>
The answer is guaranteed to fit within the range of a 32-bit signed integer.
<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> target = [1,2,3,2,1]
<strong>Output:</strong> 3
<strong>Explanation: </strong>We need at least 3 operations to form the target array from the initial array.
[0,0,0,0,0] increment 1 from index 0 to 4&nbsp;(inclusive).
[1,1,1,1,1] increment 1 from index 1 to 3&nbsp;(inclusive).
[1,2,2,2,1] increment 1 at index 2.
[1,2,3,2,1] target array is formed.
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> target = [3,1,1,2]
<strong>Output:</strong> 4
<strong>Explanation: </strong>(initial)[0,0,0,0] -&gt; [1,1,1,1] -&gt; [1,1,1,2] -&gt; [2,1,1,2] -&gt; [3,1,1,2] (target).
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> target = [3,1,5,4,2]
<strong>Output:</strong> 7
<strong>Explanation: </strong>(initial)[0,0,0,0,0] -&gt; [1,1,1,1,1] -&gt; [2,1,1,1,1] -&gt; [3,1,1,1,1] 
                                  -&gt; [3,1,2,2,2] -&gt; [3,1,3,3,2] -&gt; [3,1,4,4,2] -&gt; [3,1,5,4,2] (target).
</pre>

<p><strong>Example 4:</strong></p>

<pre>
<strong>Input:</strong> target = [1,1,1,1]
<strong>Output:</strong> 1
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= target.length &lt;= 10^5</code></li>
	<li><code>1 &lt;= target[i] &lt;= 10^5</code></li>
</ul>

### Related Topics
  [[Array](../../tag/array/README.md)]
  [[Dynamic Programming](../../tag/dynamic-programming/README.md)]
  [[Stack](../../tag/stack/README.md)]
  [[Greedy](../../tag/greedy/README.md)]
  [[Monotonic Stack](../../tag/monotonic-stack/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
For a given range of values in target, an optimal strategy is to increment the entire range by the minimum value. The minimum in a range could be obtained with Range minimum query or Segment trees algorithm.
</details>

<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../number-of-steps-to-reduce-a-number-in-binary-representation-to-one "Number of Steps to Reduce a Number in Binary Representation to One")
　　　　　　　　　　　　　　　　
[Next >](../stone-game-iii "Stone Game III")

## [1405. Longest Happy String (Medium)](https://leetcode.com/problems/longest-happy-string "最长快乐字符串")

<p>A string is called <em>happy</em> if it does&nbsp;not have any of the strings <code>&#39;aaa&#39;</code>, <code>&#39;bbb&#39;</code>&nbsp;or <code>&#39;ccc&#39;</code>&nbsp;as a substring.</p>

<p>Given three integers <code>a</code>, <code>b</code> and <code>c</code>, return <strong>any</strong> string <code>s</code>,&nbsp;which satisfies following conditions:</p>

<ul>
	<li><code>s</code> is <em>happy&nbsp;</em>and longest possible.</li>
	<li><code>s</code> contains <strong>at most</strong> <code>a</code>&nbsp;occurrences of the letter&nbsp;<code>&#39;a&#39;</code>, <strong>at most</strong> <code>b</code>&nbsp;occurrences of the letter <code>&#39;b&#39;</code> and <strong>at most</strong> <code>c</code> occurrences of the letter <code>&#39;c&#39;</code>.</li>
	<li><code>s&nbsp;</code>will only contain <code>&#39;a&#39;</code>, <code>&#39;b&#39;</code> and <code>&#39;c&#39;</code>&nbsp;letters.</li>
</ul>

<p>If there is no such string <code>s</code>&nbsp;return the empty string <code>&quot;&quot;</code>.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> a = 1, b = 1, c = 7
<strong>Output:</strong> &quot;ccaccbcc&quot;
<strong>Explanation:</strong> &quot;ccbccacc&quot; would also be a correct answer.
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> a = 2, b = 2, c = 1
<strong>Output:</strong> &quot;aabbc&quot;
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> a = 7, b = 1, c = 0
<strong>Output:</strong> &quot;aabaa&quot;
<strong>Explanation:</strong> It&#39;s the only correct answer in this case.
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>0 &lt;= a, b, c &lt;= 100</code></li>
	<li><code>a + b + c &gt; 0</code></li>
</ul>

### Related Topics
  [[String](../../tag/string/README.md)]
  [[Greedy](../../tag/greedy/README.md)]
  [[Heap (Priority Queue)](../../tag/heap-priority-queue/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Use a greedy approach.
</details>

<details>
<summary>Hint 2</summary>
Use the letter with the maximum current limit that can be added without breaking the condition.
</details>

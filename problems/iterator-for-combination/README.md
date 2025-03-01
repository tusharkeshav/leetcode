<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../find-the-start-and-end-number-of-continuous-ranges "Find the Start and End Number of Continuous Ranges")
　　　　　　　　　　　　　　　　
[Next >](../element-appearing-more-than-25-in-sorted-array "Element Appearing More Than 25% In Sorted Array")

## [1286. Iterator for Combination (Medium)](https://leetcode.com/problems/iterator-for-combination "字母组合迭代器")

<p>Design the <code>CombinationIterator</code> class:</p>

<ul>
	<li><code>CombinationIterator(string characters, int combinationLength)</code>&nbsp;Initializes the object with&nbsp;a string&nbsp;<code>characters</code>&nbsp;of <strong>sorted distinct</strong> lowercase English letters and a number&nbsp;<code>combinationLength</code> as arguments.</li>
	<li><code>next()</code>&nbsp;Returns the next combination of length <code>combinationLength</code>&nbsp;in <strong>lexicographical order</strong>.</li>
	<li><code>hasNext()</code>&nbsp;Returns <code>true</code>&nbsp;if and only if&nbsp;there exists a next combination.</li>
</ul>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input</strong>
[&quot;CombinationIterator&quot;, &quot;next&quot;, &quot;hasNext&quot;, &quot;next&quot;, &quot;hasNext&quot;, &quot;next&quot;, &quot;hasNext&quot;]
[[&quot;abc&quot;, 2], [], [], [], [], [], []]
<strong>Output</strong>
[null, &quot;ab&quot;, true, &quot;ac&quot;, true, &quot;bc&quot;, false]

<strong>Explanation</strong>
CombinationIterator itr = new CombinationIterator(&quot;abc&quot;, 2);
itr.next();    // return &quot;ab&quot;
itr.hasNext(); // return True
itr.next();    // return &quot;ac&quot;
itr.hasNext(); // return True
itr.next();    // return &quot;bc&quot;
itr.hasNext(); // return False
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= combinationLength &lt;=&nbsp;characters.length &lt;= 15</code></li>
	<li>All the characters of <code>characters</code> are <strong>unique</strong>.</li>
	<li>At most <code>10<sup>4</sup></code>&nbsp;calls will be made to <code>next</code> and <code>hasNext</code>.</li>
	<li>It&#39;s guaranteed that all&nbsp;calls&nbsp;of the function <code>next</code>&nbsp;are valid.</li>
</ul>

### Related Topics
  [[String](../../tag/string/README.md)]
  [[Backtracking](../../tag/backtracking/README.md)]
  [[Design](../../tag/design/README.md)]
  [[Iterator](../../tag/iterator/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Generate all combinations as a preprocessing.
</details>

<details>
<summary>Hint 2</summary>
Use bit masking to generate all the combinations.
</details>

<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../count-all-possible-routes "Count All Possible Routes")
　　　　　　　　　　　　　　　　
[Next >](../number-of-ways-where-square-of-number-is-equal-to-product-of-two-numbers "Number of Ways Where Square of Number Is Equal to Product of Two Numbers")

## [1576. Replace All ?'s to Avoid Consecutive Repeating Characters (Easy)](https://leetcode.com/problems/replace-all-s-to-avoid-consecutive-repeating-characters "替换所有的问号")

<p>Given a string <code>s</code> containing only lowercase English letters and the <code>&#39;?&#39;</code> character, convert <strong>all </strong>the <code>&#39;?&#39;</code> characters into lowercase letters such that the final string does not contain any <strong>consecutive repeating </strong>characters. You <strong>cannot </strong>modify the non <code>&#39;?&#39;</code> characters.</p>

<p>It is <strong>guaranteed </strong>that there are no consecutive repeating characters in the given string <strong>except </strong>for <code>&#39;?&#39;</code>.</p>

<p>Return <em>the final string after all the conversions (possibly zero) have been made</em>. If there is more than one solution, return <strong>any of them</strong>. It can be shown that an answer is always possible with the given constraints.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> s = &quot;?zs&quot;
<strong>Output:</strong> &quot;azs&quot;
<strong>Explanation</strong>: There are 25 solutions for this problem. From &quot;azs&quot; to &quot;yzs&quot;, all are valid. Only &quot;z&quot; is an invalid modification as the string will consist of consecutive repeating characters in &quot;zzs&quot;.</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> s = &quot;ubv?w&quot;
<strong>Output:</strong> &quot;ubvaw&quot;
<strong>Explanation</strong>: There are 24 solutions for this problem. Only &quot;v&quot; and &quot;w&quot; are invalid modifications as the strings will consist of consecutive repeating characters in &quot;ubvvw&quot; and &quot;ubvww&quot;.
</pre>

<p><strong>Example 3:</strong></p>

<pre>
<strong>Input:</strong> s = &quot;j?qg??b&quot;
<strong>Output:</strong> &quot;jaqgacb&quot;
</pre>

<p><strong>Example 4:</strong></p>

<pre>
<strong>Input:</strong> s = &quot;??yw?ipkj?&quot;
<strong>Output:</strong> &quot;acywaipkja&quot;
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= s.length &lt;= 100</code></li>
	<li><code>s</code> consist of lowercase English letters and <code>&#39;?&#39;</code>.</li>
</ul>

### Related Topics
  [[String](../../tag/string/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
Processing string from left to right, whenever you get a ‘?’, check left character and right character, and select a character not equal to either of them
</details>

<details>
<summary>Hint 2</summary>
Do take care to compare with replaced occurrence of ‘?’ when checking the left character.
</details>

<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../maximum-score-words-formed-by-letters "Maximum Score Words Formed by Letters")
　　　　　　　　　　　　　　　　
[Next >](../smallest-common-region "Smallest Common Region")

## [1256. Encode Number (Medium)](https://leetcode.com/problems/encode-number "加密数字")

<p>Given a non-negative integer <code>num</code>, Return its <em>encoding</em> string.</p>

<p>The encoding is done by converting the integer to a string using a secret function that you should deduce from the following table:</p>

<p><img alt="" src="https://assets.leetcode.com/uploads/2019/06/21/encode_number.png" style="width: 164px; height: 360px;" /></p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> num = 23
<strong>Output:</strong> &quot;1000&quot;
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> num = 107
<strong>Output:</strong> &quot;101100&quot;
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>0 &lt;= num &lt;= 10^9</code></li>
</ul>

### Related Topics
  [[Bit Manipulation](../../tag/bit-manipulation/README.md)]
  [[Math](../../tag/math/README.md)]
  [[String](../../tag/string/README.md)]

### Similar Questions
  1. [Convert to Base -2](../convert-to-base-2) (Medium)

### Hints
<details>
<summary>Hint 1</summary>
Try to find the number of binary digits returned by the function.
</details>

<details>
<summary>Hint 2</summary>
The pattern is to start counting from zero after determining the number of binary digits.
</details>

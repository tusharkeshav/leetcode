<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../binary-prefix-divisible-by-5 "Binary Prefix Divisible By 5")
　　　　　　　　　　　　　　　　
[Next >](../number-of-enclaves "Number of Enclaves")

## [1019. Next Greater Node In Linked List (Medium)](https://leetcode.com/problems/next-greater-node-in-linked-list "链表中的下一个更大节点")

<p>You are given the <code>head</code> of a linked list with <code>n</code> nodes.</p>

<p>For each node in the list, find the value of the <strong>next greater node</strong>. That is, for each node, find the value of the first node that is next to it and has a <strong>strictly larger</strong> value than it.</p>

<p>Return an integer array <code>answer</code> where <code>answer[i]</code> is the value of the next greater node of the <code>i<sup>th</sup></code> node (<strong>1-indexed</strong>). If the <code>i<sup>th</sup></code> node does not have a next greater node, set <code>answer[i] = 0</code>.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>
<img alt="" src="https://assets.leetcode.com/uploads/2021/08/05/linkedlistnext1.jpg" style="width: 304px; height: 133px;" />
<pre>
<strong>Input:</strong> head = [2,1,5]
<strong>Output:</strong> [5,5,0]
</pre>

<p><strong>Example 2:</strong></p>
<img alt="" src="https://assets.leetcode.com/uploads/2021/08/05/linkedlistnext2.jpg" style="width: 500px; height: 113px;" />
<pre>
<strong>Input:</strong> head = [2,7,4,3,5]
<strong>Output:</strong> [7,0,5,5,0]
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li>The number of nodes in the list is <code>n</code>.</li>
	<li><code>1 &lt;= n &lt;= 10<sup>4</sup></code></li>
	<li><code>1 &lt;= Node.val &lt;= 10<sup>9</sup></code></li>
</ul>

### Related Topics
  [[Stack](../../tag/stack/README.md)]
  [[Array](../../tag/array/README.md)]
  [[Linked List](../../tag/linked-list/README.md)]
  [[Monotonic Stack](../../tag/monotonic-stack/README.md)]

### Hints
<details>
<summary>Hint 1</summary>
We can use a stack that stores nodes in monotone decreasing order of value.  When we see a node_j with a larger value, every node_i in the stack has next_larger(node_i) = node_j .
</details>

<!--|This file generated by command(leetcode description); DO NOT EDIT.    |-->
<!--+----------------------------------------------------------------------+-->
<!--|@author    openset <openset.wang@gmail.com>                           |-->
<!--|@link      https://github.com/openset                                 |-->
<!--|@home      https://github.com/openset/leetcode                        |-->
<!--+----------------------------------------------------------------------+-->

[< Previous](../min-stack "Min Stack")
　　　　　　　　　　　　　　　　
[Next >](../read-n-characters-given-read4 "Read N Characters Given Read4")

## [156. Binary Tree Upside Down (Medium)](https://leetcode.com/problems/binary-tree-upside-down "上下翻转二叉树")

<p>Given a binary tree where all the right nodes are either leaf nodes with a sibling (a left node that shares the same parent node) or empty, flip it upside down and turn it into a tree where the original right nodes turned into left leaf nodes. Return the new root.</p>

<p><strong>Example:</strong></p>

<pre>
<strong>Input: </strong>[1,2,3,4,5]

    1
   / \
  2   3
 / \
4   5

<strong>Output:</strong> return the root of the binary tree [4,5,2,#,#,3,1]

   4
  / \
 5   2
    / \
   3   1  
</pre>

<p><strong>Clarification:</strong></p>

<p>Confused what <code>[4,5,2,#,#,3,1<font face="monospace">]</font></code>&nbsp;means? Read more below on how binary tree is serialized on OJ.</p>

<p>The serialization of a binary tree follows a level order traversal, where &#39;#&#39; signifies a path terminator where no node exists below.</p>

<p>Here&#39;s an example:</p>

<pre>
   1
  / \
 2   3
    /
   4
    \
     5
</pre>

<p>The above binary tree is serialized as <code>[1,2,3,#,#,4,#,#,5]</code>.</p>

### Related Topics
  [[Tree](../../tag/tree/README.md)]
  [[Depth-First Search](../../tag/depth-first-search/README.md)]
  [[Binary Tree](../../tag/binary-tree/README.md)]

### Similar Questions
  1. [Reverse Linked List](../reverse-linked-list) (Easy)

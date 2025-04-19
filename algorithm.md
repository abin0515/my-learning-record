# Binary Tree
To start with, we can summarize that there are main thinking patterns for solving binary tree problems.
1.Traverse mindset: 
Think about it, can you obtain the answer by traversing the tree once? If so, implement a **traverse** function that updates an external variable as you go--this is the traversal approach.
2.Divide and conquer: 
Can you define a recursive function whose return value for each subtree leads directly to the answer for the whole tree? If so, write out that recursive function's signature and make full use of its return value--this is the **divide and conquer** approach.

And no matter which approach you choose, you should always think about the following questions:
If we abstract one individual node as a tree, what operations need to be performed on it? And when should they be done--at the pre-order, in-order, or post-order position?

Every binary-tree problem boils down to injecting your clever logic at the pre-, in-, or post-order position to achieve your goal. You only need to decide what each individual node should do; recursion will take care of applying that same operation to each node, so you don't have to worry about the rest.

For example, leetcode 104 https://leetcode.com/problems/maximum-depth-of-binary-tree/description/.
It is a problem that asks you to find the maximum depth of a binary tree.

1.traverse:
// Traversal approach
class Solution {

    // Tracks the depth as we traverse
    int depth = 0;

    // Stores the maximum depth found
    int res = 0;

    public int maxDepth(TreeNode root) {
        traverse(root);
        return res;
    }

    // Traverse the binary tree
    void traverse(TreeNode root) {
        if (root == null) {
            return;
        }

        // Pre‑order position (entering the node): increment depth
        depth++;
        // If this is a leaf, update the maximum depth
        if (root.left == null && root.right == null) {
            res = Math.max(res, depth);
        }
        traverse(root.left);
        traverse(root.right);

        // Post‑order position (leaving the node): decrement depth
        depth--;
    }
}

2.recursion(divede and conquer):
// Divide‑and‑conquer approach
class Solution {
    // Definition: given a node, return the maximum depth of the binary tree rooted at this node
    public int maxDepth(TreeNode root) {
        if (root == null) {
            return 0;
        }
        // Using the definition, compute the maximum depth of the left and right subtrees
        int leftMax = maxDepth(root.left);
        int rightMax = maxDepth(root.right);

        // Derive the maximum depth of the current tree from its subtrees:
        // The overall tree depth is the greater of the two subtree depths,
        // plus one for the root node itself
        return 1 + Math.max(leftMax, rightMax);
    }
}

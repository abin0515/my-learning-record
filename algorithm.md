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

```java
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
```

2.recursion(divede and conquer):

```java
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
```

Also, we have another way to solve this problem--level order traversal.
Binary tree problems are primarily designed to develop recursive thinking, whereas level-order trvaversal is an iterative approach and is relatively straightforward.

```java
int levelTraverse(TreeNode root) {
    if (root == null) return 0; // Modified return to 0 for null root
    Queue<TreeNode> q = new LinkedList<>();
    q.offer(root);
    int maxDepth = 0;
    // iterate through each level from top to bottom
    while (!q.isEmpty()) {
        int sz = q.size();
        maxDepth++;
        // iterate through each node in the current level from left to right
        for (int i = 0; i < sz; i++) {
            TreeNode cur = q.poll();
            // store next level nodes
            if (cur.left != null) {
                q.offer(cur.left);
            }
            if (cur.right != null) {
                q.offer(cur.right);
            }
        }
    }
    return maxDepth;
}
```

# BackTrack
Solving a backtrack problem is essentially a process of **traversing a decision tree**, where each **leaf node** represents a valid solution to the problem. By travering the decision tree and collecting all the answers at the leaf nodes, we can obtain all valid solutions to the problem.

when we at a decision tree node, we should consider three things:

1.path: what we have chosen so far

2.options: what we can choose at current node

3.base case: when we reach the leaf node, we can not do more decision again, return the path

backtrack template:

```java
List<Integer> res = new ArrayList<>();
public void backtrack(List<Integer> path, int[] options) {
    if /*satisfy base case*/{ 
        res.add(path);
        return;
    }
    for (int option : options) {
        // do decision
        backtrack(path, options);
        // undo decision
    }
}
```
The core idea is that we do recursion inside the for loop: **"make a choice"** before the recursive call and **"undo the choice"** after the recursive call.

## Now, we use backtrack template to solve permutation, combination, and subset problem:

Whether it's a permutation, combination, or subset problem, simply put, they all involve selecting a number of elements from a sequence nums based on certain rules. There are mainly the following variations:

## Form 1: Elements are unique and cannot be reused.
This is the most basic form — all elements in nums are distinct, and each element can be used at most once.

For example, in a combination problem, if the input is nums = [2, 3, 6, 7], the only valid combination that sums to 7 would be [7].

## Form 2: Elements may repeat in nums but cannot be reused.
In this case, nums may contain duplicate elements, but each element can still be used at most once.

For example, in a combination problem, if the input is nums = [2, 5, 2, 1, 2], valid combinations that sum to 7 would include [2, 2, 2, 1] and [5, 2].

## Form 3: Elements are unique and can be reused.
Here, elements in nums are distinct, but each element can be chosen multiple times.

For example, in a combination problem, if the input is nums = [2, 3, 6, 7], valid combinations that sum to 7 would be [2, 2, 3] and [7].

Of course, you could also consider a fourth form, where elements may repeat and can also be reused. But since elements can be reused, having duplicates in nums becomes redundant. Once duplicates are removed, it becomes equivalent to Form 3, so this case doesn't need separate consideration.

The examples above are based on combination problems, but the same three basic forms apply to permutations, combinations, and subsets — resulting in a total of 9 possible variations.

## Subset(Elements are unique and cannot be reused):

For example, leetcode 78 https://leetcode.cn/problems/subsets/

```java
class Solution {
    List<List<Integer>> res = new LinkedList<>();
    List<Integer> track = new LinkedList<>();
    public List<List<Integer>> subsets(int[] nums) {
        
        backtrack(nums, 0);
        return res;
    }

    void backtrack(int[] nums, int start){
        // base case
        // we do not need to check base case here, after the for loop, function will end
        res.add(new LinkedList<>(track));
        for(int i = start; i < nums.length; i++){
            // do decision
            track.add(nums[i]);
            backtrack(nums, i + 1);
            // undo decision
            track.removeLast();
        }
    }
}
```

## Combination(Elements are unique and cannot be reused):

For example, leetcode 77 https://leetcode.cn/problems/combinations/
```java
class Solution {
    List<List<Integer>> res = new LinkedList<>();
    List<Integer> track = new LinkedList<>();

    public List<List<Integer>> combine(int n, int k) {
        backtrack(n, k, 1);
        return res;
    }
    void backtrack(int n, int k, int start){
        //base case, we only need to add 2 number combination to res
        if(track.size() == k){
            res.add(new LinkedList<>(track));
        }
        for(int i = start; i <= n; i++){
            track.add(i);
            
            backtrack(n, k, i + 1);
            track.removeLast();
        }
    }
}
```

## Permutation(Elements are unique and cannot be reused):
For example, leetcode 46 https://leetcode.cn/problems/permutations/
```java
class Solution {
    List<List<Integer>> res;
    List<Integer> track;
    boolean[] used;
    public List<List<Integer>> permute(int[] nums) {
        int n = nums.length;
        res = new LinkedList<>();
        used = new boolean[n];
        track = new LinkedList<>();
        backtrack(nums, track, used);
        return res;
    }
    void backtrack(int[] nums, List<Integer> track, boolean[] used){
        if(track.size() == nums.length){
            res.add(new LinkedList<>(track));
            return;
        }
        for(int i = 0; i < nums.length; i++){
            if(used[i]){
                continue;
            }
            track.add(nums[i]);
            used[i] = true;
            backtrack(nums, track, used);
            track.removeLast();
            used[i] = false;

        }
    }
}
``` 

## Subset and Combination(Elements are not unique and cannot be reused):
Combination is kind of same as subset, but we need to add a pruning logic to avoid duplicate combinations.

let see subset code first:

For example, leetcode 90 https://leetcode.cn/problems/subsets-ii/
```java
class Solution {
    List<List<Integer>> res = new LinkedList<>();
    List<Integer> track = new LinkedList<>();
    public List<List<Integer>> subsetsWithDup(int[] nums) {
        Arrays.sort(nums);
        backtrack(nums, 0);
        return res;
    }
    void backtrack(int[] nums, int start){
        res.add(new LinkedList<>(track));
        for(int i = start; i < nums.length; i++){
            if(i > start && nums[i] == nums[i - 1]){
                continue;
            }
            track.add(nums[i]);
            backtrack(nums, i + 1);
            track.removeLast();
        }
    }
}
```

This piece of code is almost identical to the standard subset problem code, with the addition of sorting and pruning logic

Then, let's look at the combination problem:

For example, leetcode 40 https://leetcode.cn/problems/combination-sum-ii/description/

```java
class Solution {
    List<List<Integer>> res = new LinkedList<>();
    List<Integer> track = new LinkedList<>();
    public List<List<Integer>> combinationSum2(int[] candidates, int target) {
        int pathSum = 0;
        Arrays.sort(candidates);
        backtrack(candidates, 0, pathSum, target);
        return res;
    }
    void backtrack(int[] candidates, int start, int pathSum, int target){
        if(pathSum == target){
            res.add(new LinkedList<>(track));
            return;
        }
        if(pathSum > target){
            return;
        }
        for(int i = start; i < candidates.length; i++){
            if(i > start && candidates[i] == candidates[i - 1]){
                continue;
            }
            track.add(candidates[i]);
            pathSum += candidates[i];
            backtrack(candidates, i + 1, pathSum, target);
            track.removeLast();
            pathSum -= candidates[i];
        }
    }
}
```
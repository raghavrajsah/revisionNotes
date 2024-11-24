# Recurison

### **What is Recursion?**
Recursion is when a function **calls itself** to solve a smaller subproblem, and the solutions to these subproblems combine to solve the original problem.




### **Simplified Template**
Use this **general template** to avoid getting confused:
```java
ReturnType recursion(Parameters params) {
    // 1. Base Case: Stop recursion
    if (baseCondition) {
        return baseResult;
    }

    // 2. Recursive Case: Break into smaller subproblems
    ReturnType leftResult = recursion(smallerSubproblem1);
    ReturnType rightResult = recursion(smallerSubproblem2);

    // 3. Combine Results: Merge subproblem results
    ReturnType result = combine(leftResult, rightResult);

    return result;
}
```


#### **Example 1: Factorial**
```java
int factorial(int n) {
    // Base Case
    if (n == 0) return 1;

    // Recursive Case
    return n * factorial(n - 1);
}
```

#### **Example 2: Fibonacci**
```java
int fibonacci(int n) {
    // Base Case
    if (n <= 1) return n;

    // Recursive Case
    return fibonacci(n - 1) + fibonacci(n - 2);
}
```

#### **Example 3: Binary Tree Maximum Depth**
```java
int maxDepth(TreeNode root) {
    // Base Case
    if (root == null) return 0;

    // Recursive Case
    int leftDepth = maxDepth(root.left);
    int rightDepth = maxDepth(root.right);

    return Math.max(leftDepth, rightDepth) + 1;
}
```



# Heap Notes

### **How to Identify Heap/Queue Problems**
Look for these keywords in the problem:
1. **Top K**: "Find the K largest/smallest/frequent..."
2. **Priority**: "Process tasks in order of priority..."
3. **Shortest Path**: "Find the shortest path from X to Y..."
4. **Sliding Window**: "Find max/min/median in a window..."
5. **Intervals**: "Schedule tasks, minimize overlap, or count intervals."

If any of these patterns show up, it's a strong hint that a **heap/priority queue** could be useful.

---

### **Quick Recap of Common Use Cases**
| **Use Case**                     | **Heap Type**          | **Key Approach**                                     |
|-----------------------------------|------------------------|-----------------------------------------------------|
| Top K Elements                   | Min-Heap               | Maintain a heap of size \(K\).                     |
| Merge K Sorted Lists             | Min-Heap               | Store smallest element of each list.               |
| Shortest Path (Dijkstra)         | Min-Heap               | Always process the node with the smallest distance.|
| Sliding Window Maximum           | Max-Heap               | Keep track of largest element in window.           |
| Task Scheduling                  | Min-Heap/Max-Heap      | Process tasks by time or frequency.                |
| Median in Data Stream            | Min-Heap + Max-Heap    | Balance elements to calculate median.              |
| Meeting Rooms II                 | Min-Heap               | Track earliest finishing intervals.                |

---

Let me know if you'd like to dive deeper into any specific use case or see a problem worked through! 😊

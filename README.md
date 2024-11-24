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

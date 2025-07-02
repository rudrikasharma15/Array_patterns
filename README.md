# 🌟 Array DSA Patterns  
**Author: Rudrika Sharma**

🧩 ARRAY PATTERNS (with Examples)

1. Sliding Window → Efficient handling of subarrays  
2. Two Pointers → Comparing/moving across a sorted array  
3. Prefix Sum → Fast range sum queries  
4. Hashing / HashMap / HashSet → Track frequencies, subarrays  
5. Monotonic Stack / Deque → Next Greater/Smaller Element  
6. Binary Search on Answer → Optimize over value space  
7. Greedy → Locally best → globally optimal  
8. Kadane's Algorithm → Max subarray sum  
9. Sorting + Two Pointers → Pair/triplet matching after sort  
10. Difference Array → Fast range updates  
11. Bit Manipulation → XOR tricks, subsets  
12. Backtracking → Generate all valid combinations  

---

## 1. 🪟 Sliding Window
Use when the problem involves subarrays of fixed or variable size (max/min/sum/count).

### 🧠 Technique:
- Fixed window: move `right` pointer forward, slide window by moving `left`
- Variable window: expand `right`, shrink `left` when constraints break

### 🔹 Examples:
- Maximum Sum Subarray of Size K  
- Minimum Size Subarray Sum  
- Longest Substring with K Distinct Characters *(string variant)*  

---

## 2. 🎯 Two Pointers
Use when the array is sorted or requires comparing/moving from both ends.

### 🧠 Technique:
- One pointer at start, one at end
- Move based on condition (sum, duplicate, etc.)

### 🔹 Examples:
- Two Sum II (sorted)  
- Remove Duplicates from Sorted Array  
- Merge Sorted Arrays  
- Sort Colors  

---

## 3. ➕ Prefix Sum
Use when calculating range sums or subarray sums efficiently.

### 🧠 Technique:
- Build prefix sum array
- `sum(l, r) = prefix[r] - prefix[l - 1]`

### 🔹 Examples:
- Subarray Sum Equals K  
- Find Pivot Index  
- Range Sum Query  

---

## 4. 🧠 Hashing (HashMap / HashSet)
Use when frequency count, lookup, or subarray uniqueness matters.

### 🧠 Technique:
- HashMap → store counts, indices  
- HashSet → track seen elements  

### 🔹 Examples:
- Two Sum  
- Contains Duplicate  
- Longest Consecutive Sequence  
- Subarray with Sum 0  

---

## 5. 📉 Monotonic Stack / Deque
Use for problems involving next greater/smaller element, or range queries.

### 🧠 Technique:
- Stack stores indices or values in increasing/decreasing order  
- Pop when current element breaks monotonic condition

### 🔹 Examples:
- Next Greater Element  
- Daily Temperatures  
- Largest Rectangle in Histogram  
- Sliding Window Maximum  

---

## 6. 🔍 Binary Search on Answer
Use when you need to find min/max value that satisfies a condition — not position in array.

### 🧠 Technique:
- Binary search over possible **values**, not array indices  
- Use greedy check function inside

### 🔹 Examples:
- Koko Eating Bananas  
- Minimum Days to Make M Bouquets  
- Aggressive Cows  
- Allocate Minimum Pages  

---

## 7. ⚡ Greedy
Use when making locally optimal choices leads to global optimum.

### 🧠 Technique:
- Sort if needed  
- Always take the best option for current state

### 🔹 Examples:
- Jump Game I / II  
- Merge Intervals  
- Gas Station  
- Candy Distribution  

---

## 8. 💥 Kadane's Algorithm
Use when finding maximum sum of a **contiguous subarray**.

### 🧠 Technique:
- Track local max and update global max  
```java
currMax = Math.max(arr[i], currMax + arr[i]);
maxSum = Math.max(maxSum, currMax);
```

### 🔹 Examples:
- Maximum Subarray (Leetcode #53)
- Maximum Circular Subarray
- Maximum Sum of 2 Non-Overlapping Subarrays

---

## 9. 🧮 Sorting + Two Pointers
Use for problems involving triplets, closest pairs, or comparing across sorted arrays.

### 🧠 Technique:
- Sort the array
- Fix one index, apply two-pointer from both sides on the rest

### 🔹 Examples:
- 3Sum  
- 4Sum  
- Closest Pair from Two Arrays  
- Meeting Rooms (Interval Overlap)  

---

## 10. 🧾 Difference Array (Advanced)
Use for **efficient range updates** in O(1) when multiple operations are applied.

### 🧠 Technique:
- Apply delta at `start`, subtract at `end + 1`
- Do prefix sum at end to get final array

```java
diff[start] += value;
diff[end + 1] -= value;
```

### 🔹 Examples:
- Range Addition  
- Corporate Flight Bookings  
- Car Pooling  

---

## 11. 🧩 Bit Manipulation
Use for problems involving XOR, toggling bits, finding unique numbers, subsets, or masks.

### 🧠 Technique:
- Use `XOR` to cancel out duplicate numbers  
- Use bit masking to generate subsets

### 🔹 Examples:
- Single Number (Leetcode #136)  
- Find Missing Number  
- Subsets using Bitmasks  
- Bitwise AND of Numbers Range  

---

## 12. 🔄 Backtracking on Arrays
Use when generating all combinations, permutations, or valid partitions.

### 🧠 Technique:
- Use recursion to explore choices  
- Backtrack by undoing choices after recursive call

### 🔹 Examples:
- Subsets / Subsets II  
- Permutations  
- Combination Sum  
- N-Queens (2D variant)  

---


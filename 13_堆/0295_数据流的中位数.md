# 295. 数据流的中位数

## 题目描述

中位数是有序整数列表中的中间值。如果列表的大小是偶数，则没有中间值，中位数是两个中间值的平均值。

请你设计一个支持以下两种操作的数据结构：

- `void addNum(int num)` - 从数据流中添加一个整数到数据结构中。
- `double findMedian()` - 返回目前所有元素的中位数。

## 示例

**示例 1：**

```
输入:
["MedianFinder", "addNum", "addNum", "findMedian", "addNum", "findMedian"]
[[], [1], [2], [], [3], []]
输出:
[null, null, null, 1.5, null, 2.0]

解释:
MedianFinder medianFinder = new MedianFinder();
medianFinder.addNum(1);    // arr = [1]
medianFinder.addNum(2);    // arr = [1, 2]
medianFinder.findMedian(); // 返回 1.5 ((1 + 2) / 2)
medianFinder.addNum(3);    // arr = [1, 2, 3]
medianFinder.findMedian(); // 返回 2.0
```

## 提示

- `-10⁵ <= num <= 10⁵`
- 在调用 `findMedian` 之前，数据结构中至少有一个元素
- 最多 `5 * 10⁴` 次调用 `addNum` 和 `findMedian`

**本周学习的是数组、链表、双端链表、跳表，栈、队列、双端队列、优先队列的等数据结构及算法实现。**

# 1、数组(Array)

是有序的，每个元素有代表的它的索引，查询快、增删慢。

平均时间复杂度，查询O(n)，新增O(n),删除O(n);

空间复杂度是O(n)

# 2、单链表(Singly LinkedList)

当前节点指向下一个节点，增删快，查询慢。

平均时间复杂度：查询O(n), 新增O(1),删除O(1)；

空间复杂度：O(n)

# 3、双端链表(Double LinkedList)

当前节点即有next指向下一个节点，也有prev指向上一个节点。

平均时间复杂度：查询O(n)， 新增O(1)，删除O(1)

空间复杂度：O(n)

# 4、跳表(Skip List)

搜索从最稀疏的子序列开始，直到找到两个连续的元素，一个小于或等于或大于等于搜索到的元素。通过链接的层次结构，这两个元素链接到下一个最稀疏子序列的元素，在该子序列中继续搜索，直到最终我们以完整序列搜索。

就是将整个链表抽层出来，最低层是整个链表数据，

![image-20200628122428719](/Users/shizhenqiang/Library/Application%20Support/typora-user-images/image-20200628122428719.png)

先判断最高层的数，如果小再找下一层左边的数进行比较，如果大于，则找右边。依次类推。最终找到要查询的值。

# 5、栈(Stack)

栈的特性是先进后出。

平均时间复杂度：查询O(n)，新增O(1)，删除O(1)

空间复杂度：O(n)

# 6、队列(Queue)

队列的特性是：先进先出

平均时间复杂度：查询O(n)，新增O(1)，删除O(1)

空间复杂度：O(n)

# 7、双端队列(Double Queue)

两边都可以添加和删除数据，在两边都可以作为 先进先出

平均时间复杂度：查询O(n)，新增O(1)，删除O(1)

空间复杂度：O(n)

# 8、优先队列(PriorityQueue)

是一个无界、值不为null且进行排序过的队列。

添加数据，需要根据Comparator进行排序，比如插入的是整数类型，会根据元素的大小进行排序。小的在最前面，也可以自定义Comparator根据什么规则进行排序。




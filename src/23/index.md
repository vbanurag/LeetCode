因为这道题的思路也比较繁琐这里也详细记录一下

先设 传入队列数组为 lists, 其长度为 n

#### 第一步
首先我们可以对列表当前节点的值升序排序排序

#### 第二步
然后取出lists[0]，并将lists[0]指向 lists[0].next

#### 第三步

检测lists[0]是否为空，如果为空则从数组中移除队列,
如果不为空，则将数组插入到其值大小对应的位置，这里可以使用二分法来找到插入的位置

#### 第四步

如果 lists.lengt > 1 则继续第二步，否则将lists[0]的值全部提取出来
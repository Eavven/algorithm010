学习笔记

第一部分：priority queue python源代码分析
python中的PriorityQueue里使用的heapq这个数据结构，heapq是一个二叉树
其父节点的值恒小于或等于其孩子节点的值，因此最小的值位于根节点上

class PriorityQueue(Queue):
    '''Variant of Queue that retrieves open entries in priority order (lowest first).
    Entries are typically tuples of the form:  (priority number, data).
    '''

    def _init(self, maxsize):
        self.queue = []

    def _qsize(self):
        return len(self.queue)
    
    
    # heappush操作，将value置入heapq中
    def _put(self, item):
        heappush(self.queue, item)
    
    #heappop操作将弹出最小值也就是根节点，如果heapq为空，返回IndexError
    def _get(self):
        return heappop(self.queue)
 
第二部分：总结

老师做题建议：课前预习题，LC每日一题，经典例题，课后习题
考虑问题时，有暴力先考虑暴力方法，找到重复子问题
栈解决最近邻，队列解决先进先出，像sliding window的题目用滑动窗口解决即可，是种套路

本周算法题有上课例题，实战题还有作业题，大概一个算法题如果有多重解法的话，再加上理解和每个解法过五次，大概一个算法题就要一个多小时。所有本周的题量并没完成。之后要匀出更多的时间，并且去提高效率、

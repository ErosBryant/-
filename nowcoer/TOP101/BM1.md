## <span style="color:red">Point : List</span>

## BM1 反转链表

#### `描述`
给定一个单链表的头结点pHead(该头节点是有值的，比如在下图，它的val是1)，长度为n，反转该链表后，返回新链表的表头。

数据范围： 0\leq n\leq10000≤n≤1000

要求：空间复杂度 O(1)O(1) ，时间复杂度 O(n)O(n) 。

如当输入链表{1,2,3}时，
经反转后，原链表变为{3,2,1}，所以对应的输出为{3,2,1}。

以上转换过程如下图所示：![](https://uploadfiles.nowcoder.com/images/20211014/423483716_1634206291971/4A47A0DB6E60853DEDFCFDF08A5CA249)

              输入：               返回值：
              {1,2,3}             {3,2,1}
            
              
---
`ANS`

```python3
class Solution:
    def ReverseList(self , head: ListNode) -> ListNode:
        #处理空链表
        if not head:
            return None
        cur = head # 지금 node 
        pre = None # 이전 node 
        while cur:
            # next node의  point 를 temp에 저장 
            temp = cur.next 
            
            # 처음 : next node point을 null 즉 없애기 
            # 다음부터 : 이전 loop의 cur이 cur.point가 됨  
            cur.next = pre
            
            # 지금 값을 pre 이로 저장 
            pre = cur 
            
            # next node의  point를 cur로 
            cur = temp
        return pre

# 다음걸 temp에 저장하고 none 하고 , 지금 걸  pre에 저장하고  다음 값을 지금 변수에 저장  
# 노드가  있대까지 계속 
              
```     
![](https://uploadfiles.nowcoder.com/images/20211001/397721558_1633084777359/E53A90674EDC6B8D31549D8DF4E7B38E)

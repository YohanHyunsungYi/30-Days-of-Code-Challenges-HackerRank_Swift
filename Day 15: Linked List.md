## Day 15: Linked List
https://www.hackerrank.com/challenges/30-linked-list/problem

### Solution
```
func insert(head: Node!, data: Int!) -> Node {
    // Enter your code here.   
    if head == nil
    {
        let newNode = Node(data: data)
        //head.next = newNode
        return newNode
    }
    else
    {
        var lastNode: Node! = head
        let newNode = Node(data: data)
        while lastNode.next != nil
        {
            lastNode = lastNode.next
        }
    
        lastNode.next = newNode
    }
    
    return head
}
```

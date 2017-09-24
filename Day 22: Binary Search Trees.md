## Day 22: Binary Search Trees
https://www.hackerrank.com/challenges/30-binary-search-trees/problem

### Solution
```
 func getHeight(root: Node?) -> Int {
    	// Complete the function
        
        if let root = root {
			let leftHeight = getHeight(root: root.left) + 1
			let rightHeight = getHeight(root: root.right) + 1
			
			return leftHeight > rightHeight ? leftHeight : rightHeight
		}
		else {
			return -1
		}
 } // End of get Height function
```

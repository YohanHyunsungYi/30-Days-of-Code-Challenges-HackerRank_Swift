## Day 14: Scope
https://www.hackerrank.com/challenges/30-scope/problem

### Solution
```
init (a: [Int]){
	self.elements = a
    }
    
    func computeDifference(){
        maximumDifference = 0 
		for i in elements {
			for j in elements {
				if abs(i-j) > maximumDifference{
					maximumDifference = abs(i-j)
				}
			}			
		}
  }
```

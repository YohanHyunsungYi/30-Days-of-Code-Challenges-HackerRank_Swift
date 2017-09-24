## Day 10: Binary Numbers
https://www.hackerrank.com/challenges/30-binary-numbers/problem

### Solution
```
import Foundation

let number = String(Int(readLine()!)!, radix: 2)
var result = 0, high = 0

for i in number.characters{
	if i == "1"{
		result += 1
		if result > high{
			high = result
		}
	}else{
		result = 0
	}
}

print(high)
```

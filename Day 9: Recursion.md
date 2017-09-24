## Day 9: Recursion
https://www.hackerrank.com/challenges/30-recursion/problem

### Solution
```
import Foundation

let number = Int(readLine()!)!

func factorial(_ Number: Int) -> Int {
   	if Number > 1 {
		return Number * factorial(Number-1)	
	}else{
		return Number
	}	
}

print(factorial(number))
```

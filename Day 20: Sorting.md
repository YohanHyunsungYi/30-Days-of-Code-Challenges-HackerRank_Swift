## Day 20: Sorting
https://www.hackerrank.com/challenges/30-sorting/problem

## Solution
```
import Foundation

// read the integer n
let n = Int(readLine()!)!

// read the array
let arr = readLine()!.components(separatedBy: " ").map{ Int($0)! }

var count = 0
var endPosition = n-1
var arry = arr

while endPosition > 0{
	var swapPosition = 0
	for i in 0..<endPosition{
		if arry[i] > arry[i + 1] {
			// Swap elements 'i' and 'i + 1':
			var tmp = arry[i]
			arry[i] = arry[i + 1]
			arry[i + 1] = tmp
			swapPosition = i
			count += 1
		} // end if
	} // end for
	endPosition = swapPosition
} // end while

print("Array is sorted in \(count) swaps.")
print("First Element: \(arry[0])")
print("Last Element: \(arry[n-1])")
```

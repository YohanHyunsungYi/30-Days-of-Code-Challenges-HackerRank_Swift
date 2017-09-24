## Day 7: Arrays
https://www.hackerrank.com/challenges/30-arrays/problem

### Solution
```
import Foundation

// number of elements
let n = Int(readLine()!)!

// read array
let arr = readLine()!.components(separatedBy: " ").map{ Int($0)! }

// iterate over the array in reverse order and print the elements separated by space
var result : String = ""

var j = n-1
for i in 0...(n-1) {
    result.append(String(arr[j]))
    result.append(" ")    
    j -= 1
}

print(result)
```

## Simple Array Sum

https://www.hackerrank.com/challenges/simple-array-sum/problem


### Solution

```
import Foundation

// number of elements
let n = Int(readLine()!)!

// read array and map the elements to integer
let arr = readLine()!.components(separatedBy: " ").map{ Int($0)! }

// find and print the sum of array
var result = 0
for i in 0...(n-1) {
    result += arr[i]
}
print(result)
```

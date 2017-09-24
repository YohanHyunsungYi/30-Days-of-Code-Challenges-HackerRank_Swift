## Compare the Triplets

https://www.hackerrank.com/challenges/compare-the-triplets/problem



### Solution

```
import Foundation

// Enter your code here 

let bob = readLine()!.components(separatedBy: " ").map{ Int($0)! }
let alice = readLine()!.components(separatedBy: " ").map{ Int($0)! }


var bobScore = 0
var aliceScore = 0

for i in 0...2 {
    if bob[i] > alice[i]{
        bobScore += 1
    }else if bob[i] < alice[i]{
        aliceScore += 1
    }
}
print("\(bobScore) \(aliceScore)")
```

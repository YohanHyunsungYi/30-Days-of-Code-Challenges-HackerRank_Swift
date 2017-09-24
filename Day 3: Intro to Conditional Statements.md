## Day 3: Intro to Conditional Statements

https://www.hackerrank.com/challenges/30-conditional-statements/problem

### Solution

```
// Enter your code here 

import Foundation

let n = Int(readLine()!)!

if n%2 == 0 {
    if 2 <= n && n <= 5 {
        print("Not Weird")
    }else if 6 <= n && n <= 20{
        print("Weird")
    }else{
        print("Not Weird")
    }
}else{
    print("Weird")
}
```

## Day 8: Dictionaries and Maps
https://www.hackerrank.com/challenges/30-dictionaries-and-maps/problem

### Solution
```
// Enter your code here. Read input from STDIN. Print output to STDOUT

import Foundation

let numberOfDic = Int(readLine()!)!
var Dictionarys : [String:Int] = [:]

for _ in 0 ..< numberOfDic {
    let temp = readLine()!.components(separatedBy: " ").map{ String($0)! }
    Dictionarys["\(temp[0])"] = Int(temp[1])
}

while let findingKey = readLine() {
    var result = 0    
    if Dictionarys["\(findingKey)"] != nil {
        result = Dictionarys["\(findingKey)"]!
        print("\(findingKey)=\(result)")
    }else{
        print("Not found")
    }
}
```

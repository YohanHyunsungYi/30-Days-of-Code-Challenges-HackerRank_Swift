## Day 6: Let's Review
https://www.hackerrank.com/challenges/30-review-loop/problem

### Solution
```
import Foundation
import Darwin

let numStrings = Int(readLine()!)!

func printEvenAndOdd(string: String) {   
    var even = "", odd = ""
	var j = 1 
    
	for i in string.characters{
		if j == 0 {
			even.append(i)
		}else if j != 0 && (j + 1) % 2 == 0{
			even.append(i)
		}else if j != 0 && (j + 1) % 2 != 0{
			odd.append(i)
		}
		j += 1
	}
    print("\(even) \(odd)")
}

for _ in 1...numStrings {
    let inputString = readLine()!
    printEvenAndOdd(string: inputString)
}
```

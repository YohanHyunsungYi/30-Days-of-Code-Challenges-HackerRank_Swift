## Day 2: Operators

https://www.hackerrank.com/challenges/30-operators/problem

### Solution

```
// Enter your code here. Read input from STDIN. Print output to STDOUT
import Foundation

let mealCost = Double(readLine()!)!
let tipPercent = Double(readLine()!)!
let taxPercent = Double(readLine()!)!

let tip = mealCost * (tipPercent/100)
let tax = mealCost * (taxPercent/100)

var totalCost = mealCost + tip + tax

totalCost = totalCost.rounded()

print ("The total meal cost is \(Int(totalCost)) dollars.")
```

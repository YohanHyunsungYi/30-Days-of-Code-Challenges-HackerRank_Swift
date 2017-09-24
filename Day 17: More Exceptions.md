## Day 17: More Exceptions
https://www.hackerrank.com/challenges/30-more-exceptions/problem

### Solution
```
// Start of class Calculator
class Calculator {
    // Start of function power
    func power(n: Int, p: Int) throws -> Int {
        
        if n == 0{
			return 0
		}
		
		if p == 0{
			return 1
		}
		
        guard n >= 0 && p >= 0 else {
            throw RangeError.NotInRange("n and p should be non-negative")
        }
        
        var result = n
		for _ in 1 ..< p{
			result = result * n
		}
		
		return result
        // Add your code here

    } // End of function power
} // End of class Calculator
```

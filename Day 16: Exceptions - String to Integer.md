## Day 16: Exceptions - String to Integer
https://www.hackerrank.com/challenges/30-exceptions-string-to-integer/problem

## Solution
```
/*
 * If typecasting is not possible, throw exception, otherwise return the Integer value
*/
 
func stringToInt(inputString: String) throws -> Int {
    // Write your code here
    
    guard let result = Int(inputString) else{
        throw StringToIntTypecastingError.BadString
    }
    
    return result    
}
```


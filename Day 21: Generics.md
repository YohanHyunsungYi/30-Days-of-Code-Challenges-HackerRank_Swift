## Day 21: Generics
https://www.hackerrank.com/challenges/30-generics/problem

### Solution
```
struct Printer<T> {
	/**
	*    Name: printArray
	*    Print each element of the generic array on a new line. Do not return anything.
	*    @param A generic array
	**/
    func printArray ( array: [T]) {
        for i in 0...array.count-1 {
            print(array[i])
        }
    }
	
	// Write your code here
    
}
```

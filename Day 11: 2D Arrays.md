## Day 11: 2D Arrays
https://www.hackerrank.com/challenges/30-2d-arrays/problem

### Solution
```
import Foundation

var arr : [[Int]] = [[0,0,0,0,0,0],
					 [0,0,0,0,0,0],
					 [0,0,0,0,0,0],
					 [0,0,0,0,0,0],
					 [0,0,0,0,0,0],
					 [0,0,0,0,0,0]]

for i in 0...5 {
    arr[i] = readLine()!.components(separatedBy: " ").map{ Int($0)! }
}

var high = -999999

func check (_ x:Int,_ y:Int ) -> Int{
	var result = 0
	result += arr[x][y]
	result += arr[x][y+1]
	result += arr[x][y+2]
	result += arr[x+1][y+1]
	result += arr[x+2][y]
	result += arr[x+2][y+1]
	result += arr[x+2][y+2]
	return result
}

for i in 0...3 {
	for j in 0...3 {
		if check(i,j) >= high {
			high = check(i,j)
		}
	}
}

print(high)
```

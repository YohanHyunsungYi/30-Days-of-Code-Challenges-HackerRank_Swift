## Day 18: Queues and Stacks
https://www.hackerrank.com/challenges/30-queues-stacks/problem

## Solution
```
class Solution {
  //Write your code here
  
    var Stacks = [Character]()
    var Queues =  [Character]()
    var i = 0 , j = -1
	
    func pushCharacter(c: Character){
    	Stacks.append(c)
    }
    
    func enqueueCharacter(c: Character){
    	j += 1
		Queues.append(c)		
    }
    
    func popCharacter() -> Character {
		let result = Stacks[i]
		i += 1
		return result		
    }
    
    func dequeueCharacter() -> Character {
    	let result = Queues[j]
		j -= 1
		return result
    }
}
```

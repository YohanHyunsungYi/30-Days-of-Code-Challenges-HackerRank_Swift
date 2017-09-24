## Day 12: Inheritance
https://www.hackerrank.com/challenges/30-inheritance/problem

### Solution
```
class Student: Person {
    var testScores=0
	
    /*	
    *   Initializer
    *   
    *   Parameters:
    *   firstName - A string denoting the Person's first name.
    *   lastName - A string denoting the Person's last name.
    *   id - An integer denoting the Person's ID number.
    *   scores - An array of integers denoting the Person's test scores.
    */
    // Write your initializer here
    
    	init(firstName: String, lastName: String, identification: Int, scores: [Int]) {
		super.init(firstNameString: firstName, lastNameString: lastName, identificationNumber: identification)
        self.firstName = firstName
        self.lastName = lastName
        self.id = identification
        var AveagerScore = 0
        for i in scores{
            AveagerScore += i
        }
        testScores = AveagerScore / scores.count
    }

    /*	
    *   Method Name: calculate
    *   Return: A character denoting the grade.
    */
    // Write your method here
    func calculate() -> Character {
    	if (100 >= testScores && testScores >= 90){
            return("O")
        }else if (90 > testScores && testScores >= 80){
            return("E")
        }else if (80 > testScores && testScores >= 70){
            return("A")
        }else if (70 > testScores && testScores >= 55){
            return("P")
        }else if (55 > testScores && testScores >= 40){
            return("D")
        }else {
            return("T")
        }
    }
} // End of class Student
```

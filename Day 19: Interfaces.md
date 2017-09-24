## Day 19: Interfaces
https://www.hackerrank.com/challenges/30-interfaces/problem

### Solution - Java
```
class Calculator implements AdvancedArithmetic {
    public int divisorSum(int n) {
        int sum = n;
        for (int i = 1; i <= n/2; i++) {
            if (n % i == 0)
                sum += i;
        }
        return sum;
    }
}
```

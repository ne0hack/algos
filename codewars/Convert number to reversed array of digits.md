# Convert number to reversed array of digits


## Description
Given a random non-negative number, you have to return the digits of this number within an array in reverse order.

### Example(Input => Output):

```
35231 => [1,3,2,5,3]
0 => [0]
```


## Sample Tests
```python
import codewars_test as test
from solution import digitize

@test.describe("Fixed Tests")
def basic_tests():
    @test.it('Basic Test Cases')
    def basic_test_cases():
        test.assert_equals(digitize(35231),[1,3,2,5,3])
        test.assert_equals(digitize(0),[0])
        test.assert_equals(digitize(23582357),[7,5,3,2,8,5,3,2])
        test.assert_equals(digitize(984764738),[8,3,7,4,6,7,4,8,9])
        test.assert_equals(digitize(45762893920),[0,2,9,3,9,8,2,6,7,5,4])
        test.assert_equals(digitize(548702838394),[4,9,3,8,3,8,2,0,7,8,4,5])
```


## Solution
### Python3
```python
def digitize(n):
    return list(map(int, list(str(n))))[::-1]
```

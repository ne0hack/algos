# Convert a Number to a String!


## Description
We need a function that can transform a number (integer) into a string.

What ways of achieving this do you know?

#### Examples (input --> output):

```
123  --> "123"
999  --> "999"
-100 --> "-100"
```


## Sample Tests
```python
import codewars_test as test
from solution import number_to_string

@test.describe("Fixed Tests")
def basic_tests():
    @test.it('Basic Test Cases')
    def basic_test_cases():
        test.assert_equals(number_to_string(67), '67')
        test.assert_equals(number_to_string(79585), '79585')
        test.assert_equals(number_to_string(79585), "79585")
        test.assert_equals(number_to_string(1+2), '3')
        test.assert_equals(number_to_string(1-2), '-1')
```


## Solution
```python
def number_to_string(num):
    # Return a string of the number here!
    return str(num)
```

# Convert a String to a Number!


## Description
We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.

### Examples

```
"1234" --> 1234
"605"  --> 605
"1405" --> 1405
"-7" --> -7
```


## Sample Tests
```python
import codewars_test as test
from solution import string_to_number

@test.describe("string_to_number")
def basic_tests():
    @test.it('Basic Test Cases')
    def basic_test_cases():
        test.assert_equals(string_to_number("1234"), 1234)
        test.assert_equals(string_to_number("605"), 605)
        test.assert_equals(string_to_number("1405"), 1405)
        test.assert_equals(string_to_number("-7"), -7)
```


## Solutoin
### Python3
```python
def string_to_number(s):
    return int(s)
```

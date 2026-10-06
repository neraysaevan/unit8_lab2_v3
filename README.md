# Reflection – AI Number Program Lab

***PROFESSOR, MY COMMITS ARENT SHOWING UP ON GITHUB :(***

##  Student Name:
Maria Moskvichova

##  GitHub Repository Link:
[(Insert your repository URL here)](https://github.com/neraysaevan/unit8_lab2_v3)

## Iteration 1

What the AI code does:
- The `findResult` method calculates the sum of all the numbers in the array.
- It starts with a sum of 0.
- It loops through each value in the array and adds it to the sum.
- It then returns the total sum.

Tests passed/failed:
- `testBasicArray` - Failed. Expected 9, but the method returned 26.
- `testNegativeNumbers` - Failed. Expected -1, but the method returned -64.
- `testSingleValue` - Passed. The method returned 42 as expected.
- `testEmptyArray` - Failed. Expected `Integer.MIN_VALUE`, but the method returned 0.
- 1/4 tests passed

What surprised you:
- The tests appear to expect the largest number in the array rather than the sum. The sum implementation works correctly for calculating a total, but it does not match what the provided tests expect. The empty array returns 0 with this implementation because the initial value of `sum` is 0.

Commit message:
- Add NumberProgram class with findResult method for calculating array sum

---

## Iteration 2

What changed:
- Changed the `findResult` method from calculating the sum of the array to finding the largest integer.
- Added logic to compare each value with the current largest value.
- Added handling for an empty array by returning `Integer.MIN_VALUE`.

What improved:
- The method now matches the requirements of the provided JUnit tests.
- Negative numbers are handled correctly.
- Single-value arrays and empty arrays are handled correctly.

What still failed and why:
- Nothing failed. All four provided tests passed after updating the method.

Commit message:
- Iteration 2: largest value implementation

---

## Iteration 3

Final behavior:
- The `findResult` method returns the largest integer in the given array.
- It correctly handles positive and negative numbers.
- If the array is empty, it returns `Integer.MIN_VALUE`.

What was fixed:
- The original method calculated the sum of the array instead of finding the largest value.
- The method was changed to compare each value and keep track of the largest integer.
- An additional check was added for empty arrays so that `Integer.MIN_VALUE` is returned instead of causing an error.

What you learned:
- A method needs to match the expected behavior defined by the tests.
- Initializing the largest value with the first element allows the method to work correctly with negative numbers.
- Empty arrays need to be handled separately because they do not contain a first element.
- Unit tests are useful for identifying whether the implementation behaves as expected.

Commit message:
- Iteration 3: final version passing all tests

---

## Final Reflection

- How did AI responses change across prompts?
- How did testing affect your changes?
- What did version control help you understand?

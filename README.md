Our data sets have been getting bigger lately, and calculating some of these things in our head has become cumbersome. We need some help to process and analyze some data encoded as strings. Your task is to write a program that takes a string of numeric data representing measurements from a space probe and performs calculations on them.

Complete the `SpaceNumberCruncher` class to do the following:

- Create a method `convertToDoubleArray` that takes a comma-separated `String` of values, splits it at the commas, and returns the values as a `double` array.
  - If one of the comma-separated values cannot be converted to a number (for example, it contains letters or is empty), store `0.0` in that position instead — do **not** skip it. The returned array should always have one element for every comma-separated value in the input.
  - If the input string itself is empty (or contains only whitespace), return an array with zero elements.
- Create a method `calculateAverage` that takes the `double` array and returns the average of its values (total / number of elements), or `0.0` if the array has zero elements.
- Create a method `findHighest` that takes the `double` array and returns the highest value in it.
- Create a method `findLowest` that takes the `double` array and returns the lowest value in it.

In addition, implement the `main` method so that it does the following:

1. Prompts the user with exactly: `Enter space probe data (comma-separated numeric values): `
2. Reads the entered line as a `String`.
3. Converts it to a `double` array using `convertToDoubleArray`.
4. If the resulting array has zero elements, displays `Invalid input. Please provide numeric values.` and stops — do not attempt to calculate statistics.
5. Otherwise, calculates the average, highest, and lowest values using the methods above, then displays them.

Sample input:
```
123.5, 456.2, 789.9, 234.0, 567.8
```

Sample output:
```
Enter space probe data (comma-separated numeric values): Space Probe Data Statistics:
Average measurement: 434.28
Highest measurement: 789.9
Lowest measurement: 123.5
```

Requirements:
- Use `Scanner` to read the probe data entered by the user.
- Handle floating-point numeric values (e.g., decimal measurements) as well as whole numbers.
- Use a separate method for each calculation, as described above — don't do the math directly in `main`.
- Handle invalid entries (non-numeric values) gracefully, as described above, instead of crashing.
- Handle blank/empty input gracefully by displaying the invalid-input message described above.

Hint:
You can use `Double.parseDouble()` to convert each numeric string to a `double`. Wrap the conversion in a `try`/`catch` block so an invalid entry can be replaced with `0.0` instead of crashing the program.

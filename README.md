Our data sets have been getting bigger lately and calculating some of these things in our head has become cumbersome. We need some help to process and analyze some data encoded as strings. Your task is to write a program that takes a string of numeric data representing different measurements from a space probe and performs calculations on them.

Complete the `SpaceNumberCruncher` class to do the following:
- Create a method `calculateStatistics` that takes a string of numeric data as input. The string will contain numeric values separated by commas, representing measurements from the space probe.
- Create a method named `convertToDoubleArray` that takes the comma separated values, separates them at the commas, and returns them in a single double array.
- Create a method `calculateAverage` that takes all of the numbers in the double array created in `convertToDoubleArray`, and returns the average of those numbers.
- Create a method `findHighest` that returns the value of the highest number within the array.
- Create a method `findLowest` that returns the value of the lowest number within the array.

In addition, implement the main method that does the following:
Prompt the user to enter the space probe's data as a comma-separated string of numeric values.
Call the `calculateStatistics` method to compute the required statistics.
Display the average, highest, and lowest values with appropriate messages.

Sample input: `"123.5, 456.2, 789.9, 234.0, 567.8"`
Sample output:
```
Space Probe Data Statistics:
Average measurement: 434.28
Highest measurement: 789.9
Lowest measurement: 123.5
```

Requirements:
Handle floating-point numeric values (e.g., decimal measurements).
Use a method for calculating statistics, as mentioned above.
Handle invalid input gracefully, such as non-numeric values or improperly formatted input.
Ensure your program handles both integer and floating-point values correctly.
Make sure to gracefully exit the program at the end.

Hint:
You can use the Double.parseDouble() method to convert the numeric strings to double values for calculations.

{Submit|assessment}(test-3455788452)

# Running the project:
- Open the project in IntelliJ IDEA.
- Run the `CalculatorMain.java` class.
- Observe that the code runs without errors.

# I structured the code around three small interfaces in compliance with the ISP:
- BasicOperations: add, subtract, multiply, divide
- ScientificOperations: sqrt, log, sin, cos
- ProgrammingOperations: and, or, xor

# Three calculators implement these interfaces according to their specific needs:
- BasicCalculator: Implements BasicOperations; meaning it performs only the four basic operations.
- ScientificCalculator: Implements BasicOperations and ScientificOperations; meaning it performs square root, logarithm, sin, and cos in addition to basic operations.
- ProgrammingCalculator: Implements BasicOperations and ProgrammingOperations; meaning it performs AND, OR, and XOR in addition to basic operations.

# As a result:
- No class is forced to implement a method it does not use. CalculatorMain calls the specific operations for each calculator.

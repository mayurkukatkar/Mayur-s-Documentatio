# Operators in Java

An explanation of the different types of operators in Java.

## Goal
The goal of this section is to understand the various operators available in Java, including arithmetic, relational, logical, assignment, and bitwise operators. We will also cover operator precedence.

## Explanation
Operators are special symbols that perform operations on one, two, or three operands, and then return a result. The operators in Java can be classified into several types:

*   **Arithmetic Operators:** Used to perform common mathematical operations.
    *   `+` (Addition), `-` (Subtraction), `*` (Multiplication), `/` (Division), `%` (Modulus)
*   **Relational Operators:** Used to compare two values.
    *   `==` (Equal to), `!=` (Not equal to), `>` (Greater than), `<` (Less than), `>=` (Greater than or equal to), `<=` (Less than or equal to)
*   **Logical Operators:** Used to determine the logic between variables or values.
    *   `&&` (Logical AND), `||` (Logical OR), `!` (Logical NOT)
*   **Assignment Operators:** Used to assign values to variables.
    *   `=` (Assignment), `+=` (Add and assign), `-=` (Subtract and assign), `*=` (Multiply and assign), `/=` (Divide and assign), `%=` (Modulus and assign)
*   **Unary Operators:** Used with only one operand.
    *   `++` (Increment), `--` (Decrement), `!` (Logical complement), `+` (Unary plus), `-` (Unary minus)
*   **Bitwise Operators:** Used to perform bit-level operations.
    *   `&` (Bitwise AND), `|` (Bitwise OR), `^` (Bitwise XOR), `~` (Bitwise complement), `<<` (Left shift), `>>` (Right shift), `>>>` (Unsigned right shift)

### Operator Precedence
Operator precedence determines the order in which operators are evaluated in an expression. For example, multiplication and division have a higher precedence than addition and subtraction.

## Code
Here is an example that demonstrates the use of various operators in Java:

```java
public class OperatorsExample {
    public static void main(String[] args) {
        int a = 10;
        int b = 5;

        // Arithmetic operators
        System.out.println("a + b = " + (a + b));
        System.out.println("a - b = " + (a - b));
        System.out.println("a * b = " + (a * b));
        System.out.println("a / b = " + (a / b));
        System.out.println("a % b = " + (a % b));

        // Relational operators
        System.out.println("a == b is " + (a == b));
        System.out.println("a != b is " + (a != b));

        // Logical operators
        boolean x = true;
        boolean y = false;
        System.out.println("x && y is " + (x && y));
        System.out.println("x || y is " + (x || y));
        System.out.println("!x is " + !x);
    }
}
```

## Diagrams
```mermaid
graph TD
    subgraph Operators
        A[Arithmetic] --> B{+, -, *, /, %}
        C[Relational] --> D{==, !=, >, <, >=, <=}
        E[Logical] --> F{&&, ||, !}
        G[Assignment] --> H{=, +=, -=, *=, /=, %=}
        I[Unary] --> J{++, --, !, +, -}
        K[Bitwise] --> L{&, |, ^, ~, <<, >>, >>>}
    end
```

## Pitfalls
*   **Integer Division:** When dividing two integers, the result will be an integer, and the fractional part will be truncated. For example, `5 / 2` will result in `2`, not `2.5`.
*   **Short-Circuiting Logical Operators:** The `&&` and `||` operators are short-circuiting. This means that if the result of the expression can be determined from the first operand, the second operand will not be evaluated.
*   **Operator Precedence:** Not being aware of operator precedence can lead to unexpected results. It is often a good practice to use parentheses to make the order of evaluation explicit.

## Exercises/Examples
1.  **Write a program that takes a number as input and checks if it is even or odd.**
    <details>
    <summary>Answer</summary>

    ```java
    import java.util.Scanner;

    public class EvenOdd {
        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
            System.out.print("Enter a number: ");
            int num = scanner.nextInt();

            if (num % 2 == 0) {
                System.out.println(num + " is even.");
            } else {
                System.out.println(num + " is odd.");
            }
        }
    }
    ```
    </details>
2.  **What is the difference between `==` and the `.equals()` method for comparing strings?**
    <details>
    <summary>Answer</summary>
    The `==` operator compares the memory addresses of two string objects, while the `.equals()` method compares the actual content of the strings.
    </details>
3.  **What is the result of the expression `5 + 15 / 3 * 2 - 8 % 3`?**
    <details>
    <summary>Answer</summary>
    The result is `13`. The order of operations is: division, multiplication, modulus, addition, and subtraction.
    </details>

## References
*   [Oracle Operators](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/operators.html)
*   [W3Schools Java Operators](https://www.w3schools.com/java/java_operators.asp)
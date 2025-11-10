# Introduction to Java

A high-level overview of what Java is, its history, and its core principles.

## Goal
The goal of this section is to introduce the Java programming language, its key features, and why it remains one of the most popular and widely-used languages in the world.

## Explanation
Java is a high-level, object-oriented, and platform-independent programming language developed by Sun Microsystems (now owned by Oracle). It was first released in 1995 and has since become a cornerstone of modern software development.

### Key Features of Java:
*   **Platform Independent:** Java code is compiled into an intermediate format called bytecode, which can run on any machine with a Java Virtual Machine (JVM). This "write once, run anywhere" philosophy is a key advantage.
*   **Object-Oriented:** Java is built around the concept of objects, which bundle data and behavior together. This makes it easier to model real-world entities and build modular, reusable code.
*   **Statically Typed:** Variables must be declared with a specific type before they are used. This helps catch errors early in the development process.
*   **Automatic Memory Management:** Java's garbage collector automatically reclaims memory that is no longer in use, freeing developers from manual memory management.
*   **Rich Standard Library:** Java provides a vast collection of pre-built classes and methods for common tasks, from I/O and networking to data structures and GUI development.

## Code
Here is a simple "Hello, World!" program in Java:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

### How to Compile and Run:
1.  Save the code in a file named `HelloWorld.java`.
2.  Open a terminal and compile the code using the Java compiler:
    ```bash
    javac HelloWorld.java
    ```
3.  Run the compiled bytecode using the Java interpreter:
    ```bash
    java HelloWorld
    ```

## Diagrams
```mermaid
graph TD
    A[Java Source Code (.java)] -->|Compiler (javac)| B(Bytecode (.class));
    B --> C{JVM};
    C --> D[Windows];
    C --> E[macOS];
    C --> F[Linux];
```

## Pitfalls
*   **Verbosity:** Java can be more verbose than some other languages, requiring more boilerplate code for simple tasks.
*   **Performance:** While modern JVMs are highly optimized, Java can sometimes be slower than natively compiled languages like C++.
*   **Setup:** Setting up the Java Development Kit (JDK) and understanding the classpath can be a hurdle for beginners.

## Exercises/Examples
1.  **Modify the "Hello, World!" program to print your name.**
    <details>
    <summary>Answer</summary>

    ```java
    public class HelloWorld {
        public static void main(String[] args) {
            System.out.println("Hello, [Your Name]!");
        }
    }
    ```
    </details>
2.  **Write a program that prints the numbers from 1 to 5.**
    <details>
    <summary>Answer</summary>

    ```java
    public class PrintNumbers {
        public static void main(String[] args) {
            for (int i = 1; i <= 5; i++) {
                System.out.println(i);
            }
        }
    }
    ```
    </details>
3.  **What is the purpose of the `main` method in a Java program?**
    <details>
    <summary>Answer</summary>
    The `main` method is the entry point of a Java application. When you run a Java program, the JVM looks for the `main` method and starts execution from there.
    </details>

## References
*   [Oracle Java Documentation](https://docs.oracle.com/en/java/)
*   [W3Schools Java Tutorial](https://www.w3schools.com/java/)
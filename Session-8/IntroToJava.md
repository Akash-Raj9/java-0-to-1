# Session 8: Introduction to Java

## Overview
In this session, we will introduce the fundamental concepts of Java, including its syntax, structure, and the components required to run Java programs. You will learn about the **JDK**, **JVM**, **JRE**, how to write your first Java program, and how to run it from the command line.

---

## What is Java?
Java is a widely-used, high-level programming language that follows the Object-Oriented Programming (OOP) paradigm. Java is platform-independent, meaning that it can run on any device with a Java Virtual Machine (JVM). Java is used for web development, mobile apps, enterprise applications, and much more.

---

## JDK, JVM, and JRE

Before we get started with Java programming, let's understand some important components:
- **JDK (Java Development Kit):** The JDK is a software development kit used to develop Java applications. It includes tools like the Java compiler (`javac`), Java runtime libraries, and the JRE.
- **JRE (Java Runtime Environment):** The JRE contains the necessary components to run Java applications. It includes the JVM and libraries but does not contain the tools needed for developing Java programs.
- **JVM (Java Virtual Machine):** The JVM is responsible for running Java programs. It converts Java bytecode into machine code that can be executed on the specific hardware platform.

---

## Installing Java (JDK)

To start coding in Java, you'll need to install the **Java Development Kit (JDK)**. You can download the JDK from the official Oracle website:

[Download JDK 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

Alternatively, if you're using Linux, you can install the JDK via the terminal with the following command:

For **Ubuntu**:
```bash
sudo apt update
sudo apt install openjdk-17-jdk
```

For **Fedora**:
```bash
sudo dnf install java-17-openjdk-devel
```

Once installed, check if Java is installed correctly by typing the following command in the terminal:

```bash
java --version
```

This should display the installed version of Java.

---

## Writing Your First Java Program

1. **Creating the Java File:**
   Open a text editor (like Notepad, VSCode, or any IDE) and create a new file. Name the file `HelloWorld.java`. The name of the file **must** match the name of the class in the program.

2. **HelloWorld.java Code Example:**

   Here's a simple Java program that prints `Hello, World!` to the console:

   ```java
   // HelloWorld.java

   public class HelloWorld {
       public static void main(String[] args) {
           System.out.println("Hello, World!");
       }
   }
   ```

3. **Explanation of the Code:**
   - `public class HelloWorld`: This defines the class named `HelloWorld`. In Java, all code must be inside a class.
   - `public static void main(String[] args)`: This is the entry point of the Java program. The `main` method is where the program starts running. 
     - `public`: It indicates that the method is accessible by anyone.
     - `static`: It means the method can be called without creating an instance of the class.
     - `void`: It means the method does not return any value.
     - `String[] args`: This allows the program to accept command-line arguments.
   - `System.out.println("Hello, World!");`: This prints the text `"Hello, World!"` to the console.

4. **Running the Java Program from the Command Line:**

   To run the program, follow these steps:
   - Open your terminal or command prompt.
   - Navigate to the directory where your `HelloWorld.java` file is saved.
   - First, compile the program using the `javac` command:
     ```bash
     javac HelloWorld.java
     ```
     This will generate a `HelloWorld.class` file (the bytecode).
   
   - Now, run the program using the `java` command:
     ```bash
     java HelloWorld
     ```
     This should output:
     ```
     Hello, World!
     ```

---

## Common Errors

- **If the `main` method is changed to something else like `Ayush`:**
   If you rename the `main` method, like this:
   ```java
   public class HelloWorld {
       public static void Ayush(String[] args) {
           System.out.println("Hello, World!");
       }
   }
   ```
   When you try to run the program, you'll get the following error:
   ```
   Error: Main method not found in class HelloWorld, please define the main method as:
   public static void main(String[] args)
   ```

---

## Structure of Java Code

Java code must be organized in a specific way:
- **Class:** All Java code must be inside a class. A class defines the blueprint for creating objects.
- **Main Method:** The `main` method is the entry point of any Java application.
- **Syntax:** Java follows strict syntax rules. For example, every statement must end with a semicolon (`;`), and code blocks are enclosed in curly braces (`{}`).

In future sessions, you will learn more about **classes** and **objects** in depth.

---

## **HelloWorld.java Program:**
[Download HelloWorld.java](https://github.com/rothardo/java-0-to-1/blob/master/Session-8/HelloWorld.java)


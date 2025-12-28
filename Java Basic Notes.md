# Java Notes ☕📘

These notes are written for **freshers and beginners** who are learning Java and preparing for interviews.  
The focus is on **clear concepts, simple explanations, and quick revision**.

---

## 1. Introduction to Java

Java is a **high-level, object-oriented programming language** developed by **James Gosling** at **Sun Microsystems** (now owned by Oracle).

Java follows the principle **"Write Once, Run Anywhere" (WORA)**.  
This is possible because Java programs run on the **Java Virtual Machine (JVM)**.

### Features of Java
- Platform Independent  
- Object-Oriented  
- Robust and Secure  
- Multithreaded  
- Automatic Memory Management (Garbage Collection)

---

## 2. Java Program Structure

Every Java program must have:
- A **class**
- A **main() method** (entry point)
- Statements inside the main method

### Basic Java Program
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```
~Explanation

      class HelloWorld → Defines a class

      main() → Program execution starts here

      System.out.println() → Prints output to console
---


## 3. Data Types in Java

Java data types are divided into two categories.
 ### 1.) Primitive Data Types
```
| Data Type | Size    | Description         |
| --------- | ------- | ------------------- |
| byte      | 1 byte  | Small integer       |
| short     | 2 bytes | Integer             |
| int       | 4 bytes | Integer             |
| long      | 8 bytes | Large integer       |
| float     | 4 bytes | Decimal (7 digits)  |
| double    | 8 bytes | Decimal (15 digits) |
| char      | 2 bytes | Single character    |
| boolean   | 1 bit   | true / false        |
```
### Examples
  ```
   public class DataTypesExample {
    public static void main(String[] args) {
        int age = 25;
        double price = 99.99;
        char grade = 'A';
        boolean isJavaFun = true;

        System.out.println(age);
        System.out.println(price);
        System.out.println(grade);
        System.out.println(isJavaFun);
    }
}
```
---
## 4. Operators in Java
 Types of Operators

   . Arithmetic:( + - * / % )

   . Relational:( == != > < >= <= )

   . Logical:( && || ! )

   . Assignment:( = += -= *= )

   . Increment / Decrement:( ++ -- )
 ### Example
    public class OperatorsExample {
    public static void main(String[] args) {
        int a = 10, b = 5;
        System.out.println(a + b);
        System.out.println(a > 5 && b < 10);
    }
    }

---
## 5. Control Statements
   ### 1. If-Else Statement
      int number = 10;
      if (number > 0) {
         System.out.println("Positive Number");
      } 
      else {
         System.out.println("Negative Number");
      }
  
   ### 2. Switch Case
    int day = 3;
    switch (day) {
       case 1: System.out.println("Monday"); break;
       case 2: System.out.println("Tuesday"); break;
       default: System.out.println("Other Day");
    }
    
  ### 3. Loops
   #### a.) For Loop
    for (int i = 1; i <= 5; i++) {
        System.out.println(i);
    }
   #### b.) While Loop
     int i = 1;
     while (i <= 5) {
       System.out.println(i);
       i++;
     }

---
## 6. Arrays in Java
Arrays are used to store multiple values of the same data type.

    public class ArrayExample {
       public static void main(String[] args) {
        int[] numbers = {10, 20, 30, 40};

        for (int i = 0; i < numbers.length; i++) {
            System.out.println(numbers[i]);
         }
       }
     }
---
## 7. Object-Oriented Programming (OOP)
Java follows four main OOP principles:

   1. Encapsulation – Data hiding

   2. Inheritance – Reusing parent class properties

   3. Polymorphism – Same method, different behavior

   4. Abstraction – Hiding implementation details

### Class and Object Example
    class Car {
        String brand;
        int speed;

       void show() {
        System.out.println("Brand: " + brand + ", Speed: " + speed);
       }
    }

    public class Main {
        public static void main(String[] args) {
           Car myCar = new Car();
           myCar.brand = "Tesla";
           myCar.speed = 200;
           myCar.show();
       }
    }
   
### Inheritance Example
    class Animal {
       void makeSound() {
          System.out.println("Animal makes a sound");
       }
    }

    class Dog extends Animal {
         void bark() {
            System.out.println("Dog barks");
         }
    }  

    public class InheritanceExample {
         public static void main(String[] args) {
            Dog d = new Dog();
           d.makeSound();
           d.bark();
        }
    }
---


      


    


      


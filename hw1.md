**HW#1 - Java OOP and Core Concepts**

### 1 - Why do we need to use OOP? Some major OOP languages?
**Answer:** OOP (Object-Oriented Programming) provides modularity, reusability, scalability, and maintainability in software development. It organizes code into objects that encapsulate data and behaviors.

**Major OOP Languages:** Java, C++, Python, C#, Ruby.

---
### 2 - Interface vs Abstract Class?
**Answer:**
- **Interface:** Defines a contract that implementing classes must follow. It only contains method signatures (default methods in Java 8+ are an exception).
- **Abstract Class:** Can have both abstract and concrete methods. It provides partial implementation that subclasses can extend.

**When to Use?**
- Use interfaces when multiple classes share the same behavior but do not share implementation.
- Use abstract classes when classes share both behavior and some implementation.

---
### 3 - Why do we need equals and hashCode? When to override?
**Answer:**
- `equals()` is used to compare object content instead of memory reference.
- `hashCode()` ensures that objects with the same content have the same hash value for efficient hashing (e.g., HashMap, HashSet).

**Override them when:**
- Custom classes need logical equality comparison.
- Objects are used as keys in hash-based collections.

---
### 4 - Diamond Problem in Java? How to fix it?
**Answer:**
- The **Diamond Problem** occurs when a class inherits from two interfaces that define the same default method.
- **Fix:** Override the method in the child class or specify which interface’s method to use (`Interface.super.methodName();`).

---
### 5 - Why do we need a Garbage Collector? How does it run?
**Answer:**
- **Garbage Collector (GC)** automatically manages memory by reclaiming unused objects.
- Runs as part of the JVM in multiple algorithms (e.g., Mark-and-Sweep, G1GC).

---
### 6 - Java `static` keyword usage?
**Answer:**
- **Static variables:** Shared across all instances of a class.
- **Static methods:** Can be called without an instance.
- **Static blocks:** Used for one-time initialization.
- **Static nested classes:** Can exist independently of an instance.

---
### 7 - Immutability means? Where, how, and why to use it?
**Answer:**
- **Immutable objects:** Cannot be modified after creation (e.g., `String`, `Integer`).
- **Where & Why?** Used in multi-threading and caching to prevent unintended modifications.
- **How?**
  - Declare fields as `private final`.
  - Remove setters.
  - Return copies instead of references.

---
### 8 - Composition and Aggregation: Meaning and Differences?
**Answer:**
- **Composition:** Strong relationship; child cannot exist without parent (e.g., Engine in a Car).
- **Aggregation:** Weak relationship; child can exist independently (e.g., Student and College).

---
### 9 - Cohesion and Coupling: Meaning and Differences?
**Answer:**
- **Cohesion:** How closely related a class’s responsibilities are. Higher is better.
- **Coupling:** Dependency between classes. Lower is better for maintainability.

---
### 10 - Heap and Stack: Meaning and Differences?
**Answer:**
- **Heap:** Stores objects and dynamically allocated memory.
- **Stack:** Stores method call stack, local variables, and method execution context.

---
### 11 - Exception means? Types of Exceptions?
**Answer:**
- **Exception:** An event that disrupts normal execution.
- **Types:**
  - **Checked Exceptions:** Must be handled (e.g., `IOException`).
  - **Unchecked Exceptions:** Runtime errors (e.g., `NullPointerException`).

---
### 12 - How to summarize ‘clean code’ as short as possible?
**Answer:**
- **Readable:** Use meaningful names, keep functions short.
- **Simple:** Follow SRP (Single Responsibility Principle).
- **Maintainable:** Write modular and well-structured code.
- **Efficient:** Avoid unnecessary computations.

---
### 13 - What is the method of hiding in Java?
**Answer:**
- **Method Hiding:** When a `static` method in a child class has the same signature as a `static` method in a parent class, but does not override it. Instead, it hides the parent’s method.

---
### 14 - Difference between Abstraction and Polymorphism in Java?
**Answer:**
- **Abstraction:** Hides implementation details (e.g., abstract classes, interfaces).
- **Polymorphism:** Allows different behaviors based on object type (e.g., method overloading & overriding).

---

This document provides clear, structured, and concise answers to the homework questions. Let me know if you need any refinements!


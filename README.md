## 🚀 Java OOP Mini-Project: **Library Management System**

### 📘 Objective:
Build a simple `LibraryBook` system that tracks books in a library using **OOP principles in Java**, with a focus on:
- Constructor types (no-arg, parameterized)
- Constructor overloading
- Static variables and methods
- Static factory methods

---

### 📝 Problem Statement:
You are tasked with creating a Java class that models a book in a library. Every book should have:
- A **title**
- An **author**
- A **unique ID number**
- A **status** (e.g., *available*, *checked out*)

Your job is to build this with clean, readable, maintainable code using everything you’ve learned today.

---

### ✅ Requirements:

#### 1. `LibraryBook` class:
- **Private Fields**:
  - `String title`
  - `String author`
  - `String bookId` *(unique for each book)*
  - `String status` *(defaults to “available”)*
- **Static Fields**:
  - `int totalBooks` *(tracks how many books have been created)*
- **Static Methods**:
  - `generateBookId()` → returns a unique book ID like `BOOK1001`, `BOOK1002`...
  - `getTotalBooks()` → returns current number of books created

---

#### 2. Constructors:
- **No-arg constructor** → sets title and author to `"Unknown"`, status to `"available"`
- **Constructor with title and author**
- **Constructor with title, author, and status**
> Use constructor overloading to implement this.

---

#### 3. Static Factory Method:
```java
public static LibraryBook createAvailable(String title, String author)
```
- Creates a book with status set to "available" (even if constructor takes custom ones).

---

#### 4. Utility Method:
- `public String toString()` → display book details nicely.

---

### 🔍 Sample Output:
```java
LibraryBook book1 = new LibraryBook();
LibraryBook book2 = LibraryBook.createAvailable("1984", "George Orwell");

System.out.println(book1);
System.out.println(book2);
System.out.println("Total Books: " + LibraryBook.getTotalBooks());
```

---

### 💡 Bonus:
- Add a static `List<LibraryBook>` to simulate the library’s collection.
- Add a static method to print all books in the collection.

---

### 📦 Deliverables:
1. Java class: `LibraryBook.java`
2. A `main()` method in a test class `LibraryTest.java` demonstrating object creation and functionality.
3. Code must follow good naming, formatting, and best practices (comments, spacing, etc.)
4. Include a `README.md` describing:
   - What your program does
   - How to run it
   - What Java features you used

---

### 🧑‍🏫 Instructions:
1. Fork this repository into your personal GitHub account.
2. Clone the repo locally.
3. Add your solution.
4. Commit and push your code to your GitHub repo.
5. Submit the GitHub repo link via GitHub Classroom.

---

### 📚 Concepts Covered:
- Constructors
- Constructor overloading
- Static variables & methods
- Static factory methods
- Clean coding

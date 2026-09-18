## Aryan GUPTA (25BAI11516)

# Campus Course & Records Manager (CCRM)

welcome to CCRM - basically a campus management system that I made for my project. Its not just another boring console application that no one wants to use. This is a Java project that actually makes managing students, courses, and enrollments pretty decent to work with.

## what Makes This Special?

Think of CCRM as like your digital campus assistant or something. Whether your tracking student enrollments, managing course catalogs, or just need to backup your data, this thing can handle it. I built it using object-oriented principles that I learned in class, so its not just working - its actually maintainable and stuff.

if you want to add database integration later? no problem! The architecture I implemented makes future enhancements easy to add.

## How Its Organized

```
CCRM-Java-Project/
 ├─ edu/ccrm/
 │   ├─ cli/           ← main menu stuff (MainMenu.java)
 │   ├─ config/        ← App settings and configuration
 │   ├─ domain/        ← important classes (Student, Course, etc.)
 │   ├─ service/       ← where the business logic happens
 │   └─ util/          ← utility classes and helpers
 ├─ screenshots/       ← screenshots to show it works
 └─ README.md         ← this file
```

## Getting Started

**What You Need:**
- Java 17 or newer (prof said to use this version)
- VS Code with Java Extension Pack or Eclipse IDE
- around 5-10 minutes
<img width="1596" height="650" alt="downloading java" src="https://github.com/user-attachments/assets/33b20a3d-bd8c-48a0-b5d5-571835a03300" />

**How to run:**
1. open VS Code and load the `CCRM-Java-Project` folder
2. go to `edu/ccrm/cli/MainMenu.java`
3. click run and it should start working

the menu is pretty intuitive so you can figure it out easily.

## Java History (quick overview)

Heres how Java evolved over time:
- **1995**: Java 1.0 was released (Sun Microsystems made it)
- **2004**: Java 5 added Generics and Enums (these are really useful)
- **2014**: Java 8 brought Streams and Lambdas (functional programming stuff)
- **2017**: Oracle started releasing new versions every 6 months
- **now**: We're using Java 17+ because it has Long Term Support

## Java Editions - which one to use

| what you want to build | which Java Edition |
|------------------------|-------------------|
| Desktop apps, console programs | **Java SE** (this is what we used) |
| Web applications, enterprise stuff | **Java EE/Jakarta EE** |
| Mobile apps, embedded systems | **Java ME** |

## JVM, JRE, JDK explained

- **JVM**: runs the bytecode 
- **JRE**: JVM + libraries needed to run programs
- **JDK**: everything - JRE + compiler + development tools

basically JDK contains JRE, and JRE contains JVM.

## Windows setup (quick guide)

1. download JDK from [Oracle website](https://www.oracle.com/java/technologies/javase-downloads.html)
2. install it and setup `JAVA_HOME` environment variable
3. test if its working:
   ```bash
   java -version
   javac -version
   ```
![java version](https://github.com/user-attachments/assets/7e7d0f3a-4650-426f-8c4a-de99b31cc124)

if you see version numbers then your good to go.

## Learning concepts we used

This project demonstrates various OOP concepts that we learned in our course:

| **concept** | **where to find it** | **why its important** |
|-------------|----------------------|---------------------|
| **Encapsulation** | `Student.java` with private fields | keeps data secure |
| **Inheritance** | `Person → Student, Instructor` | reuse code efficiently |
| **Abstraction** | `Person.java` abstract class | clean interfaces |
| **Polymorphism** | `printProfile()` method variations | same method, different behavior |
| **Immutable Classes** | `CourseCode.java` | thread-safe objects |
| **Nested Classes** | `Course.Builder` | better organization |
| **Enums** | `Grade.java`, `Semester.java` | type-safe constants |
| **Lambda expressions** | used throughout the project | makes code more readable |
| **Design Patterns** | Singleton, Builder patterns | industry standards |
| **File Operations** | `FileUtil.java` with NIO.2 | modern file handling |
| **Date/Time API** | Student admission dates | better than old Date class |

## Screenshots included

I added screenshots to show that everything actually works:
- Java version check
- VS Code project structure 
- CLI running 
- Backup functionality working

## for Eclipse users

if you prefer Eclipse IDE:
1. **File → New → Java Project**
2. name it `CCRM-Java-Project`
3. copy source files into `edu/ccrm/` package structure
4. run `MainMenu.java` 
<img width="1091" height="544" alt="Eclipse setup" src="https://github.com/user-attachments/assets/f6758ac1-46c7-4056-8126-9ae414213a23" />
<img width="638" height="679" alt="eclipse install" src="https://github.com/user-attachments/assets/becaaee9-3832-49e6-b9c7-1632797ee4a5" />

**enabling assertions** (optional but recommended)
```java
// in your code:
assert credits > 0 : "Credits must be positive";
```

run with assertions:
```bash
java -ea edu.ccrm.cli.MainMenu
```

**compile everything:**
```bash
# compile all Java files properly
javac -d . $(find edu -name "*.java")

# run the program
java edu.ccrm.cli.MainMenu
```

## future improvements

this is just the beginning! the design makes it easy to add:
- Database connectivity (JDBC integration)
- web interface
- REST API 
- better reporting features
- whatever else we think of later

the modular structure means I can keep adding features without breaking existing code.

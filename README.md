# POLYSOLVE

### Polynomial & Calculus Calculator

POLYSOLVE is a Java Swing desktop application for performing polynomial algebra and calculus operations through an intuitive graphical user interface. The application is designed using the **Model-View-Controller (MVC)** architecture to maintain a clean separation between mathematical logic, user interface, and application control.

## ✨ Features

### Algebra Operations
- Addition of two polynomials
- Subtraction of two polynomials
- Multiplication of two polynomials

### Calculus Operations
- Evaluate a polynomial for a given value of `x`
- Differentiate a polynomial
- Calculate indefinite integrals
- Calculate definite integrals over a specified interval

### Input Support
POLYSOLVE supports multiple polynomial input formats:

```text
3x^2 + 2x + 1
x^3 - x
3,2,1

---
```
The comma-separated format represents coefficients from the highest degree to the constant term.

User Experience
Clean Java Swing graphical interface
Separate Algebra and Calculus sections
Input validation and user-friendly error messages
Modular MVC-based architecture
Reusable mathematical model classes

## Architecture (MVC)

```
                         POLYSOLVE
                             │
             ┌───────────────┼───────────────┐
             │               │               │
           Model          Controller         View
             │               │               │
       Polynomial.java       │          MainFrame.java
       PolynomialParser.java │          AlgebraPanel.java
                             │          CalculusPanel.java
                             │          Theme.java
                             │
                     PolySolveController
```
## Model

Responsible for polynomial representation and mathematical operations.
```
model/
├── Polynomial.java
└── PolynomialParser.java
```
Polynomial.java handles polynomial operations such as addition, subtraction, multiplication, evaluation, differentiation, and integration.
PolynomialParser.java converts user-entered polynomial expressions into polynomial objects.
### View
Responsible for the graphical user interface.
```
view/
├── MainFrame.java
├── AlgebraPanel.java
├── CalculusPanel.java
└── Theme.java
```
### Controller
Connects the user interface with the mathematical model.
```
controller/
└── PolySolveController.java
```
The controller processes user actions and coordinates communication between the Model and View layers.
### 🛠️ Tech Stack
```
| Technology           | Purpose                                          |
| -------------------- | ------------------------------------------------ |
| **Java**             | Core application development                     |
| **Java Swing**       | Desktop graphical user interface                 |
| **Maven**            | Build and dependency management                  |
| **MVC Architecture** | Application structure and separation of concerns |
| **Git & GitHub**     | Version control and project hosting              |
```
### 📂 Project Structure
```
POLYSOLVEEE/
│
├── docs/
│   ├── Project_Report.docx
│   └── UML_Class_Diagram.png
│
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── polysolve/
│                   ├── Main.java
│                   │
│                   ├── controller/
│                   │   └── PolySolveController.java
│                   │
│                   ├── model/
│                   │   ├── Polynomial.java
│                   │   └── PolynomialParser.java
│                   │
│                   └── view/
│                       ├── AlgebraPanel.java
│                       ├── CalculusPanel.java
│                       ├── MainFrame.java
│                       └── Theme.java
│
├── .gitignore
├── pom.xml
└── README.md
```
### 🚀 Getting Started
### Prerequisites
Make sure the following are installed:

Java JDK
Apache Maven
Git

Verify Java:
```
java -version
```
Verify Maven:
```
mvn -version
```
Clone the Repository
```
git clone https://github.com/angelgali13/POLYSOLVEEE.git
```
Navigate into the project:
```
cd POLYSOLVEEE
```

Build the Project
```
mvn clean install
```
Run the Application
```
mvn exec:java -Dexec.mainClass="com.polysolve.Main"
```

The POLYSOLVE desktop application will launch.


### 🧮 Example Operations
Polynomial Addition
```
Polynomial A: 3x² + 2x + 1
Polynomial B: 2x² + x + 4

Result: 5x² + 3x + 5
```
Differentiation
```
Input: 3x² + 2x + 1

Derivative: 6x + 2
```
Integration
```
Input: 3x² + 2x + 1

Integral: x³ + x² + x + C
```
Evaluation
```
Input: 3x² + 2x + 1
x = 2

Result: 17
```
### 🎯 Project Objectives
Implement polynomial algebra operations programmatically
Implement fundamental calculus operations
Build an interactive desktop application using Java Swing
Apply MVC architecture in a real-world software project
Practice object-oriented programming and modular software design
Separate mathematical logic from presentation and user interaction
### 💡 Key Concepts Demonstrated
Object-Oriented Programming,

MVC Design Pattern,

Java Swing GUI Development,

Polynomial Data Structures,

Expression Parsing,

Mathematical Computation,

Event-Driven Programming,

Modular Software Design,

Input Validation,

Maven Project Management,

Git Version Control.

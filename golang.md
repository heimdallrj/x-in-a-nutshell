# Go Programming

## Overview
<todo>

## Audience
Students new to the language who have experience with other programming languages.

## Prerequisites
This course is specially designed for individuals with prior programming background. Also it assumes a working knowledge of basic Object Oriented Programming concepts. If you have no prior programming experience or or not familiar with Object Oriented Programming, you should consider our "Programming Basics for Non-Programmers with Python" course.

## Course Outline
### 1: Variables and Operators
- Introduction 
- What Does Go Look Like?
- Exercise 1.01: Using Variables, Packages, and Functions to Print Stars
- Activity 1.01 Defining and Printing
- Declaring Variables 
- Declaring a Variable Using var
Exercise 1.02: Declaring a Variable Using var
Declaring Multiple Variables at Once with var
Exercise 1.03: Declaring Multiple Variables at Once with var
Skipping the Type or Value When Declaring Variables
Exercise 1.04: Skipping the Type or Value When Declaring Variables
Type Inference Gone Wrong
Short Variable Declaration
Exercise 1.05: Implementing Short Variable Declaration
Declaring Multiple Variables with a Short Variable Declaration
Exercise 1.06: Declaring Multiple Variables from a Function
Using var to Declare Multiple Variables in One Line
Non-English Variable Names
Changing the Value of a Variable
Exercise 1.07: Changing the Value of a Variable
Changing Multiple Values at Once
Exercise 1.08: Changing Multiple Values at Once
Operators
Exercise 1.09 Using Operators with Numbers
Shorthand Operator
Exercise 1.10: Implementing Shorthand Operators
Comparing Values
Exercise 1.11: Comparing Values
Zero Values
Exercise 1.12 Zero Values
Value versus Pointer
Getting a Pointer
Exercise 1.13: Getting a Pointer 
Getting a Value from a Pointer
Exercise 1.14: Getting a Value from a Pointer
Function Design with Pointers
Exercise 1.15: Function Design with Pointers
Activity 1.02: Pointer Value Swap
Constants
Exercise 1.16: Constants
Enums
Scope
Activity 1.03: Message Bug
Activity 1.04: Bad Count Bug
Summary

### 2: Logic and Loops
Introduction
if Statements
Exercise 2.01: A Simple if Statement
if else Statements
Exercise 2.02: Using an if else Statement
else if Statements
Exercise 2.03: Using an else if Statement
The Initial if Statement
Exercise 2.04: Implementing the Initial if Statements
Activity 2.01: Implementing FizzBuzz
Expression switch Statements
Exercise 2.05: Using a switch Statement
Exercise 2.06: switch Statements and Multiple case Values
Exercise 2.07: Expressionless switch Statements
Loops
Exercise 2.08: Using the for i Loop
Exercise 2.09: Looping Over Arrays and Slices
The range Loop
Exercise 2.10: Looping Over a Map
Activity 2.02: Looping Over Map Data Using range
break and continue
Exercise 2.11: Using break and continue to Control Loops
Activity 2.03: Bubble Sort
Summary

### 3: Core Types
Introduction 
True and False 
Exercise 3.01: Program to Measure Password Complexity
Numbers
Integer
Floating Point 
Exercise 3.02: Floating-Point Number Accuracy
Overflow and Wraparound
Exercise 3.03: Triggering Number Wraparound
Big Numbers
Exercise 3.04: Big Numbers
Byte
Text
Rune
Exercise 3.05: Safely Looping over a String
The nil Value
Activity 3.01: Sales Tax Calculator
Activity 3.02: Loan Calculator
Summary

### 4: Complex Types
Introduction
Collection Types
#### Arrays
Exercise 4.01: Defining an Array
Comparing Arrays
Exercise 4.02: Comparing Arrays
Initializing Arrays Using Keys
Exercise 4.03: Initializing an Array Using Keys
Reading from an Array
Exercise 4.04: Reading a Single Item from an Array
Writing to an Array
Exercise 4.05: Writing to an Array
Looping an Array
Exercise 4.06: Looping Over an Array Using a "for i" Loop
Modifying the Contents of an Array in a Loop
Exercise 4.07: Modifying the Contents of an Array in a Loop
Activity 4.01: Filling an Array
#### Slice
Exercise 4.08: Working with Slices 
Activity 4.02: Printing a User's Name Based on User Input
Appending Multiple Items to a Slice
Exercise 4.09: Appending Multiple Items to a Slice
Activity 4.03: Creating a Locale Checker
Creating Slices from Slices and Arrays
Exercise 4.10: Creating Slices from a Slice
Understanding Slice Internals 
Exercise 4.11: Using make to Control the Capacity of a Slice
Background Behavior of Slices 
Exercise 4.12: Controlling Internal Slice Behavior
#### Map Fundamentals
Exercise 4.13: Creating, Reading, and Writing a Map
Reading from Maps
Exercise 4.14: Reading from a Map
Activity 4.04: Slicing the Week
Deleting Elements from a Map
Exercise 4.15: Deleting an Element from a Map
Activity 4.05: Removing an Element from a Slice
#### Simple Custom Types 
Exercise 4.16: Creating a Simple Custom Type
#### Structs
Exercise 4.17: Creating Struct Types and Values
Comparing Structs to Each Other
Exercise 4.18: Comparing Structs to Each Other
Struct Composition Using Embedding
Exercise 4.19: Struct Embedding and Initialization
Type Conversions
Exercise 4.20: Numeric Type Conversion
Type Assertions and interface{}
Exercise 4.21: Type Assertion 
Type Switch
Exercise 4.22: Type Switch
Activity 4.06: Type Checker
Summary

### 5: Functions
Introduction 
Functions 
Parts of a function 
fizzBuzz
Exercise 5.01: Creating a Function to Print Salesperson
Expectation Ratings from the Number of Items Sold
Parameters
The Difference between an Argument and a Parameter
Exercise 5.02: Mapping Index Values to Column Headers
Function Variable Scope
Return Values
Exercise 5.03: Creating a fizzBuzz Function with Return Values
Activity 5.01: Calculating the Working Hours of Employees
Naked Returns
Exercise 5.04: Mapping a CSV Index to a Column Header
with Return Values
Variadic Function
Exercise 5.05: Summing Numbers
Anonymous Functions 
Exercise 5.06: Creating an Anonymous Function to Calculate
the Square Root of a Number
Closures
Exercise 5.07: Creating a Closure Function to Decrement a Counter
Function Types 
Exercise 5.08: Creating Various Functions to Calculate Salary
defer
Activity 5.02: Calculating Payable Amount for Employees
Based on Working Hours 
Summary

### 6: Errors
Introduction 
What Are Errors?
Syntax Errors
Runtime Errors 
Exercise 6.01: Runtime Errors While Adding Numbers
Semantic Errors
Exercise 6.02: Logic Error with Walking Distance
Error Handling Using Other Programming Languages
Error Interface Type
Creating Error Values
Exercise 6.03: Creating an Application to Calculate Pay for the Week
Panic
Exercise 6.04: Crashing the Program on Errors Using panic
Recover
Exercise 6.05: Recovering from a Panic
Guidelines when working with Errors and Panic
Activity 6.01: Creating a Custom Error Message
for a Banking Application
Activity 6.02: Validating a Bank Customer's
Direct Deposit Submission
Activity 6.03: Panic on Invalid Data Submission
Activity 6.04: Preventing a Panic from Crashing the App
Summary

### 7: Interfaces
Introduction 
Interface 
Defining an Interface
Implementing an Interface
Advantages of Implementing Interfaces Implicitly
Exercise 7.01: Implementing an Interface 
Duck Typing
Polymorphism 
Exercise 7.02: Calculating the Area of Different Shapes
Using Polymorphism
Accepting Interfaces and Returning Structs
Empty interface{}
Type Assertion and Switches
Exercise 7.03: Analyzing Empty interface{} Data
Activity 7.01: Calculating Pay and Performance Review
Summary

### 8: Packages
Introduction 
Maintainable 
Reusable
Modular
What Is a Package?
Package Structure
Package Naming 
Package Declarations
Exported and Unexported Code
GOROOT and GOPATH
Package Alias
Main Package 
Exercise 8.01: Creating a Package to Calculate Areas of Various Shapes
The init() Function 
Exercise 8.02: Loading Budget Categories 
Executing Multiple init() Functions
Exercise 8.03: Assigning Payees to Budget Categories
Activity 8.01: Creating a Function to Calculate Payroll and Performance
Review
Summary

### 9: Basic Debugging
Introduction 
Methods for Bug-Free Code
Code Incrementally and Test Often
Writing Unit Tests
Handling All Errors 
Performing Logging
Formatting Using fmt
Exercise 9.01: Working with fmt.Println 
Formatting Using fmt.Printf() 
Additional Options for Formatting
Exercise 9.02: Printing Decimal, Binary, and Hex Values
Basic Debugging
Printing Go Variable Types
Exercise 9.03 Printing the Go Representation of a Variable
Logging
Log Fatal Errors
Activity 9.01: Building a Program to Validate Social
Security Numbers
Summary

### 10: About Time
Introduction 
Making Time
Exercise 10.1: Creating a Function to Return a timestamp
Comparing Time 
Duration Calculation
Managing Time
Exercise 10.2: Duration of Execution
Formatting Time
Exercise 10.03: What Is the Time in Your Zone?
Activity 10.01: Formatting a Date According to User Requirements
Activity 10.02: Enforcing a Specific Format of Date and Time
Activity 10.03: Measuring Elapsed Time 
Activity 10.04: Calculating the Future Date and Time
Activity 10.05: Printing the Local Time in Different Time Zones

### 11: Encoding and Decoding (JSON)
Introduction
JSON
Decoding JSON
Struct Tags
Exercise 11.01: Unmarshaling Student Courses
Encoding JSON
Exercise 11.02: Marshaling Student Courses
Unknown JSON Structures
Exercise 11.03: Analyzing College Class JSON
GOB: Go's Own Encoding 
Exercise 11.04: Using gob to Encode Data 
Activity 11.01: Mimicking a Customer Order Using JSON
Summary

### 12: Files and Systems
Introduction 
Filesystem
File Permissions
Flags and Arguments 
Signals
Exercise 12.01: Simulating Cleanup 
Creating and Writing to Files 
Reading the Whole File at Once
Exercise 12.02: Backing Up Files 
CSV
Activity 12.01: Parsing Bank Transaction Files459
Summary

### 13: SQL and Databases
Introduction 
The Database 
Database API and Drivers 
Connecting to Databases
Creating Tables
Inserting Data 
Exercise 13.01: Creating a Table with Numbers 477
Retrieving Data
Updating Existing Data 
Deleting Data
Exercise 13.02: Holding Prime Numbers in a Database485
Truncating and Deleting Table 
Activity 13.01: Holding User Data in a Table
Activity 13.02: Finding Messages of Specific Users490
Summary

### 14: Using the Go HTTP Client
Introduction 
The Go HTTP Client and Its Uses
Sending a Request to a Server 
Exercise 14.01: Sending a Get Request to a Web Server
Using the Go HTTP Client 
Structured Data
Exercise 14.02: Using the HTTP Client with Structured Data499
Activity 14.01: Requesting Data from a Web Server
and Processing the Response
Sending Data to a Server 
Exercise 14.03: Sending a Post Request to a Web Server
Using the Go HTTP Client 
Uploading Files in a Post Request
Exercise 14.04: Uploading a File to a Web Server via a Post Request506
Custom Request Headers 
Exercise 14.05: Using Custom Headers and Options
with the Go HTTP Client
509
Activity 14.02: Sending Data to a Web Server and Checking
Whether the Data Was Received Using POST and GET 512
Summary

### 15: HTTP Servers
Introduction 
How to Build a Basic Server
HTTP Handler 
Exercise 15.01: Creating a Hello World Server518
Simple Routing 
Exercise 15.02: Routing Our Server 
Handler versus Handler Function 
Activity 15.01: Adding a Page Counter to an HTML Page524
Returning Complex Structures 
Activity 15.02: Serving a Request with a JSON Payload527
Dynamic Content
Exercise 15.03: Personalized Welcome
Templating
Exercise 15.04: Templating Our Pages
Static Resources
Exercise 15.05: Creating a Hello World Server Using a Static File
Getting Some Style
Exercise 15.06: A Stylish Welcome
Getting Dynamic
Activity 15.03: External Template
HTTP Methods 
Exercise 15.07: Completing a Questionnaire
JSON loads
Exercise 15.08: Building a Server That Accepts JSON Requests
Summary

### 16: Concurrent Work
Introduction 
Goroutines
Exercise 16.01: Using Concurrent Routines
WaitGroup 
Exercise 16.02: Experimenting with WaitGroup
Race Conditions
Atomic Operations
Exercise 16.03: An Atomic Change 
Invisible Concurrency
Activity 16.01: Listing Numbers
Channels
Exercise 16.04: Exchange Greeting Messages via Channels
Exercise 16.05: Two-Way Message Exchange with Channels
Exercise 16.06: Sum Numbers from Everywhere
Exercise 16.07: Request to Goroutines
The Importance of Concurrency
Exercise 16.08: Equally Splitting the Work between Routines
Concurrency Patterns
Activity 16.02: Source Files
Buffers
Exercise 16.09: Notifying When Computation Has Finished
Some More Common Practices
HTTP Servers 
Methods as Routines 
Exercise 16.10: A Structured Work
Go Context Package
Exercise 16.11: Managing Routines with Context
Summary

### 17: Using Go Tools
Introduction 
The go build Tool
Exercise 17.01: Using the go build Tool 
The go run Tool
Exercise 17.02: Using the go run Tool
The gofmt Tool 
Exercise 17.03: Using the gofmt Tool
The goimports Tool
Exercise 17.04: Using the goimports Tool
The go vet Tool
Exercise 17.05: Using the go vet Tool
The Go Race Detector
Exercise 17.06: Using the Go Race Detector
The go doc Tool
Exercise 17.07: Implementing the go doc Tool
The go get Tool
Exercise 17.08: Implementing the go get Tool
Activity 17.01: Using gofmt, goimport, go vet, and go get to Correct a File
Summary

### 18: Security
Introduction 
Application Security
SQL Injection
Command Injection
Exercise 18.01: Handling SQL Injection
Cross-Site Scripting
Exercise 18.02: Handling XSS Attacks
Cryptography 
Hashing Libraries
Exercise 18.03: Using Different Hashing Libraries
Encryption
Symmetric Encryption
Exercise 18.04: Symmetric Encryption and Decryption
Asymmetric Encryption
Exercise 18.05: Asymmetric Encryption and Decryption
Random Generators
Exercise 18.06: Random Generator
HTTPS/TLS
Exercise 18.07: Generating a Certificate and Private Key
Exercise 18.08: Running an HTTPS Server
Password Management
Activity 18.01: Authenticating Users on the Application
Using Hashed Passwords
Activity 18.02: Creating CA Signed Certificates Using Crypto Libraries

### 19: Special Features
Introduction
Build Constraints
Build Tags
Filenames
Reflection
TypeOf and ValueOf
Exercise 19.01: Using Reflection
Activity 19.01: Defining Build Constraints Using Filenames
DeepEqual
Wildcard Pattern
The unsafe Package
Exercise 19.02: Using cgo with unsafe
Activity 19.02: Using Wildcard with Go Test

# Best Way to Learn Python (2020 Step-by-Step Guide)

Python is a very popular language.

It’s also one of the languages that I recommend for beginners to start with.

But how do you go about learning this language?

The best way to learn Python is to understand the big picture of all what you need to learn before you dive in and start learning.

In this article, I divide the path of learning Python into 6 levels.

Each level covers a subset of the language that you need to master before you move on to the next one.

My focus on this article is for you to be a competent well-rounded programmer so you can easily get a job at any tech company that you choose.

But don’t worry, you don’t need to go all the way to level 6 in order to get your first job 🙂

Let’s get started.

## Level 0: The Beginnings

This is the level you begin at if you are an absolute beginner.

And by absolute beginner, I mean someone who has never coded before in Python or any other programming language for that matter.

If you are coming from a different programming language, then you should skip to level 1.

In this level, most of the concepts you will be learning are general programming concepts. The fundamental skills that will bootstrap you as a programmer.

This means that these concepts are not really exclusive to Python but can be extended to other programming languages as well.

You see, a lot of programming languages are very similar and knowing what’s common (and what’s not) between programming languages will help you transition into a different one in the future.

If you are at this level, then I highly recommend this course on Udemy.

So what are some of these general programming concepts that I am talking about?

Some of these fundamental concepts are variables, data types, operations, functions, conditionals, and loops.

If you understand what these concepts are, then skip to level 1.

Otherwise, Let me give you a very brief introduction about what these concepts mean.

### Variables
Variables are essentially storage for data in your program.

More accurately, it’s a way of giving a name for data for later use.

Let’s look at an example.

```python
# variables
msg = "Hello World!"
print(msg)
# this code outputs Hello World! on the screen
```

In the Python snippet above, we define a variable msg that stores the value Hello World!

This allows us to later print Hello World! on the screen by just using the variable name that stores this value instead of having to type the value Hello World! every time we want to use it.

### Data Types
We talked about variables as storage for data, now let’s talk about data.

In Python, data has types.

For example, in the code snippet above, the data Hello World! has a specific type that Python (and other programming languages) call string.

A String is simply a sequence of characters.

But strings aren’s the only data type in Python, there are also integers, floating-point numbers, boolean, lists, tuples, and dictionaries.

By the end of level 0, you need to be comfortable with these data types and understand when (and how) to use them in your program.

### Operations
Operations is how you manipulate and change data in your program.

In other words, your programs need to operate on data and produce more data, that you also operate on, until you reach the final outcome.

This is just the lifecycle of any program.

In Python and all programming languages, there exists at least Arithmetic, Comparison, and Logic operations.

```python
# an example of an arithmetic operation
x = 5 + 2

# an example of a comparison operation
y = 3 > 4

# an example of a logic operation
z = True or False
```

### Conditionals

In order to write any program that is useful, you almost always will need the ability to check conditions and change the behavior of the program accordingly.

Conditional statements using if, if else, or if elsif else gives you this ability.

Here is an example of an if-else statement in Python.

```python
>>> if 3 > 5:
...   print('3 is greater than 5')
... else:
...   print('3 is not greater than 5')
...
3 is not greater than 5
```

### Functions
A function is essentially a block of Python code that only runs when it is called.

You can pass parameters into a function as input and a function can return data as output.

In Python, you define a function using the def keyword.

Here is an example of a hello world program using a function `say_hello`

```python
def say_hello(msg):
  # this is the function
  # msg is the input parameter
  print(f'hello {msg}')

# calling the say_hello function
say_hello('world')
```
```bash
# output:
hello world
```
So this was an example of the fundamental concepts that you should learn at this level.

But most importantly, what you really need to do in order to master this level is to use the above concepts to solve problems.

You will never be a good programmer if all that you do is read books or take courses.

You need to practice solving problems so get your hands dirty and start solving simple problems using Python. You can start by solving Project Euler problems.

I can’t stress enough the importance of mastering level 0.

The reason for that is, this level lays the foundation and the fundamental concepts for not only mastering Python but mastering any other programming language as well.

So even though this is level 0, don’t take it lightly.



## Level 1: Object-oriented Programming


Before we start, if you are at this level, make sure you sign up so that you can get notified when my premium OOP course becomes live.

Everything in Python is an object.

You either heard this already, or you are destined to hear about it 🙂

But wait a minute, what exactly is an object?

There are many different ways, models, or paradigms to write computer programs.

One of the most popular programming paradigms is called object-oriented programming (OOP).

In object-oriented programming, an object refers to a particular instance of a Class.

And a Class is like a blueprint of the state and actions that an object can take.

For example, in Python, a Person Class might look something like this.

```python
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age
  
  def get_name(self):
    return self.name
```
The class declared above describes the state and actions of any Person object.

For example, any Person object will have a name and an age. These two fields are what determines the state of the object.

In OOP’s terminology, name and age are called the object attributes.

You can also call `get_name()` on any Person object to return the name of the person.

We call get_name a method.

And this method, in addition to any other methods that we define, is what determines the object’s actions.

In other words, a Python object has attributes and methods that are defined in the object’s Class.

Here’s how to create a Person object

```python
>>> p = Person('Alice', 22)
>>> p.get_name()
'Alice'
```

Object-oriented programming is essentially one way of structuring and designing your code.

However, I want you to understand that it is not the only way, and it is not necessarily the best way.

In order to learn OOP in Python, you need to progress through a few steps.

### Step 1: Learn the concepts of OOP
As I mentioned earlier, OOP is a programming paradigm, a way of structuring and designing your code.

OOP concepts are not exclusive to Python so the concepts you will learn will easily transition to any other programming language.

Some examples of these concepts are inheritance, encapsulation, and polymorphism.

So make sure you understand these concepts at an abstract level first before you jump into Python’s OOP.

### Step 2: Learn about Python’s Classes and Objects
In this step, you need to apply the abstract concepts you learned in the previous step but specifically in Python.

Get comfortable with writing Classes and creating Objects.

Write classes that inherit from other classes and investigate the attributes and methods of the objects created.

### Step 3: Solve Python problems using OOP
This is a crucial step.

In this step, you want to learn how to use OOP to design and structure your code.

And as a matter of fact, this step is more of an art than a science. That means the only way to get better is through practice, practice, and more practice.

Again keep solving more problems using Python, but try to structure your solutions in an object-oriented way.

The more you practice, the more you will feel at ease with OOP.

## Level 2: Concurrent and Parallel Programming

The days of single-core processors are far gone.

Nowadays whether you are buying an off-the-shelf laptop or a high-end server for your business, your processor will definitely have multiple cores.

And sometimes, your program needs to take advantage of these multiple cores to run things in parallel.

This can potentially lead to increased throughput, higher performance, and better responsiveness.

But let me be clear about one thing here.

If high performance and increased throughput are absolutely crucial, Python wouldn’t be the best language to support parallel programming.

In this situation, I would personally prefer golang instead (or good old C).

But since this is an article about Python, let’s keep our focus on Python.

Before you dive in and write your first parallel program, there are some parallel processing concepts that you should learn about first.

Here are some of these concepts.

Mutual Exclusion
When you have some data that is shared across multiple threads or processes, it is important to synchronize access to these shared resources.

If you don’t, a race condition can happen which might lead to unexpected and sometimes disastrous consequences. I will talk more about race conditions later.

Mutual exclusion means that one thread blocks the further progress of other concurrent threads that require the use of the shared resource.

Locks
Locks is one of the various implementations of mutual exclusion.

To understand what locks are, you can think about them from a conceptual perspective.

If a thread wants to access a shared resource, this thread must grab a lock before it’s granted access to that resource.

And after it’s done with the resource, it releases this lock.

If the lock is not available because it is grabbed by another thread, then the thread has to wait for the lock to be released first.

This simple concept guarantees that at most one thread can have access to a shared resource at a time.

Deadlocks
A deadlock is when your program comes to a complete halt because some of the threads can’t progress further because they can’t acquire a lock.

For example, imagine Thread A is waiting on Thread B to release a lock. At the same time, Thread B is waiting on Thread A to release another lock that Thread A is currently holding.

In this dire situation, neither Thread A nor Thread B can progress any further so your program is hosed!

This is what a deadlock is.

And it happens more often than you think.

To make the situation worse, it’s also one of the hardest problems to debug.

Race conditions
As I mentioned earlier, a race condition is a situation that arises when accessing a shared resource isn’t protected (for example, by locks).

This can lead to disastrous unexpected outcomes.

Take a look at this example.

import threading
# x is a shared value
x = 0
COUNT = 1000000

def inc():
    global x
    for _ in range(COUNT):
        x += 1

def dec():
    global x
    for _ in range(COUNT):
        x -= 1

t1 = threading.Thread(target=inc)
t2 = threading.Thread(target=dec)
t1.start()
t2.start()
t1.join()
t2.join()

print(x)
Here is what the code above does. There is a shared global variable x that is initialized to 0.

Two functions inc and dec run in parallel. inc() increments the value of x 1 million times whereas dec() decrements the value of x 1 million times.

By quickly going through the code, it can be concluded that the final value of x should be 0… but is it?

Here is what I get when I run the above code.

 $ python3 race.py
158120
 $ python3 race.py
137791
 $ python3 race.py
-150265
 $ python3 race.py
715644
The reason why this is happening is that the shared resource x is not protected (by locks for example).

Python’s Parallel Programming
Only after you’re comfortable with the concepts discussed above that you are ready to learn how to write concurrent programs in Python.

First, you should learn how Python’s definition of multiprocessing is different from multithreading. (By the way, this is completely unrelated to threads and processes from an OS perspective).

To understand this distinction between multiprocessing and multithreading from Python’s view, you will need to learn and understand the global interpreter lock (GIL).

You will also need to learn about the threading, queue, and multiprocessing Python modules.

All of these modules provide you with the primitives you need to write parallel programs.

Here is a good article about multiprocessing in Python.


## Level 3: Socket Programming


By now you should be very comfortable writing Python code that runs on a single machine.

But what if you want to write code that communicates with other machines over a network?

If you want to do that, then you need to learn about socket programming.

And for that I highly recommend you learn about the basics of computer networks first. Here’s my favorite book.

After you learn the basic networking concepts, you can use Python’s libraries to write code on one machine that communicates with code on another.

It’s like magic. I still remember the exhilaration I felt the first time I had two laptops communicating back and forth to each other over a Wifi network.

Follow these three steps to get started.

Step 1: Write an Echo Program
In this step, you will use Python’s socket module to write a simple TCP server on one machine and a TCP client on another.

Make sure they are two different computers and that both of them are connected to your home network.

The idea of the Echo program is simple. The client-side reads a message from the user and sends this message to the server over the network.

At the server-side, when this message is received, the server echoes the same message back to the client.

Think of the Echo program as the Hello World program but for socket programming.

After that, you can move on to more complex programs.

Step 2: Play around with HTTP
Once you’re comfortable with writing simple TCP client-server applications, you can start using Python’s requests module to send and receive HTTP messages.

This is especially useful because the vast majority of web services these days provide an HTTP API interface that you can interact with programmatically. For example, Facebook, Twitter, and Google maps all have HTTP API interfaces that your code can communicate with.

And if you feel a little more adventurous and want to take this a bit further, you can also scrape the web with BeautifulSoup.

Step 3: Know thy tools
Like any other program, sometimes when you write a networking program, your program will not work from the first attempt.

However, debugging networking programs is a little different than debugging regular programs.

That’s why you need to equip yourself with the tools necessary to troubleshoot what’s going on.

Here are some of the most popular networking tools that you will need.

ping is used to check the connectivity between your machine and another one.



netstat is a versatile networking tool that allows you to, among other things, monitor network connections both incoming and outgoing.

tcpdump is one of my favorite tools for learning networks. It tools allows you to listen to, capture, and analyze real packets going into and out of your computer through any network interface.

Wireshark is a nice GUI interface that does pretty much everything that tcpdump can do. I recommend starting out with Wireshark before moving on to tcpdump just because it’s a little more user-friendly.



And like I said, to understand what all these Get, SYN, SYN ACK, FIN mean you need to learn networking fundamentals first.



## Level 4: Data Structures and Algorithms in Python


If you reached this level, give yourself a pat on the shoulder.

Because by now, you have the skills that enable you to solve a wide variety of problems.

However, something is missing.

You are still not seasoned enough at writing efficient code.

What do I mean by that?

For example, you don’t know how to modify your code to make it run faster. You can’t even analyze why it is slow in the first place.

This is normal.

The knowledge you have learned so far in the previous levels are not enough for you to have a solid understanding of what performance really is, and how to modify your existing code to make it run faster.

Don’t believe me? Look at this simple code that calculates the nth Fibonacci number.

def fib(n):
    if n < 2:
        return n
    return fib(n-2) + fib(n-1)

print(fib(100))
The code looks simple enough and very straightforward, right?

Try using this code to calculate fib(100) [SPOILER ALERT: it will take an extremely long time]

Now let’s make a simple modification to the code.

def fib(n, d):
    if n < 2:
        return n
    if n not in d:
        d[n] = fib(n-2, d) + fib(n-1, d)
    return d[n]

print(fib(100, {}))
This time all it took was a few milliseconds and you will get the answer, which is 354224848179261915075 just in case you’re wondering 🙂

I used what’s called dynamic programming to solve this problem and make it run astronomically faster.

Well, I hope you are convinced by now that you should learn data structures and algorithms.

The skills that you are going to learn at this level are some of the major differentiators between average coders and solid programmers.

You will need to learn about linked lists, trees, stacks, queues, graphs, hash tables, recursion, dynamic programming, searching and sorting algorithms, etc…

Once you master these concepts, you are steps away from getting a software engineering job at any tech company of your choice.

I really mean it!



## Level 5: Python Coding Interview Practice
Congratulations! Now you have what it takes to apply for any software engineering job in any tech company in the whole world.

You only need to pass this dreaded coding interview.

In fact a series of them.

If you are at this level, I have written an in-depth article about how you can prepare for a coding interview.

A typical coding interview will assess your problem-solving skills, communication skills, knowledge of data structures and algorithms, in addition to how good and efficient you are at translating your thoughts into code.

The best way to pass coding interviews is to give yourself an ample amount of time to prepare.

The more you prepare, the better your interview experience will be, and the more likely you will land your dream job.

Leetcode is an excellent resource with a ton of coding interview questions.



Leetcode allows you to submit your Python solutions to the coding questions and get instant feedback about the validity and the efficiency of your solutions.

After you start working, you will learn a lot on the job and you will start gaining extensive experience in a very short amount of time.

This is when level 6 starts.

## Level 6: Advanced Python

If you want to venture into the territory of Python fluency and take your skills to the next level, then I highly recommend the “Fluent Python” book.

This book assumes you already have a solid understanding of the basics of Python.

In Fluent Python, some of the concepts that you already learned from introductory books are covered from a different angle, in more detail, and with greater depth.

In addition to that, you will learn some new concepts as well.

For example, some of the new concepts that you will learn in this book are

Higher-order Functions: explains how functions can be used as first-class
Thissobjects in Python
Control Flow: covers the topic of generators, context managers, coroutines, and concurrency
Metaprogramming: essentially this is writing code that manipulates code. Some of the topics discussed here are decorators and meta-classes

### Optional 1: Python Libraries and Frameworks
Now you have all the basics covered, you are a Python pro.

Well done.

But the journey doesn’t end here, Python has a ton of useful libraries that can help you even more.

Knowing what libraries to use and when to use them can save you a lot of time and effort and enables you to have the breadth of knowledge that is required to choose the right tools for the right job.

So let’s talk about some of the most popular Python libraries and frameworks.

1. Building API services with Python (Flask)


These days, the way large and scalable web applications are built is by creating a bunch of smaller applications that communicate with each other.

This architecture is called a micro-services architecture [buzzword alert] and each of these smaller applications is called a service or micro-service.

These micro-services can communicate in various ways but one of the most popular methods is HTTP.

In other words, each one of these services will expose an HTTP API that other services will be able to talk to.

With that said, it’s a very good investment to learn how to create API services in Python.

And one of the most popular Python libraries that make this super easy is Flask.

Here is a good tutorial about Flask.

2. Building Web applications with Django
Django is a full-fledged web framework that allows you to create an entire web application (both front-end and back-end) in Python.

By learning Django, you will also be introduced to some concepts that are very popular in other web frameworks in other languages like MVC (model-view-controller) and ORM (object-relational mapper).

MVC is a way of structuring and organizing your web application whereas ORM is a technique that bridges the gap between object-oriented programming and accessing data in a database.

And while we’re at the topic of ORM, It’s worth mentioning that you should take a look at SQLAlchemy which is a very popular, and widely-used ORM library in Python.

So roll up your sleeves and go ahead, create your first web application 🙂

3. Machine Learning Libraries

Python has become the de-facto language for machine learning and data science.

This comes as no surprise, given the maturity of Python’s machine learning libraries.

If you want to be a data scientist, I highly recommend learning the mathematical and statistical fundamentals of machine learning first before learning the ML libraries in Python.

Introduction to Statistical Learning is an excellent place to start.

If you prefer a video course instead, then you should take Andrew Ng’s ML course on Coursera.

Once you have the basics covered, start playing around with these Python libraries.

1- scikit-learn This library has everything under the sun when it comes to ML algorithms.

2- Tensorflow Another very popular open-source machine learning framework.

3- pandas A popular data analysis library.

### Optional 2: Python Implementation (CPython)
Python is an interpreted language.

This means that your Python code doesn’t get compiled down to a machine code directly, but first, it is compiled to an intermediate language, called byte code, which is later interpreted by another piece of software called the interpreter.

Do you want to see how the bytecode looks like for a simple Hello World program?

Let’s create a source file helloworld.py

# helloworld.py
print("hello world")
Here is how to view the bytecode for the above source code

$ python3 -m dis helloworld.py
2           0 LOAD_NAME                0 (print)
            2 LOAD_CONST               0 ('hello world')
            4 CALL_FUNCTION            1
            6 POP_TOP
            8 LOAD_CONST               1 (None)
           10 RETURN_VALUE
This bytecode will then be interpreted by an interpreter. This is when it gets executed and you finally see hello world printed on your screen.

There are various Python implementations for the compiler and the interpreter.

However, CPython is the default and most widely-used one. It’s written entirely in C.

It is both an interpreter and a compiler as it compiles Python code into bytecode and then interprets the bytecode into machine language.

So why am I talking about Python implementation?

Do you really need to know this nitty-gritty details of Python to be a Python master?

Honestly, the answer is no.

But if you are curious about how Python’s list, tuples, functions,.. etc are implemented, and if you are willing to learn a new language (C) along the way, then maybe you should consider contributing to CPython.

And if you don’t know how to get started, then I highly recommend Philip Guo’s 10-hour course on CPython.

Finally, whatever level you’re at, good luck in your Python learning journey :).
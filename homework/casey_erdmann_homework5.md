# Homework 05, CPSC-4175
## Chapter 14, Object-Oriented and Classical Software Engineering September 7, 2017
### Casey Erdmann

#### 1. What are the two basic ways of designing a product? Explain what they are and how they differ.

Operation Oriented Design, and Data Oriented Design.

Operation Orients Design is more concerned with the operations of the software. For example how to data flows rather than what the data is. Data Oriented Design is focused on data structures and conforming the product to those structures.

#### 2. What are the inputs and the outputs to the design workflow, according to the book? Briefly explain why the particular inputs are important and how they impact design. Briefly explain how the particular outputs are important and how they influence design.

Input in terms of design workflow is usually the data that is expected, while the output is what we want the end result to look like. Regardless of data input is very important, as it shapes how we design certain aspects of software.

For example, if input involves PID it would be wise to consider security in the software design. If input is for a video game it influences how the player interacts with the game and plays a huge part in the game's design.

Output equally shapes the design in specific ways. In the simples form, it determines what the user sees. If it's a web page, whatever data the server might return needs to look a certain way, and how the output will play a big roll in deciding on how that data will look. The same can be said for any program that has any sort of visual output.


#### 3. Traditionally, a computer program was seen as a data processing application. Variables were divided into three categories: input variables, output variables, and processing variables. The book describes a design process based on this paradigm that is recursive. Explain in detail how you would design a student’s graduation requirements in terms of input variables, output variables, and processing variables. This is not asking for a design, but just identification of variables you might want to create and where in the design you would place them.


Variable Design for a Student's Graduation Requirements:

- Input Variables:
  - Classification
  - Required Classes Completed
- Processing Variables
  - Required Classes Remaining
  - Academic Standing
  - Financial Status
- Output Variables:
  - Classification
  - Required Classes Completed
  - Expected Graduation Date


#### 4. Perform a transaction analysis for the graduation requirements problem you used for the previous question. Your answer should be a sequential list of sub procedures you would design to solve the problem. Notice that the previous question called for what was, in essence, a list of nouns, while this question calls for, in essence, a list of verbs.

Transaction Analysis of Graduation Requirements:

- Get Classification
- Calculate Expected Graduation Date (Using Required Classes Remaining - Completed)
- Calculate Financial Status (See if any extraneous fees are owed that would prevent graduation)
- Display Classification
- Display Classes Completed
- Display Expected Graduation Date


#### 5. Object-oriented analysis and design conceptually is seen as a grouping of objects, instantiated from classes. Classes encapsulate both states (variables, nouns) and behavior (sub procedures, verbs). Based on your answers to the two previous questions, describe one class that might be appropriate for a graduation requirements application. Identify the attributes (properties) and behaviors (methods) this class might contain.


**class** Student

**property** Name

**property** Classification

**property** Financial Balance

**property** GPA

**property** Major

**method** Get Info (returns the properties of the student)

**method** Calculate Balance (Calculates an up to date financial balance)

**method** Classes Completed (returns the amount of classes completed based on the student's major)

**method** Calculate Expected Graduation Date (uses the student's properties to derive an expected graduation date)

#### 6. As discussed in the book, the design workflow can be considered an iterative, spiral process in itself. As we have been discussing in class, the design phase can be seen as part of an iterative that also includes analysis, implementation, and testing phases. The answer to this question obviously depends on the nature of the software under development, so there is no one correct answer to this question. Here is the question: Consider the software project you are working on for this class, and briefly state which view you think is more appropriate to your work. Justify your answer by making a reasonable argument as to why you answered this question the way you did.

I think to some degree, each iteration of the entire cycle contributes heavily to the design phase. I don't think during the design phase itself that it is appropriate to treat design as it's own iterative cycle, but I do think that through the normal phases of implementation and testing, you may find natural flaws in the initial design that should be corrected on the next design iteration.

So I do agree with the principle that design might have it's own sub-phases, but I think it is more practical to use the actual phases to influence design rather than iterating over the design phase itself.



#### 7. What is the difference between testing an implementation and testing a design? Write a procedure for testing the design of the student graduation requirements problem in the questions above. Define a procedure for one of the following: either a data analysis design, a transaction analysis design, or an object oriented design.

Testing the implementation of something seems more technical than testing the design. By that I mean when you test an implementation you are testing "does this work?" not "does this work well?". When you test the design, hopefully the implementation works, so you can test if the product is designed to work well, rather than just working from a technical aspect.

Testing an Implementation of OOD:
- Unit test for compiling (if applicable)
- Testing each method of each class
- Test that the software is communicating correctly with services/databases
- Test that the program runs in general and doesn't throw any errors


Testing a Design of OOD:
- From a programming aspect, is the class Design efficient? Test for this by following the flow of data between classes and look for inefficiencies (are classes loosely coupled?, following design patterns)
- Interact with the software as a user, test the UI for design issues like confusing UI or inefficient functionality (slow loading)
- Test for security issues by various means (fuzzing, accidental misuse, explicit vulnerability analysis). The software may work correctly if you use it as intended, but what if you don't?


#### 8. What is the cyclomatic complexity of figure 1? Explain your answer.

Answer: **6**

- Condition 1 has two branch options (2)
- Condition 2 has two branch options and a potential loop that causes the - condition to occur again (3)
- Based on the definition it is those above items + 1 for a total of 3 + 2 + 1 = 6


#### 9. Discuss one CASE tool you have previously used. If you have never used a CASE tool, find an open source CASE tool using an internet search, download and install it, complete a “Hello World” application, and discuss your experience.


One major CASE tool I have used is the IntelliJ IDE. It includes many features like Intellisense, which is built into all IDEs published by JetBrains, and is a very useful tool. It is able lint code for errors before compile time, keep the programmer on track with referencing correct classes, and it can even build code automatically based on GUI design if you use it's built GUI editor.

This isn't a CASE tool in the traditional sense, because it is an IDE and not a tool dedicated to CASE. However, it is very much one based on definition due to the power and feature set it it has.

If you wish to integrate documentation standards, or other design standards it also has tools built in to assist with that.

#### 10. Read the article “the-right-stuff.pdf” in the pdf directory. (You may find a better copy online.) Write a one paragraph appreciation of the article.

The Right Stuff opened with a really powerful argument for software needing to be perfect, but quickly points out how that can be achieved, by the process. In commercial business, sometimes lives aren't at stake, in fact sometimes the software isn't what drives the business, but that doesn't mean it failing can't cause damage. The article really showed that the "right stuff" comes out of the process used when building software. Software isn't good or bad because of what its application is. It is good or bad because it is written to be that way. In the case of NASA, it HAS to be good or things go horribly wrong. However, if everyone designed software with a process similar to that of development teams who build software for rockets, then perhaps that 5,000 average error count would disappear. I wasn't really all that reeled in or convinced by this article of anything new, but the point was clear, and that is process is important.

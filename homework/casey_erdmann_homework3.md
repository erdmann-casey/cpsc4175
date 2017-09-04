Homework 03, CPSC-4175
Chapter 12, Object-Oriented and Classical Software Engineering
August 16, 2017


#### 1.  What two kinds of things must a software requirements specification contain?

Functional and non-functional requirements.


#### 2.  Give an example of an ambiguous requirement in English (that is, using a natural language).  Explain the ambiguity.

The software must have an option to select from a menu of people in the People table defined by the database.

The ambiguity here isn't the functionality, but how the developer chooses to allow interaction with the functionality.
The requirements do not specify whether the option to select is a set of buttons, a pick list, a drop down menu, or some combination of those elements.
Therefore the developer can make the decisions they think is best when it comes to the user functioning with this "menu of People".

#### 3.  Consider the domain of processing student grades.  Draw a simple data  flow  diagram of the process. Create the drawing as a PDF and upload the file to your Github repository. Explain the drawing in English as your answer to this question.

The Student's flow of data goes to the Grading System. The student sends their work, and any complaints or requests to the Grading System.
The Teacher's flow of data goes to the Grading System. The teacher sends any fixes, comments, and other information to the Grading System.
The Grading System is responsible for taking the data flow and distributing it the appropriate parties. In this case when the student submits any of their data the teacher will grade, and send there data back through the grading system.
The Grading System then sends data to the student. The student will receive the information/feedback from the teacher along with their graded work via the Grading System.

#### 4.  Consider the domain of an online shopping cart.  Draw a simple finite state  machine of the process. Create the drawing as a PDF and upload the file to your Github repository.  Explain the drawing in English as your answer to this question.

The cart starts in an Empty State. From there only state it can go to is an Active State by the event of adding an item.
Once in an Active State after adding an item, it can add an item, remove an item, or proceed to the Paid State.
If another item is added, it loops back to the Active State. If an item is removed, it goes back to the Active State, unless it is the last item in the cart, in which case it will return to the Empty State.
Once shopping is completed the Active State can be transitioned into the Paid State after the Pay event occurs.

#### 5.  Consider the domain of a database with customer, products, and orders tables.  Draw a simple entity-relation diagram of the database.  Create the drawing as a PDF and upload the file to your Github repository.  Give an account of the data structure in English as your answer to this question.

- Products have Orders associated with them.
- Orders have Products, Customers, and a Store associated with them.
- Customers are entities that don't have any relational dependencies.
- Stores are entities that don't have any relational dependencies.



#### 6.  Consider the project you have chosen as a team.  Draw a simple SADT(structured analysis and design technique) diagram of the project.  Create the drawing as a PDF and upload the file to your Github repository.  Explain your project on a high level in English as your answer to this question.

The SADT Activity is the Storage of Images and Text.
The Activity receives an input of image or text. The input is then validated by the control activity, and if it is an image the mechanism will save the file.
The Output generated is either a shareable link to the text or image based on the input passed into the main Activity.

#### 7. This  is  not  in  the  book.   Consider  the  project  you  have  chosen  as  a  team.   Draw  a  simpleSDL (Specification and Description Language) diagram of the project.  Create the drawing as a PDF and upload  the  file  to  your  Github  repository.   Explain  your  project  on  a  high  level  in  English  as  your answer to this question.

A user visits the application. They supply an image or text to share. This input is then stored, and a shareable link to the input is generated as output.

#### 8.  Find an image or document online of a simple function using Z. Convert the image or document to a PDF and upload it to your Github repository.  Explain the specification in English as your answer to this question.  Note that the Z language is difficult and takes years to learn.  This course is not a course in Formal Methods,  where you might spend an entire semester learning the Z language.  You don’t have to understand the Z specification.  All you have to do is have some faint idea about its concept and operation.

In order to withdraw money the dollarAmount needs to be less than or equal to the amount in the account.
The same check applies to the centAmount.
If the centAmount is greater, then a calculation to find dollar' and cents' occurs.

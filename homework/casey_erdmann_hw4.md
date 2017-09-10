# Homework 04, CPSC-4175
# Chapter 13, Object-Oriented and Classical Software Engineering
# August 30, 2017
## Casey Erdmann

#### 1. What is an entity class? A boundary class? A control class?
Entity Class: A class that models important information that is "long lived". Examples of this might be, Account Class in terms of a bank or even a user account like a profile for social media.

Boundary Class: A class that models a software product and its "actors". Examples of this usually are anything dealing with input and output such as a class the generates reports.

Control Class: A class that models complex computations and algorithms. Examples of this could be something performing calculations or complex sorting.

#### 2. Write a use case pertaining to your project.

Use case for "Brisket" would be:
```
User -> Views Images
     -> Views Text
     -> Searches Images
     -> Searches Text
     -> Uploads Image
     -> Uploads Text
```

#### 3. Write a successful scenario pertaining to your project.

1. User visits the site
2. Images on the site load successfully
3. User clicks the "Upload Image" button
4. User selects an Image to Upload
5. User successfully Uploads the Image
6. A link to the Image is generated for the user to copy and share

#### 4. Write an unsuccessful scenario pertaining to your project.

1. User visits the site
2. Images on the site load successfully
3. User clicks the "Post Text" button
4. User types their text to Post
5. The user text exceeds the permitted size to Post
6. User leaves the site to share their text another way

#### 5. Using your answers to the three previous questions, use the noun extraction method to extract the classes. If practicable, identify the classes you extract as entity, boundary, and control classes. If all your classes are entity classes, you will not be able to do this.

Entity Classes: Image Class, Text Class

Boundary Classes: Uploader Class

Control Classes: Link Generator Class

(Our application is mix of OOD and functional programming depending on the section of the app, so these don't 100% apply, but for the sake of the assignment this is what I came up with)

#### 6. Using your answer to the previous question, draw an appropriate class diagram.

[Homework 4 Class Diagram]()

#### 7. Complete a CRC card for one of your classes.

[Homework 4 CRC]()

#### 8. Draw a state chart for one specific behavior of your project.

[Homework 4 State Chart]()

#### 9. Draw a communication diagram for one specific realization of a use case.

[Homework 4 Communication Diagram]()

#### 10. Draw a sequence diagram for one specific realization of a use case.


[Homework 4 Sequence Diagram]()

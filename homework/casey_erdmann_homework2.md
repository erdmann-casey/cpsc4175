# Homework 02, CPSC-4175
## Chapter 11, Object-Oriented and Classical Software Engineering
## August 12, 2017

### Casey Erdmann

#### 1. What is the first step in creating a piece of software?

  Simply put the first step in creating a piece of software is to analyze the requirements. In perspective this could mean understanding a client's problems, analyzing the domain where the software solution is being applied, and making sure there is clear communication between you (and your team if applicable) and the client about what it is they want to get out of the software.

#### 2. What is the difference in discovering what the client needs and discovering what the software should do?

  Discovering what the client needs is what impacts what the software will actually do, but these aren't the same thing.

  The client's needs might be what makes up some of the requirements for the software. However, the discovering what the software will do as a whole is a summation of all the requirements, including the client's needs.

  For example, maybe the client is a bank and they need software that will allow their users to withdraw money from their bank account. That is a client need.

  The software will need to be able to contact the bank, do various authentication methods for verification, need access to account information, a machine to dispense money, etc... (basically I am describing an ATM)

  So in order for the Software to do what the client needs, it ends up requiring a little more than the statement "it needs to let users withdraw money from their bank accounts".


#### 3. In what sense is a software engineer a generalist rather than a specialist?

  Well a Software Engineer might have to apply their skills to many domains. So while they may specialize in "software" that isn't truly a specialization.

  Software can have many genres and applications across many professional domains from finance to medical, or even something like video games.

  As a result writing software is a generalized skill that can be applied to many domains. That's why a Software Engineer might be considered more of a generalist.


#### 4.  List some techniques the book identifies as useful for determining requirements, and for each, give one reason why that technique might not be effective.

  - Determining what the client needs: This is generally effective and is usually the first step into creating software requirements. However, in the event that the client doesn't NEED the software they are asking for but they still WANT it even after you suggest an alternative, then it is fruitless to investigate the need.
  - Understanding the Use Cases: While it is important to understand what the use case for software might be, this could end up being less effective than you might think. If you design a piece of software and focus solely on the use case requirements, and then a user decides to use the software in a way that you did not account for, then your use case based design goes unused.
  - Understanding the Business Model: This is great and can really allow you to find out information about how your software is going to need to be designed in order to flow with the business model. But what if the business model changes, or what if your software is supposed to change the business model? Well in case of the business model changing, you will have to update your software at some point to support this. In the case of your software changing the business model, then it is less effective to understand the business model, and more effective to understand how you are going to change it.

#### 5.  In what sense are requirements dynamic rather than static?

  Well requirements can change throughout development in a lot of ways, especially if you are supporting the software even after initial release. Even during initial development requirements can change too. Maybe a client wants to add a new feature, or remove one during the development process. Those changes will affect the software's requirements. Requirements are never really concrete which is why they are considered dynamic. While in some cases they may not change, that doesn't mean that they can't change.

#### 6.  In your own words, state the difference between functional and nonfunctional requirements. Do you think that there is any such thing as a “nonfunctional” requirement?

  A functional requirement is something the software does, while a non-functional requirement is something the software is (like an attribute of the software).

  There are definitely non-functional requirements of software. The UI/UX design is a very big one. Also things like verbiage in text that is displayed, or the navigation structure of the software. Anything that is not a functionality of the software, but is necessary, is a non-functional requirement.

#### 7.  What  is top-down analysis?   You  may  also  see  this  referred  to  as structured analysis.  How  is  this different than the case study in chapter 11 in the book?

  Top-down analysis is all about looking at the big picture first. In software engineering this means identifying the overall solution to the problem from a more generalized view, and breaking it down from there (starting from the top, and moving down).

  This is different from the case study in the book, because the case study in the book builds up to the bigger picture, rather than down from it. It describes identifying specific sections and requirements and building piece by piece to make the whole.

  At the end of the day you will still build piece by piece to create the "big picture" so to speak, but your perspective and how you design the software is very different based on which approach you take.

#### 8.  Prototyping is a very controversial issue.  Can you think of some reasons why many software engineers think that prototyping is harmful?

  Prototyping is generally a good thing in my opinion. It can really help demonstrate what the software will look like and how it will function, and it can help correct foundational issues early on. However, prototyping does have the potential for major flaws.

  One of these flaws is misinformation to the client. If the client sees a prototype of a piece of software, and it's doing everything they want, then they may be confused why it isn't the finished product. Resolving that kind of issue just takes good communication, but without it, your prototype could come back and bite you.

  Another flaw is that if you build a prototype, you may accidentally base your final model off that prototype. A prototype should never be anything close to the final product. The only purpose of a prototype is to demonstrate a proof of concept.

  One last flaw I can think of is that it creates a false solution. If you prototype something, and fake a core piece of functionality that hasn't been developed for the sake of demonstration, then you can really hurt yourself in the long run. What if that fake functionality has a fatal requirements conflict and can't actually be implemented? If so your client won't be happy about that.

#### 9.  Teams One and Two both have the responsibility for developing a software requirements specification for a project.  Team One has infrequent changes to its requirements specification, while Team Two has very frequent changes to its requirements specification.  Which team is doing the better job?  Justify your answer.

  This is extremely ambiguous, and my actual answer is that there is not enough information available to truly answer this question.

  However, for the sake of argument I am going to assume a few things and pick a side.

  I am assuming that these teams are following a specific software development process, spiral development, since that has been the topic in class.

  I am also going to assume they are creating requirements for the same project.

  Lastly I am going to assume that each iteration of the cycle is when software requirements are changed, and they are not just arbitrarily being changed at any time (i.e. they are correctly following the development cycle).

  Based on these assumptions I pick Team Two. This is because software requirements are dynamic, and the frequency at which Team Two's requirements are changing a indicative of them progressing in the Spiral Development cycle.

  Now it is important to note that this argument isn't concrete it is just the most logical with the data provided. However, changing requirements isn't necessarily a positive thing, nor is it necessary. It could be argued that Team One has progressed just as much, but the software requirements changes just aren't a good indication of Team One's progress.

#### 10.  More software defects are traceable to bad requirements analysis than to any other source.  Why do you think this is true?

  I think it is for one simple reason, that is if software doesn't function like it is supposed to, it likely means that something from the requirements wasn't implemented correctly.

  For example if a piece of software has requirements that specifies the following: There must be a way for users to take notes in the software, and those notes are to be stored in a database. The notes must accessible from the software on another page.

  If the Software Engineer looks at that, and creates it, but doesn't have a way to differentiate between the users accessing the application, then that will cause a huge problem because every user will be able to see all notes by all users.

  Now that is a very simple trivial requirement, but it shows that if the Software Engineer doesn't carefully analyze the requirements, read between the lines, or ask questions to further clarify, then you will end up with a major defect in the software.

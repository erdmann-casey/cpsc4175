# Homework 10, CPSC-4175
# Chapter 09, Object-Oriented and Classical Software Engineering
## October 16, 2017
## Casey Erdmann
### This homework includes significant research requirements beyond the text.  It’s more important to focus on the general concepts than it is to memorize formulas.  It’s also important to illustrate your understanding of the concepts by giving examples, and by writing brief summaries of the material.

#### 1.  In building a software product, the book identifies two kinds of planning that must occur.  Name the two types and give two examples of each.

I didn't find two distinct plannings that occur as defined by the book, but what I did find was:

1. planning for the project
2. testing the plan

Planning for the project involves all sorts of steps. Software life cycle, cost of building, software requirements, are all just a few of the things that go into software planning.

Testing the plan involves using many modules for each step of the project plan. Each of these modules should be designed to thoroughly test the plan, and insure it's accuracy.


#### 2.  What  does  figure  9.1  tell  you  about  the  range  of  cost  estimates  during  the  various  workflows  of  a software project?  Be specific as to the percentage of uncertainty at each of the four workflows shown on the X axis of the chart.

Around 80-90% of the cost estimate is made during the requirements and analysis phases.


#### 3.  The book identifies two different kinds of costs associated with building a software product.  Identify the two kinds of costs, and for each give two examples.

1. Internal cost - the cost to the Developers, this is like the salary of a Developer.

2. External cost - the cost to the client, this is like the cost of the software.

#### 4.  The  book  lists  six  reasons  why  the  LOC  (lines  of  code)  metric  may  not  be  satisfactory.   List  four of them and for each,  give an example (preferably from your own personal experience) showing the problematic nature of that reason.

1. Writing code isn't the bulk of the software process. Figuring out what the software needs to do (requirements) can often take more time than it will to implement. For example, when deciding on my project, it took several hours to pick the functional requirements. One of these requirements was the ability to upload images and text. However, implementing this took only 1 hour at most versus the many hours it took to come up with the requirements.

2. Implementing the same product in multiple languages can result in different lines of code. This one is an example I encounter far too frequently. When developing mobile apps, Objective-C and Swift for iOS development is far less verbose than Java is for Android. The libraries for iOS are also make many basic things far simpler to implement. What takes me 2 lines of code in iOS programming, takes 10 lines in Android.

3. Defining "what is a line of code" is difficult. I see this at my job very often. While we do adhere to programming standards, there are slight flavors of this standard that vary from developer to developer. While the change between programming styles never falls away from the standard, it can definitely be different enough to add or reduce lines depending on a programmer. It doesn't mean one programmer is better than the other, you could have two solutions that are exactly the same, but one has a few more spaces than the other therefore adding more lines. Are those really "lines of code"? Well some might say yes, some might say no, I don't think anyone is wrong, but it proves this point exactly.

4. Code generation may add lines of code. Yes, especially in writing GUI for Java. There is a fantastic GUI code generation utility, and it implements things far more correctly and quickly than any java programmer I have ever seen. However, it adds extra lines to be more readable. This doesn't reflect the work of a programmer though, because this code was generated.

#### 5.  The function point metric is widely used.  Do some independent research on function point analysis/-function point estimation and write a brief summary of your research.  In particular, Does there seem to be a widely accepted formula for function point estimation?

This basically categorizes the inputs/outputs/inquiries/etc...(requirements) of a software and assigns "point" values to them to measure the size of a given project.

There doesn't seem to be a standard in place, but one formula I saw a lot was:

 FP = UAF * VAF

 Where UAF is Unadjusted Function Point and VAF is value adjustment factor.

#### 6.  The book references IEEE-158.  This standard has been superseded by IEEE-16326.  I have placed a copy of IEEE-16326 in the SWE directory of my Github repository for CPSC-4175.  Select one major subsection of subsection 5 (Elements of the project management plan) and write a brief discussion of that major subsection.  Choose whatever item interests you.


Project Deliverables:

Project Deliverables are everything that needs to be produced as a result of the project. In the case of software these are things like, how the software is packaged, the software itself, the source code (if applicable), instructions for the software, etc...


#### 7.  The book notes that, for every 100 hours developers spent on implementation, they spent 150 hours on activities related to documentation.  Give some thought to your project in this class, and state some practices and/or guidelines you may adopt in an effort to generate appropriate documentation for your project.  As you will discover when you work as a developer, in many cases, a failure to document your efforts is tantamount to a failure to complete the project.

Commenting on code as you go can help if you plan to document post-implementation. Where possible, document during implementation. This is difficult to do with this project as the implementation could change fairly quickly, so unless I am sure the functionality of a method won't change, it is hard to document. So that is why commenting in detail can assist in speedy post documentation later, that way you won't have to read into the code quite as hard because you left yourself some notes.


#### 8.  Why  do  you  think  a  user  would  conclude  that  you  did  not  write  a  piece  of  software  if  you  did  not document the software?

Well not ALL software needs documentation. For example, a quick scripting tool that has clear instructions as part of the software doesn't need documentation. While having documentation would be responsible, the clear instructions are often more than enough. So in this case I would argue that it is because the user is stupid and mean.

However, if instructions aren't clear, and there is no documentation, it can appear incomplete. In this case I would understand a user seeing the software as unfinished, therefore concluding that you never finished writing it.

It's perspective overall though. I don't think a user ever has a valid opinion to determine whether I wrote software or not based whether it has documentation or not. They can certainly quantify other metrics to come to this conclusion, but documentation is not one of them. If the user is my client, and they didn't request documentation as a deliverable, it is really none of their business whether or not we documented the software or not, that is an internal development practice concern. As long as I provide all deliverables accurately and up to spec, then I have written the software. I'm not arguing that it's okay to not document code/software, I personally think all code should be documented when possible, but I am arguing against the stance of a user having a valid opinion on concluding a piece of software is not written based on lack of documentation, as long as it was completed and delivered correctly.

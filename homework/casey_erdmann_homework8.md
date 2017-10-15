# Homework 08, CPSC-4175
# Chapter 3, Object-Oriented and Classical Software Engineering
# October 9, 2017
## Casey Erdmann
### Note: The text for this class uses some terms in ways that are not consistent with the way that I have used these terms. Software engineering has not been systematized to the point where all terms have one meaning, and only one meaning. To some extent this is true throughout computer science, for example, “variable” sometimes means a single assignment variable (i.e., a constant), sometimes means only that which can appear on the left hand side of an assignment operator, and sometimes means an expression or a token that can appear on both the right hand side and left hand side of an assignment statement. The key is to understand the concepts to which the term refers, and not to get confused by the fact that sometimes the same word can refer to different concepts. When you work as a software developer, you will learn to adapt to the terminology of your employer, even though it may not conform to your previous experience. Again, don’t get confused when the words don’t mean what you might expect them to mean.
#### 1. The book notes that the Unified Process is not “a specific series of steps.” It notes that “[i]nstead, the Unified Process should be viewed as an adaptable methodology.” Given this, how should you approach the content in this chapter that seems to present the Unified Process as a specific series of steps? How would you approach this chapter if you in fact viewed the Unified Process, not as a process, but simply as a methodology?

I would make note of the steps as they are presented, and point out the goal achieved by the process. From there to adapt it as a methodology, I would modify steps as needed to achieve the same goal depending on my environment. That is the definition of using this as an adaptive methodology.


#### 2. The book states that “[t]he object-oriented paradigm is an iterative-and-incremental methodology.” Do you think that this is a true statement? How is this similar to our class discussions of a spiral approach to software engineering? Is there any difference between these two views, and if so, what is the difference?

The object-oriented paradigm can definitely be seen as an iterative-and-incremental methodology. When designing classes for objects it tends to make sense to do this in steps. If I want a class that handles network connectivity, and then another one that executes code based on the network status, I would design these classes in an iterative manner, building based on dependencies in each iteration.

This is similar to our spiral approach, but the spiral approach is more broad. I could implement the object-oriented paradigm inside of a spiral process, so the spiral process can facilitate the object-oriented paradigm, but it could also facilitate other paradigms as well, so they aren't the exact same.


#### 3. In class, we are using an iterative process with four phases: analysis, design, implementation, and testing. The book discusses the five core workflows of the Unified Process. List the five core workflows, and for each, give a brief summary of the workflow.

Requirements:
In the Unified Process this workflow exists in the inception and elaboration phases. This means this workflow consists of determining if software is worth making, and if it is, requirements are built and refined.

Analysis:
This workflow exists in the elaboration phase and bleeds into the construction phase a little. Here requirements are finished being refined, and are looked over and revised more as needed.

Design:
Design occurs at the end of the elaboration phase, once requirements should finally be refined. Basically, the software is defined before construction is begun.

Implementation:
Occurs during the construction phase. Simply put, this when the software is actually built.

Test:
Occurs during construction and during the transition phase. Software is tested during development, and then tested further to insure all requirements have been met.


#### 4. What is the relationship between the software project management plan and the software development process? Do you think that a software project management plan can replace an explicit software development process? Why or why not?

Software project management is how the project is managed, while the development process is how the software is created. Trying to replace the process with a project management plan would be like trying to replace how a transaction is conducted in a super market with the way the store is managed. That doesn't make any sense at all. The software development process fits inside a project management plan, but can not be replaced by it.


#### 5. Section 3.7 discusses testing with regard to four process areas: requirements artifacts, analysis artifacts, design artifacts, and implementation artifacts. What is the difference between the test workflow discussed in the chapter, and the testing of the artifacts produced in each of the five process areas? Do you think that this is an inconsistency in the book’s treatment of testing?

Unless I am reading this wrong there isn't a difference, but rather the artifacts define the overall workflow. Also it is definitely not an inconsistency because the book explicitly states "The nature of the test workflow changes depending on the artifacts being tested.", so the test workflow adapts based on the artifacts.


#### 6. If it is true, as the book claims, that “[p]ost delivery maintenance is not an activity grudgingly carried out after the product has been delivered and installed on the client’s computer,” how do you fit post delivery maintenance into an iterative, spiral development model?

I would think it would continue the same process as building the initial software. Instead of starting from nothing, you take your current product, identify the post delivery maintenance issue/update, create requirements, analyze, and the implement. It'd fit perfectly into the spiral development model.


#### 7. Look at figure 3.10 on page 88 of the book. This figure seems to suggest a model of five workflows (requirements, analysis, design, implementation, and testing), with each workflow consisting of four phases (inception, elaboration, construction, and transition). In class, we have talked about an iterative, spiral model with four phases for each iteration (analysis, design, implementation, and testing). Do you think that these two approaches are mutually exclusive? Do you think that they are mutually supportive? Before you answer, review your response to the first question.

Well i think that the spiral model actual fits inside the suggested model. The difference is the spiral's phases equate to the workflows in the suggested model, but this suggest that the spiral model supports the suggested model. Therefore I'd say they are mutually supportive.


#### 8. Look at figure 3.2 on page 94. In a sense, the waterfall method can be easily adopted to an iterative, spiral development model, using the waterfall approach to model each iteration, i.e., not a “waterfall” but a series of rapids, or a cascade. Viewed in this way, how do you think model 3.2a and 3.2b would actually differ in a real-life project? Do you think that they would basically amount to the same thing, or do you think that they would be fundamentally different?

If you continue to treat each waterfall iteration as an "engineering", as in building a bridge, process, then yes they would be fundamentally different. Otherwise they would amount to the same thing if you treat it like software engineering.


#### 9. The last section discusses software process improvement. What is the difference between software improvement, and software process improvement? How important do you think that software process improvement is in the field of software engineering?

Software improvement is about the actual software improving. Software process improvement is about improving the process by which software is created. This is definitely important in software engineering. If there is a way to improve the software process overall, whether it is development, testing, management, etc... then we definitely should.

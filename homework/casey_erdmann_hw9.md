# Homework 09, CPSC-4175
# Chapter 02, Object-Oriented and Classical Software Engineering
## October 10, 2017
## Casey Erdmann

### 1. The book depicts an ideal software process as a linear flow, like this:
#### Requirements ⇒ Analysis ⇒ Design ⇒ Implementation

#### The book then notes that “software development is considerably different in practice.” Which reason do you think is more important for this difference, human error or changing requirements? Why?

Changing requirements. The reason is because changing requirements is a conscious, purposeful effort, where as human error typically describes an accident.

So the importance of the changing requirements comes from the fact that it is thought out and purposeful. Human error can occur anywhere at anytime, and we can account for the best we can, but we can never measure whether it will be a small impact or large impact. The change of requirements however can definitely be quantifiably measured.


### 2. What do you think that the book means when it says that “the waterfall model, which was first put forward in 1970, is iterative (but not incremental)?”

The waterfall model is meant to end on the last iteration. There is no incremental step where requirements are re-introduced and the whole cycle is stepped through again. Once the last iteration is done, the project is complete, there is no incremental step afterwards.

### 3. Using the book’s explanation of stepwise refinement, relate an account from your previous personal experience when you used this type of development model. This does not have to be software related. Were you successful in your development? Why or why not?

At work at times I will use this philosophy for a task I am working on. For example say I need to display data on a page, and the data needs to be formatted a specific way, and the data needs to be ordered a certain way.

Well if I am having trouble retrieving the data, I'll postpone the details of the task until I have refined the core functionality of what the software needs to be doing, and that is successfully retrieving the data to be displayed.

After that has been refined, I'll add in the final details last.



### 4. Looking at figure 2.4 in the book, you see that the Requirements workflow ceases at some point early in iteration 3, while the Test workflow runs from the very beginning of iteration 1 and ends at the very end of iteration 4. Make the case that the Requirements workflow should occur in all iterations. Make the case that the Test workflow should not begin until iteration 2 at the earliest.

The case for requirements workflow being revisited in each iteration is simple. You need to be sure you are correctly implementing the requirements. It doesn't matter how smart you are, or how good of a memory you have, it is wise to re-read and review the requirements as often as possible to insure there are completed correctly.

The test workflow not beginning until iteration 2 also just makes sense. You can't test something that hasn't been implemented. If you are reviewing requirements on the initial iteration of a project there will not be anything to test.


### 5. Iterative and Incremental Model The book notes that “each iteration can be viewed as a small but complete waterfall model.” This is sometimes called the cascade model. Think about your experience in building your class project. How would you explain the iterative and incremental model to a young programmer who asked you how it worked. This question calls for a reflection on your experience, not a textbook answer. (Note that the iterative and incremental model and the spiral model are not the same thing — in this class we are using the spiral model.)

Well I would explain to them waterfall first. Then I would explain how waterfall makes sense for Engineering but not necessarily for Software Engineering.

Then I would explain the software Life-cycle, because this is the whole reason why the waterfall methodology isn't necessarily the best for Software Engineering.

After that I would explain the cascade model, and transition into some other models such as agile or the spiral model once they start understanding.


### 6. The book notes that “a critical point regarding the waterfall model is that no phase is complete until the documentation for that phase has been completed.” Do you agree with this statement? If this statement were true, what changes in your personal process would you make to conform to this dictate?


Sure I agree with this in context of the Waterfall model. I think this could be a smart concept to apply to an incremental model, but it is not necessary.

See in the waterfall model, each stage should be documented because each stage is originally intended to be finite. However in incremental models, documentation for each iteration might be wise, but it isn't necessary. Documentation can be performed later, however in order for documentation to stay up to date, documenting on each iteration is a smart thing to do.

I wouldn't make any changes currently with my personal process based on this, but it is something I would consider in the future.


### 7. The book discusses nine process models:
#### - Evolution-tree Life-cycle Model
#### - Iterative-and-incremental Life-cycle Model
#### - Code-and-Fix Life-Cycle Model
#### - Waterfall Life-Cycle Model
#### - Rapid-Prototyping Life-Cycle Model
#### - Open-Source Life-Cycle Model
#### - Agile Processes
#### - Synchronize-and-Stabilize Life-Cycle Model
#### - Spiral Life-Cycle Model

#### Of these seven, which do you think fits most closely with the software development process you think you would feel comfortable with? What is it about this process that appeals to you?


Both the Agile and Spiral models appeal to me the most. Spiral is appealing because for ticket based work it is repeatable and refined.

However for building software from scratch, agile provides a system that is useful when it comes to being able to adapt and measure progress in a way that other models just don't do as well in my opinion.

### 8. This question is semi-optional — I don’t expect you to spend more that 15 minutes answering this, and I’ll be very lenient in grading this question. Open the paper Recursive Functions of Symbolic Expressions and Their Computation by Machine, Part I, which is recursive.pdf in the PDF directory of my Github account. Read Part 2 only, pages 2 to 8. I won’t ask you to study this paper, to do so would be an onerous assignment in itself. Write a one paragraph appreciation of Part 2. Those of you who are mathematically inclined may find that this suits your taste. For those of you who aren’t, this is an essential paper that you should at least have seen, even if you don’t have much patience with the mathematics.


Being that I have a lesser taste for mathematics, this chunk is a bit hard to appreciate. It clearly has value, and articulates concepts I am familiar with, but it does so in a way that would take me more time to understand than I care to give. Obviously this was expected by the nature of this question, but I wanted to try and find some common ground with this section. The common ground I found was under the Recursive Function Definitions section. This mathematical break down made the most sense to me, and I can admire that there is a formulated way to express this concept.

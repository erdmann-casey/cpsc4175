# Homework 07, CPSC-4175
## Chapter 6, Object-Oriented and Classical Software Engineering
## October 2, 2017
## Casey Erdmann

#### 1. Where, in the software construction process, should testing occur? Explain your reasoning.

      The actual "Testing" phase should always occur AFTER implementation. One methodology of software development is to design tests first,
      and implement based on the tests that are designed. While this is a valid way to construct software, this is not the same thing as the "Testing" phase.

      In the "Testing" phase not only should the software undergo unit testing, but also quality assurance testing. Software cannot be QA tested fully unless the requirements being are implemented. This doesn't necessarily mean that the entire software should be completed of course, but the implementation goal of the current iteration should be completed so it can accurately be tested. If the requirements for a given iteration are incomplete, then they should always fail a QA test by default, which is exactly why testing should occur after implementation.

#### 2. Explain the differences and similarities between verification and validation.

- Similarities:
      - Both verification and validation deal with the affirmation of something
      - They both deal with showing something is accurate
      - By definition they are actually synonyms, so they are basically the same thing.
- Differences:
      - The only difference you can maybe draw between these two words is more so in the context of how we use them in culture sometimes.
        This is that verification means something is true, but validation means that something is just and true. This comes from how we use verification to describe identifying someone, as in I verify that I am who I say I am, but we use validation to describe one's actions being good and true. When we "validate" someone that is what we do, we affirm that their actions are correct (morally) and true.

#### 3. Explain the difference between execution-based-testing and non-execution-based-testing.

      - Execution based testing is like unit testing, you run code against modules that execute test cases to make sure there are no issues.
      - Non-execution based testing is sort of like code review. It is a static analysis of the code to check for errors manually rather than by running the program.


#### 4. Discuss the concept of quality as that word is used in the phrase “software quality assurance.”

      - Quality in "software quality assurance" means whatever a business/company/development team wants it to mean. By that I mean that depending on the focus of a company, the definition of "quality" when it comes to SQA, might change. For some companies it may mean a hard focus on no bugs to have clean polished software. For others the focus might be functionality, and insuring that the software does what it says it's going to do. Ideally however, it should be used to defined as insuring quality by making sure software is:
            1. Secure
            2. Functional
            3. Stable
            4. Correct
      This means the software keeps best security practices in mind, it works and works well, and it works correctly!

#### 5. Why should software not be tested by the implementors, and not implemented by the testers? Think of an illustration from your life experience (not necessarily IT related).

I have only worked in IT since I graduated high school, so unfortunately I don't have a cool non-IT related experience I can think of at the moment. However in my experience this can equate to a situation that is encountered with help desk style IT. If a teacher tells me something is broken, like an iPad not holding its charge. They try to fix the issue by leaving it plugged in and using it, before coming to me. They might have successfully mitigated the issue, but that doesn't fix the problem that the iPad needs to be serviced.

That's exactly why software shouldn't be implemented by testers and vice versa. While my example doesn't go both ways, it does apply both ways. Software developers know their software, and will use it how they think it SHOULD be used, but they will miss all the cases when people don't use it the way they think it should be used.

Testers will find those weird cases and help make the software better, but just because a tester knows how to make the software better does not make them qualified to implement the solution. The testers don't understand the software like the developers do, so providing a solution in the form of requirements based on testing is what they should do, not attempting to implement it themselves.

#### 6. Explain the difference between correctness proofs and execution testing? Which is “better?” Why?

Correctness proofs are a mathematical proof that a solution/algorithm will always produced the expected outputs correctly every time.

Execution testing is running the program and testing for the correct outputs "manually".

While correctness proofs have a solid argument, I feel it would be unwise to not perform execution testing just in case. I'd honestly combine the two for the best results. Make sure your solution is mathematically sound, and test for edge cases manually.

However if something can be proven to be correct, I would say that makes the correctness proof better as long as it is accurate.

#### 7. Read the article The Coming Software Apocalypse in the PDF directory. Wrote a one paragraph
appreciation of the article.

I thought the article started off as a bit of a "scare tactic", so to me that was a bit silly. As they continued they said that the software causing the issues was doing what it was told to, but the problem is what it was told to do was wrong. That right there kind of summed up the article. It's all about making software better, and not creating crappy software in the first place. Programs aren't sentient, they do exactly what we tell them too, so it is important software developers follow correct standards, and more importantly, understand the problem that they are creating a solution for. That's the main point the article was trying to convince everyone that something needs to change about how we create software, or we are going to see issues, and I think that is true.

#### 8. In regard to that article, how do you see your role in addressing the concerns raised in that article? Do you really think that there will be a “software apocalypse?”

Honestly I am chasing a path in computer science that involves security, so when it comes to software development I am focused on establishing good practices that keep things secure and accurate. I don't think there will be a "software apocalypse", that's just a "click bait" title to get people to read the article, however I do think software engineers need to be aware of the problems they are creating solutions for. Just because there won't be a "software apocalypse" doesn't mean there can't be software catastrophes. The article described quite a few that have already happened, so it is important we keep improving our methodologies and standards for the safety of everyone else as computers continue to grow and reach into various aspects of our lives.

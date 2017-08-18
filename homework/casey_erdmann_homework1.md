# Homework 01, Casey Erdmann

## 1. Answer:

- 78% of information technology organizations have been involved in disputes that ended in litigation.
- 67% of those cases, the functionality or performance of the software products as delivered did not measure up to the claims of the software developers.
- 56% of those cases, the promised delivery date slipped several times.
- 45% of those cases, the faults were so severe that the software product was unusable.

## 2. Answer:

Both the Software Life-Cycle and Software Development Cycle are concepts that have the potential to be very similar.
However, it is important to realize that they really are two completely different things.

Software Life-Cycle is a term used to describe the full "life" of the software. It's the flow of how software is made from the beginning until its end of life.

For example, a crude Software Life-Cycle might be:
  1. An idea (Birth)
  2. Research
  3. Development
  4. Initial Release
  5. Maintenance
  6. End of Support (Death)

On the other hand a Software Development Cycle is usually a part of the Life-Cycle. In our crude example it would be part of the Development and Maintenance phases.

A Software Development Cycle outlines the specific methodologies/processes that will be followed to develop software.

For example in the Spiral Development Cycle you have:
  1. Requirements Analysis
  2. Design
  3. Implementation
  4. Testing

That cycle would be followed for initial development, and then you would repeat that cycle as you maintain and update the software until it's end of life.


## 3. Answer:

#### Perfective Maintenance:

I wrote an application used to make researching quick. Anything you researched through the application could be easily cited
just by typing in your searched term into the citation generator, and picking the source you used from a list.

The app was intended to assist in writing English papers, and included a citation generator for both MLA, and APA formats.

I received some feedback from users who are in the field of Computer Science to add in functionality supporting IEEE style citations.
Although this is not the intended use for my application, I planned accordingly to add in this new feature by request of my users.

#### Adaptive Maintenance:

I run a website that is primarily a portfolio, but it does run some small back end services for a few of my applications.
Notably, the research utility application mentioned previously. I am very heavy into security, and as a result I make sure my website
and services are as secure as I can make them. A simple, yet effective way to do this is by securing you site with SSL/TLS to ensure all connections are encrypted.

However, being a poor college student, I opted for a free SSL option. This free SSL cert worked wonderfully for about 4 years.
It was signed by a widely used free certificate authority, and never gave me any issues. Unfortunately, because it was free, it became victim of abuse by illegitimate websites over the years.

Not only that, but Google was advocating for a new free SSL standard issued by Let's Encrypt. As a result, Google released a new version of Chrome that showed a security warning on any website using the same SSL
certificate that my website used. This means users visiting my site in Google Chrome would receive a scary SSL warning, and probably leave.

More importantly, this meant Android users of my research utility would not be able to access my services because the web service code using Chrome would block access to my site because of the SSL certificate.
Luckily my hosting provider had also switched to Let's Encrypt, and was offering painless upgrades to everyone using the hosting.

I had to perform some slight maintenance where services went down, but once I removed the old SSL certificates and had the new ones in place, everything was back to normal.


## 4. Answer:

While this concept isn't always true (sometimes software dies off just like hardware), the idea is accurate.
Hardware is physical, and will eventually rust, corrode, and not work anymore. Hardware in that sense is finite.

However Software does not have to end. Software can be adapted, updated, migrated, and improved, it is technically infinite if it can be maintained forever.

## 5. Answer:

It is cheaper and more effective to detect and fix issues in design or the idea itself before actually implementing it.
I think this can be true for more than just software, but there's a common saying in software development that I think
fits here pretty well that is: `"Weeks of programming can save you hours of planning".`

## 6. Answer:

Well in any form of engineering details of planning, testing, and documentation are important.
If a chemist made a new drug, and didn't test it, and a company began distributing it, that wouldn't be very safe.

It'd be even less safe if they didn't document what was in it. We can take that one step further, and say they didn't plan it, and just "eyeballed" and guessed the accurate measurements to formula.

These same things can be said about Software Engineering, but none of these things are mentioned as explicit steps.

This is because they are part of the Implementation process of a Software Engineering methodology.

You can't document code without there first being code written to document, nor can you test it.

Moreover, you shouldn't begin writing a solution without planning it. So these things aren't explicitly mentioned as steps, because they are necessary as part of implementation.

There isn't a `"set up your compiler/tools/web server/etc..."` step, but as an software engineer you should know to do those things.

If specific attributes for every section of the Software Engineering process were listed, then we would have some very long winded methodologies.

In short, these things are fundamentals in the implementation step, and therefore don't need their own phases.


## 7. Answer:

Structured programming techniques are fundamental, and arguably foundational, part of any programming paradigm.

It doesn't matter if it is functional programming, or object oriented, you are bound to rely on structured programming within the other paradigms.

For example, when building error handlers, and more complex constructors for classes you will likely rely heavily on the concept of Blocks for your conditional logic.

Video games are a great example of heavy use of object oriented programming.
Video games will rely on blocks, and subroutines to handle various things from performance, to logic for something like a quest mechanic.

So Structured programming techniques can definitely be essential in object oriented programming.


## 8. Answer:
Well it really depends on the software, but more importantly it depends on the goals.

Since the client is likely the one to set the goals I would argue it is more beneficial for the developer
to interact with the client frequently than with the users. This is because even if the goal does require interaction with users
for the software to improve, there is no way to know that unless you have interacted with the client to discuss these goals.


## 9. Answer:
I am very much into security, and one thing I could do on a fairly regular basis for the rest of my life is learning
about new vulnerabilities specific to programming languages and operating systems.

It doesn't stop there though, after learning about them, it'd be important to learn how to identify and fix them no matter what the language or operating system.

This forces me to constantly learn and improve my skills as a developer while improving the security of software I work on.


## 10. Answer:

As a developer who is familiar with open source, and maintains open source projects, I found the Cathedral and Bazaar to be fairly accurate in relation to what I have experienced.
Many of the quotes used in the essay are things I have heard all my life when it comes to writing software in general.
For example, `"To solve an interesting problem, start by finding a problem that is interesting to you"`, or perhaps my personal favorite,
`"Good programmers know what to write. Great ones know what to rewrite (and reuse)."`
These things could not be more true in my opinion, and when writing software of any kind these ideas come in handy.
What's the most interesting is how effective building software like Bazaar is as compared to a Cathedral.
It is important to notice that it is not inherently more effective than the latter, but it depends on a few things.
Things like users, and community experience, and open source code, are what makes Bazaar style building so effective.
Otherwise, if no-one uses your software, and there is no community, you might as well keep it closed source for you and your "wizards" to build the Cathedral so to speak. Regardless the essay really speaks to the benefits of open source development, and I feel it is very relatable to those who develop open source software today,
but is also insightful for those who have never entertained the idea of open source software.

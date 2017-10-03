# Homework 06, CPSC-4175
## Chapter 15, Object-Oriented and Classical Software Engineering September 25, 2017
## Casey Erdmann
#### 1. Consider the programing languages you may have studied and their differences. Think of two problem domains you would use for each language. For each problem domain, explain why your choice of the other language would be a poorer choice for an implementation language.

- C++ : C++ is a language that has stood the test of time. It can be used to run code on any operating system, and can be used to implement solutions that require access to "lower level" parts of the software. However, while it is a very powerful, portable, and useful language, one problem domain I would NOT use this in is web development. C++ is a compiled language that is best used to write tools that run locally on the end user's machine, not serve up HTML data as a webapp backend. I would use C++ to write the web-server itself, but never to write a website/webapp.

- Python : Python is a powerful language that can be used to write complex things very quickly. I personally use Python as a scripting language to do all sorts of useful things, but frameworks Django and Flask allow Python to be used as great solution for web applications. Python can run on any operating system, and is extremely useful. There really isn't much I that I would not use Python for, it can be fine tuned to a reasonable point, however if I needed extremely precise calculations, or if I need a clean proven solution of distributing software for multiple platforms, Python would not be my first choice. Although Python CAN be used for these things, it is not the best choice. With web frameworks like Ruby on Rails, Laravel for Php, and Django for Python, they are all just very similar ways to accomplish the same thing. One is not necessarily better than the other (in my opinion), they just work differently. However when it comes to writing software that needs to interact at a lower level, "closer to the metal" so to speak, Python isn't the best solution. Although it might work just fine, something like C or C++ might be a better choice.

#### 2. Give some concrete counter-examples of good programming practices as discussed in the book. These include meaningful variable names, self documenting code, symbolic constants, and code layout. In other words, give examples of what not to do.

Do Not:
- Create classes with the same name as built in language classes
- Write all your code on one line
- Name variables non-specific things
  - i.e. int num, what is num? Is it a counter, or maybe a validation check? Who knows!
- Document code with just single line descriptions.
  - i.e. //This function does some parsing and returns a string. What kind of parsing? What data am I handling, and why is it being parts?
- Only import libraries you will use. Don't import java.util.* if you're only going to use Date only import java.util.Date.

#### 3. Give two versions of coding standards for subprocedure blocks. This may require an internet search. Which do you prefer, and why?

Sub-procedures are easily confused with functions, but the distinction is important. One distinction is that functions execute sub-procedures, and in some languages that have no distinct sub-procedure definition, there are few key practices that define them as sub-procedures. One is that a sub-procedure is code that executes in a response to a call from another block of code.

When researching standards the most basic standard was what I said above:
- Sub-procedures are blocks of code that execute in response to another function call.

This is very liberal, and doesn't have many restriction on the actual block of code that is the sub-procedure.

Another standard I found has these rules:
- Sub-procedures can return 0 or more values
- Variable scope in a sub-procedure is limited to the sub-procedure
- Parameters are optional

I prefer the more liberal definition honestly, because some languages don't have built in distinct "sub-procedures/routines/calls/etc..." so being able to have a simple distinction between something like a simple recursive call and a sub-procedures goes a long way. The number of return values to me isn't important, how the code is executed however is, and the more liberal rule is a simple definition that defines that.


#### 4. An informal description of the DRY principle is this: “The second time you write exactly the same code, stop what you are doing and place that functionality in a subprocedure. Then, invoke the subprocedure whenever you need that functionality.” Give one example of this from your previous programming experience. If you have never experienced this in practice, make up an example.

A great example I have involves needing to check internet connection in a mobile app.

I developed a mobile app for a local coffee shop to take online orders, and I needed to check to see if the client using the app had there internet turned on, and was connected to the internet, and then execute logic to inform the user they needed to connect if they weren't connected.

I started to write this over and over again and checking the boolean value returned. I noticed this and quickly wrote a sub-procedure to handle this routine.

In fact from there I wanted to take more OOD approach since I used it so often, and kept adding functionality to the procedure. So, I took my procedure and made a custom Network Detection class. Creating an object using this class allowed you to detect internet connection, check if wifi is on, and even check connection to a specific server address that you pass it. This allowed me to break my procedure down into methods that handled each specific functionality. From there I just created the Network Detection object and referenced its methods where needed as if they were sub-procedures. Making this a completely decoupled class also allowed for my coworkers to use this in other apps in the future for the same purpose.



#### 5. What is a stub? What is a driver? Have you ever used stubs or drivers in your previous programming experience? If so, give an example. If not, consider a function that takes a unit price, a sales tax rate, and the quantity ordered, and write a stub (using pseudo code or a language of your choice) that takes these three arguments and returns a value.

A stub is a piece of code that emulates a called functionality.

A driver is a piece of code that emulates a piece of functionality that calls something else.

Both are used in testing, stubs are for a top down approach while drivers are for a bottom up approach.

I have not ever used these concepts so below is my psuedo code for a stub as described:

```

func saleCalc(unitPrice, salesTaxRate, quantity):

var final = unitPrice * quantity;
var tax = final * salesTaxRate;
final = tax + final;

return final;

func pricingStub(unitPrice, salesTaxRate, quantity):

var test = saleCalc(unitPrice, salesTaxRate, quantity);

var final = unitPrice * quantity;
var tax = final * salesTaxRate;
final = tax + final;

if(test == final):
  return final;

return false;

```


#### 6. List two strengths and one weakness of top down integration.

Strength:
1. Tests the code as the user experiences it directly, and will find clear flaws on the front end of things.
2. Is easy to write test for usually, because it tests in an order that makes sense in terms of development.

Weakness:
1. It won't find issues with the backend of things as easily. For example, a function may return data and pass a test, but if we aren't testing specifics about the data, it could be wrong.


#### 7. List two strengths and one weakness of bottom up integration.

Strength:
1. Easier to find problems in the core of the code because you don't move to the top until the foundation is tested.
2. It's easier to determine where the problem is if you test from the bottom, because if you're testing from the bottom and things are working, then it's a little more clear that the problem is with the top. The same can't be said for vice versa simply because you can't determine an issue exist on the bottom until you've ruled out everything on the top, which is usually more extensive and therefore not a strength.

Weakness:
1. Harder to test this way because you have to design your test to cater to the bottom end of things first, which might get in the way of designing the more complex tests as you build up.



#### 8. This is not in the book and will require some independent research. A domain specific language (DSL) is a small, incomplete language typically use as a “glue” language between a lower level language (like C) and a higher level language (like Python). An example of a DSL might be a helper language for HTML, e.g. div(...) might resolve to `<div> ...</div>`. How might a DSL promote what the book calls sandwich integration? This is not a trick question but it will require some thought. If you work as a developer, you will eventually write your own DSLs for various purposes.

Well with web applications, using HTML as the front end to display the data, you have a good example of how a DSL might promote this notion.

You can integrate backend services using whatever language, Php/Ruby/Python etc... but then you have to get data from those services, so maybe you integrate some front end service calls that send get/post requests for data from the backend services using something like JavaScript.

Well you've integrated the bottom and top, but now you need to connect the two. This is where HTML comes in handy. You can call JavaScript on an HTML page, the glue, and then once your JavaScript receives data from the service it can populate the HTML. So the HTML is the missing piece to display all the data and helps glue a front end and backend together.


#### 9. What is the difference in testing carried out by the implementation group and the testing carried out by the SQA group?

In a nutshell, the implementation group is mostly just testing to make sure everything functions.

The SQA team is more focused on everything functions CORRECTLY.

Often the dev/implementation group is focusing on the implementation, and while they will test to make sure everything is working harmoniously together, they may miss a few key bugs that they aren't looking for.

This is where SQA comes in, and actually test for core functionality, but also for security, and user experience.

#### 10. Read the letter by Edgar Dijkstra to the Communications of the ACM (in the PDF directory as dijkstra68.pdf) and write a one paragraph appreciation of this letter.

I think it is humorous to some degree that this was even a professional publication. Not because of the quality or content, but rather the subject matter. Most of the time when something is bad practice in programing, actions speak louder than words and good practice is naturally established by some very smart people. However, books *are* written to cement good practice and shine light on it, and methodologies are taught for the same reason. So in some essence, that's exactly what this is. While I never expected to read a paper about being cautious with "goto" statements, I am familiar with standard that they are bad practice basically everywhere except Assembly. So, while it may be a bit humorous to me that a publication was created about this topic specifically, it is assisting in the progress of good programming standards, and that I can definitely understand and appreciate.

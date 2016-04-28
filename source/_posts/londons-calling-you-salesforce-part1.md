title: london's calling you, salesforce
date: 2016-02-05 10:30:33
categories: events
tags:
---

{% img img-topic /images/londons-calling-banner.png %}

[London's Calling](http://www.londonscalling.net) to all the far away towns & cities of the UK for the last few months and the Salesforce community answered that call, turning up in their hundreds.

So today I have been surrounded by many of the brightest and best minds in the UK and across Europe & the Middle East too.

Here is what I discovered today in several parts:

* Part 1: Getting Agile with Salesforce & Testing
* Part 2: A career of fun & discovery
* Part 3: Lightning to the Salesforce nation

<!-- more -->

# Getting Agile with Salesforce & Testing

{% img img-topic /images/tdd-circle-of-life.png %}

There are several sessions on testing at London's calling and testing is a valuable technique in agile development.

* [Test Driven Development (TDD) in Apex & why you should be using it](http://www.londonscalling.net/sessions/test-driven-development-in-apex-and-why-you-should-be-using-it/) by [Chris Aldridge - @CAldridg3](https://twitter.com/CAldridg3)

As a developer you quickly learn that tests are an important part of writing code on the Salesforce platform, after all you need a minimum of 75% code coverage in order to deploy your code into production.  Tests are more than just a requirement, they can also help you create a good design for your code.

Using Test Driven Development (TDD) encourages a good architecture with  separation of concerns and decoupled dependencies.  Developers experienced with TDD typically spend less time debugging code as they spend less time writing those bugs in the first place.  The code tends to be shorter (easier to read) and less complex (easier to understand).

Iterative development keeps you focused on a single task at a time and stops you wasting time on all the things that could be or should be.  TDD makes it easier and safer to change your code (it is called soft-ware after all).  Instant feedback on the code that you are writing and therefore regular testing of your assumptions

When you have done a few months of the TDD approach then you will notice an unprecedented code coverage, so you never have to worry about meeting the 75% code coverage.

Sow what is test driven development (TDD)? It's more than just writing tests before writing code.  I like to think of TDD as  Chris' preferred definition is:

**"the technique of using automated unit tests to drive the design of software and force decoupling of dependencies"**

A unit test is an automated test in which the smallest testable parts of an application are individual tested.  A unit test should be:

- isoloated & independent
- one behaviour per test
- arrange (set up test data )- act (calling the method) - assert (did it do what it was supposed to)
- deterministic
- remove dependencies - too many dependencies add complexity to your testing and code
- readable

The process of test driven development is typically

1. add a test
2. run all tests; the new test should fail
3. wrote some code
4. run tests
5. new test passes
6. refactor - can I make this specific piece of code better
7. see step 1

> TDD mantra: all code is guilty until proven innocent 

Chris walked us through the TDD approach he told for a simple project, calculating if a date is a Leap year.  See the [Leap Years TDD Exercise for London's Callling on Github](https://github.com/ChrisAldridge/LondonsCalling).

Developers and engineers in almost every major programming language already getting great value from Test Driven Development, so surely its time you can also benefit from this technique.


* [Writing sustainable and maintainable Apex Tests](http://www.londonscalling.net/sessions/writing-sustainable-and-maintainable-apex-tests/) by [Simon Lawrence - @srlawr](https://twitter.com/srlawr) of [Desynit](https://twitter.com/desynit) - **1.30 Alt room**



> Also take a look at [Writing True Unit Tests using Dependency Injection and Mocking in Apex](https://adtennant.co.uk/blog/2016/01/25/writing-true-unit-tests-using-dependency-injection-mocking-apex/) by [Alex Tennant](https://twitter.com/adtennant)


* [Unit tests - they’re not just for Apex!]() by [Keir Bowden - @bobbuzard](https://twitter.com/bob_buzzard), CTO of [BrightGen]()

We are building responsive & reactive applications more and more, to meet the needs of our customers.

Wwhilst many developers are writing tests & even TDD for most languages, when it comes to JavaScript its another story.  Two big issues that affect JavaScript testing on the platform are:

- no mandate for a minimum level of test coverage
- no built in JavaScript testing on the platform (yet)

Challenges
No test context for client
- changes are not rolled back

writing testable code
- unobtrusive javascript - keep your code seperate from your HTML and CSS markup, otherwise you have to replicate this markup in orde to test

Avoid anonymous functions

functional decomposition so I can focus on the business logic
- function to decide on a ction
- function to take an action

QUnit
A generic javascript unit testing framework
use it as local files rather than CDN's
executes in the browser

qunit concepts
module is a group of tests
test is a single test
assert - confirm behaviour

sinon.js
pure javascript
spys allow you to wrap the existing functions and records executions & paramterters
stubs - spies + replace functions
mocks - stubs + expected behaviour (rarely used)

Blanket.js
code coverage for your javascript for QUnit, Mocha & jasmin (with an api for other libraries)


# Summary

London's Calling has been an amazing community driven event and I give my thanks to the organisers who spend months in the planning of this event.  Also thanks to the sponsors that helped make this possible and of course all the amazing people who spoke or attended the event.

Thank you all.
[https://twitter.com/jr0cket](John Stevenson - @jr0cket)

> London calling, yes, I was there, too.
> An' you know what they said? Well, some of it was true! 
> London calling at the top of the dial
> After all this, won't you give me a smile?
> London calling
>
> I never felt so much alike [fading] alike alike alike
>
> Copywright: The Clash, 1979


![Trailhead - Battlestations](/images/salesforce-trailhead-battlestation-banner.png)

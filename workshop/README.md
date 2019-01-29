# About Cypress.io End-To-End Testing Workshop

Until now, end-to-end testing wasn’t easy. It was the part developers hated.
Not anymore. Cypress makes setting up, writing, running and debugging tests easy.

Cypress is not a general automation framework, nor is it a unit testing framework for your back end services. There are already great tools out there that do that. Rather, we specialize in one thing - creating a great experience while you write end to end tests for your web applications.

Cypress tests anything that runs in a web browser. All of the architecture surrounding Cypress is built to handle modern JavaScript frameworks especially well. We have hundreds of projects using the latest React, Angular, Vue, Elm, etc. frameworks. Cypress also works equally well on older server rendered pages or applications.

These workshops are designed to help people get better acquainted with using Cypress for testing their frontend applications. It does not matter if that application is written in JavaScript, Angular, React, Vue or any other framework or library.

## Workshop Content

-   Chapter 1: Getting Started
    -   Using CodeSandbox for this workshop
    -   How to add Cypress to any existing project
-   Chapter 2: Basic Page Load Test
    -   Start writing your first tests using Cypress.io
-   Chapter 3: Selector Playground
    -   Not sure how to find an element on the page so that you can test its functionality? The Selector Playground makes this process much easier for you
-   Chapter 4: Resetting State
    -   Curabitur ut ex aliquam, sollicitudin sem id, luctus sapien. Nam sollicitudin, sapien id fermentum consequat, lectus justo condimentum orci, id sagittis felis mauris in ligula
-   Chapter 5: XHR Spying and Stubbing
    -   Create a functional form to adopt a dog
-   Chapter 6: CI and Cypress Dashboard
    -   Nullam rutrum enim vel pulvinar scelerisque. Vestibulum urna tortor, venenatis ac lectus at, gravida tincidunt libero. Suspendisse eget sapien lorem

---

## FAQ

**What operating systems do you support?**

You can install Cypress on Mac, Linux, and Windows.

**Do you support native mobile apps?**

Cypress will never be able to run on a native mobile app, but we do intend to support mobile web browsers in the future. Down the road we’ll likely have first class support for this, but today it is not a current priority. Cypress can test JavaScript code in hybrid mobile platforms like Ionic.
Currently our users use Cypress to control the viewport with the cy.viewport() command to test responsive, mobile views in a website or web application.

**How is this different from ‘X’ testing tool?**

The Cypress Test Runner is a hybrid application/framework/service all rolled into one. It takes a little bit of other testing tools, brings them together and improves on them.

Mocha
Mocha is a testing framework for JavaScript. Mocha gives you the it, describe, beforeEach methods. Cypress isn’t different from Mocha, it actually uses Mocha under the hood. All of your tests will be written on top of Mocha’s bdd interface.

Karma
A unit testing runner for JavaScript, Karma, works with either Jasmine, Mocha, or any other JavaScript testing framework.

Karma also watches your JavaScript files, live reloads when they change, and is also the reporter for your tests failing / passing. It runs from the command line.

Cypress essentially replaces Karma because it does all of this already and much more.

Capybara
The Ruby specific tool that allows you to write integration tests for your web application is Capybara. In the Rails world, this is the go-to tool for testing your application. It uses Sauce Labs (or another headless driver) to interact with browsers. Its API consists of commands that query for DOM elements, perform user actions, navigate around, etc.

Cypress essentially replaces Capybara because it does all of these things and much more. The difference is that instead of testing your application in a GUI-less console, you would see your application at all times. You’d never have to take a screenshot to debug because all commands instantly provide you the state of your application while they run. Upon any command failing, you’ll get a human-readable error explaining why it failed. There’s no “guessing” when debugging.

Oftentimes Capybara begins to not work as well in complex JavaScript applications. Additionally, trying to TDD your application is often difficult. You often have to resort to writing your application code first (typically manually refreshing your browser after changes) until you get it working. From there you write tests, but lose the entire value of TDD.

Protractor
Using Protractor provides a nice Promise-based interface on top of Selenium, which makes it easy to deal with asynchronous code. Protractor comes with all of the features of Capybara and essentially suffers from the same problems.

Cypress replaces Protractor because it does all of these things and much more. One major difference is that Cypress enables you to write your unit tests and integration tests in the same tool, as opposed to splitting up this work across both Karma and Protractor.

Also, Protractor is very much focused on AngularJS, whereas Cypress is designed to work with any JavaScript framework. Protractor, because it’s based on Selenium, is still pretty slow, and is prohibitive when trying to TDD your application. Cypress, on the other hand, runs at the speed your browser and application are capable of serving and rendering, there is no additional bloat.

Sauce Labs
Using Sauce Labs enables Selenium-based tests to be run across various browsers and operating systems. Additionally, they have a JavaScript Unit Testing tool that isn’t Selenium focused.

Sauce Labs also has a manual testing mode, where you can remotely control browsers in the cloud as if they were installed on your machine.

Ultimately Sauce Labs and Cypress offer very different value propositions. Sauce Labs doesn’t help you write your tests, it takes your existing tests and runs them across different browsers and aggregates the results for you.

Cypress on the other hand helps you write your tests. You would use Cypress every day, building and testing your application, and then use Sauce Labs to ensure your application works on every browser.

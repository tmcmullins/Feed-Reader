# Project Overview

In this project you are given a web-based application that reads RSS feeds. The original developer of this application clearly saw the value in testing, they've already included [Jasmine](http://jasmine.github.io/) and even started writing their first test suite! Unfortunately, they decided to move on to start their own company and we're now left with an application with an incomplete test suite. That's where you come in.


## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!


## What will I learn?

You will learn how to use Jasmine to write a number of tests against a pre-existing application. These will test the underlying business logic of the application as well as the event handling and DOM manipulation.


## How will this help my career?

* Writing effective tests requires analyzing multiple aspects of an application including the HTML, CSS and JavaScript - an extremely important skill when changing teams or joining a new company.
* Good tests give you the ability to quickly analyze whether new code breaks an existing feature within your codebase, without having to manually test all of the functionality.

# How to run this app?

Navigate to the root folder of this project and open index.html in any web browser. Allow a few seconds for all test to run. Press end to go to the bottom of the page where you can view the test results. 

# How will I complete this project?

Review the Feed Reader Testing [Project Rubric](https://review.udacity.com/#!/projects/3442558598/rubric)

1. Take the JavaScript Testing [course](https://www.udacity.com/course/ud549)
- *Reviewed the course*
***

2. Download the [required project assets](http://github.com/udacity/frontend-nanodegree-feedreader).
- *Downloaded the project*
***

3. Review the functionality of the application within your browser.
- *Tested the app*
***

4. Explore the application's HTML (**./index.html**), CSS (**./css/style.css**) and JavaScript (**./js/app.js**) to gain an understanding of how it works.
- *Explored the code*
***

5. Explore the Jasmine spec file in **./jasmine/spec/feedreader.js** and review the [Jasmine documentation](http://jasmine.github.io).
- *Explored the code and read the documentation*
***

6. Edit the `allFeeds` variable in **./js/app.js** to make the provided test fail and see how Jasmine visualizes this failure in your application.
- *Changed the allFeeds to an empty array.*
- *Test failed: Expected 0 not to be 0.*
***

7. Return the `allFeeds` variable to a passing state.
- *Changed allFeeds a populated array*
- *Test passed* 
***

8. Write a test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.
- *I used the forEach() to iterate through all items in allFeeds[].* 
- *Used the toBeDefined() matcher to check for urls* 
***

9. Write a test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.
- *I used the forEach() to iterate through all items in allFeeds[].* 
- *Used the toBeDefined() matcher to check for names* 
***

10. Write a new test suite named `"The menu"`.
- *Described a new test suite* 
***

11. Write a test that ensures the menu element is hidden by default. You'll have to analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
- *Created a variables to access the body tag as well it's className* 
- *Used .className to return a value I could use for comparison.*
- *Put test in failing state to test the test.* 
***

12. Write a test that ensures the menu changes visibility when the menu icon is clicked. This test should have two expectations: does the menu display when clicked and does it hide when clicked again.
13. Write a test suite named `"Initial Entries"`.
- *Created variable to access the body element and the menu icon* 
- *Called the trigger() to toggle the body class* 
- *Tested to see if the body element changed.* 
- *Put test in failing state to test the test.* 

***

14. Write a test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container.
- *Created variable to access the feed class DOM element.* 
- *Used beforeEach() to run loadFeed().* 
- *Used setTimeout to give the feed time to load.* 
- *Used .childElementCount on the feed class and toBeGreaterThan() for the matcher.*
- *Put test in failing state to test the test.* 
***

15. Write a test suite named `"New Feed Selection"`.
- *Described a new test suite* 

***

16. Write a test that enrsues when a new feed is loaded by the `loadFeed` function that the content actually changes.
- *Used setTimeout to give the feed time to load.*
- *Created variable in the it() to access the feed class DOM element. I have to call this after the beforeEach or else the element I'm trying to access to reference the wrong feed.* 
- *Compared the innerText against a known string to test.* 
- *Put test in failing state to test the test.* 
***

17. No test should be dependent on the results of another.
- *All test are independant.* 
***

18. Callbacks should be used to ensure that feeds are loaded before they are tested.
- *Used (done) to load feeds first.* 
***

19. Implement error handling for undefined variables and out-of-bound array access.
- *All variables are defined and there is no out-of-bound array access* 
***

20. When complete - all of your tests should pass.
- *All test passed* 
***

21. Write a README file detailing all steps required to successfully run the application. If you have added additional tests (for Udacious Test Coverage),  provide documentation for what these future features are and what the tests are checking for.
- *completed* 

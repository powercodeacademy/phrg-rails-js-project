# Build a Rails App with a jQuery Front End

## Overview

For this project, your goal is to expand upon the Rails project you did previously. The goal is to add dynamic features that are possible only through jQuery and a JSON API for your app. **Do not use `remote: true` in this application.**

## Requirements

1. Must render at least one index page (index resource - 'list of things') via jQuery and an JSON Backend. For example, in a blog domain with users and posts, you might display the index of the users posts on the users show page, fetching the posts via an AJAX GET request, with the backend rendering the posts in JSON format, and then appending the posts to the page.

2. Must render at least one show page (show resource - 'one specific thing') via jQuery and an JSON Backend. For example, in the blog domain, you might allow a user to sift through the posts by clicking a 'Next' button on the posts show page, with the next post being fetched and rendered via JQuery/AJAX.

3. The rails API must reveal at least one `has-many` relationship in the JSON that is then rendered to the page. For example, if each of those posts has many comments, you could render those comments as well on that show page.

4. Must use your Rails API and a form to create a resource and render the response without a page refresh. For example, a user might be able to add a comment to a post, and submitted via an AJAX POST request, with the response being the new object in JSON and then appending that new comment to the DOM using JavaScript (ES6 Template Literals can help out a lot with this).

5. Must translate the JSON responses into Javascript Model Objects. The Model Objects must have at least one method on the prototype. Formatters work really well for this.
Borrowing from the previous example, instead of plainly taking the JSON response of the newly created comment and appending it to the DOM, you would create a Comment prototype object and add a function to that prototype to perhaps concatenate (format) the comments authors first and last name. You would then use the object to append the comment information to the DOM.

6. Your application should conform to Nitro's Ruby linting conventions. This should already be included in your original rails project repo. Running rubocop from your application's root should return a no offenses detected message.

7. Your application should contain at least 2 model test files and at least 1 controller spec file. But the more, the better :). Each file should attempt to provide coverage over a number of public methods or endpoints in your application. Start by adding `rspec` to your `Gemfile`. Review the `Testing` section of the curriculum for some tips on best test practices. `FactoryBot` is also a gem that will need to be added to your project to use test factories. Utilize your instructor, peers, and other Nitro Developers for resources and ideas on what your application should test.

## Instructions

1. Make the changes to your existing Rails assessment repo.
1. Add the spec-js.md file from this repo to the root directory of the project, commit it to Git and push it up to GitHub.
1. Build your app. Make sure to commit early and commit often. Commit messages should be meaningful (clearly describe what you're doing in the commit) and accurate (there should be nothing in the commit that doesn't match the description in the commit message). Good rule of thumb is to commit every 3-7 mins of actual coding time. Most of your commits should have under 15 lines of code and a 2 line commit is perfectly acceptable. **This is important and you'll be graded on this**.
1. Make sure to check each box in your spec.md and explain next to each one how you've met the requirement *before* you submit your project.

### Be Prepared to:

1. Give minimal description of application, then have the reveiwer walk through it. 5 minutes.
1. Run down each item in your `spec.md` and explain how you've met each criteria. 2-5 minutes
1. Refactor code. 20-30 minutes
1. Extend the application with a new feature, more data, etc. 20-30 minutes
1. Submit an improved version.

#### Be scrappy.
- If you make a mistake, correct yourself.
- Think on your feet. We will expect you to be able to explain development concepts to us, as well as expanding on concepts that you have already implemented, but you’ll also have the opportunity to look things up during the review.

#### Make no little plans.
- Approach live coding with a constructive attitude. You might feel nervous or uncertain, but as long as you are familiar with the section material you should be able to reason your way to a solution.
- Be proud of your project and your code, and show confidence in it.

#### Radiate positivity.
- Present yourself and your project in the best way possible.
- Be open to feedback, both positive and constructive. We give feedback to help each other get better.
- If the instructor asks you to complete additional features, or you missed a project requirement, treat this as a learning experience. Becoming a developer is complex and challenging, and it’s our job to find the holes in your knowledge and help you fill them. This is to help you become a better developer, not to delay your progress in the program.

#### Work Together.
- Our goal is to give you the most thorough technical interview possible in the time allocated. This will include live coding where the instructor might give you one or two pointers, but will for the most part sit back and watch you code.
- Ask clarification questions when you need them. Asking for more details is always ok.

#### Pursue mastery.
- Use the best technical vocabulary you can. You will be expected to present yourself as a competent Rails and Javascript developer.
- Explain the details - this is your application, you should have a very thorough understanding of how each piece works.
- Curiosity and willingness to learn are hugely valued in our industry. If there are things you don’t understand, then ask questions at the end of the review for more information.

## Video Review Resources- AJAX and Rails

* [Loading Comments via GET AJAX](https://www.youtube.com/watch?v=E8TJmwW5ayQ)
* [Rails and AJAX, Submitting a Form](https://www.youtube.com/watch?v=XxzayZma5Ew)
* [Adding Form Fields via AJAX](https://www.youtube.com/watch?v=BcGtDkydAug)
* [Handlebars and JS Prototypes](https://www.youtube.com/watch?v=PT_C2211_QE)

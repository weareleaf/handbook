# The Development Handbook

## Table of Contents
- [Remember the client](#remember-the-client)
- [Projects](#projects)
- [Writing code](#writing-code)

## Remember the client

### Estimation
As a service based company, we trade our time for money. Usually, we charge an hourly rate and avoid fixed cost work, but we're only able to do this if our clients trust that our estimates are good.

If you find yourself regularly under-estimating how long things will take, it's critical that you:

 1. Communicate what's holding you up: This could be a specific, or category of things e.g. research time, test writing, rework from not having clear requirements etc.
 2. Seek help in any areas you're struggling with: Even with a few of us, we have a wide range of experience on the team.
 3. Course-correct in future estimates: If you regularly take twice as long as you estimate, start doubling your estimates.
 4. Start breaking things down and estimating in smaller chunks.
 5. Generally make a concious effort to improve: Try researching techniques and approaches - find something that works for you!

Software development estimation will always be tricky, and nobody expects you to be able to estimate _accurately_, but the impression someone gets when we take the care to give ourselves enough time, and then deliver quality work under budget is 100x better than us under estimating, and delivering work later than we said we would, and at a higher cost than we'd indicated.

The goal of estimation isn't to tell people what they want to hear, it's to give them an idea of how complex things are, and how long they will take.

### Our definition of done
At Leaf, work is "done" when we're confident we, our clients, and our client's customers will all be happy with it. Here are some things to consider before declaring work "done":

- Does it match the designs accurately?
- Does it work on supported browsers?
- Does it have suitable automated test coverage?
- Is all the code linted?
- Has the feature been code reviewed?
- Has the documentation been updated?
- Has the feature been properly tested?
- If possible, is the work viewable at a public URL?
- Have any useful update notes been written up and made available?
- Has an update been delivered back to the client?

In short, it's up to you to take ownership of your work, and ensure it's done properly.

## Projects

### Technology
We're fairly proficient in Rails, React, React Native, Node and vanilla JavaScript. While we don't have limit ourselves to these, we need to make a case internally for moving dramatically away from them. We need to consider:

 - **The impact to the project:** Will this make things take longer or cause un-necessary bugs?
 - **The impact to the team:** Will other team members be able to pick this new technology up and understand it?
 - **The impact to the client:** Will the client be able to easily find new hires of their own to continue working on this project after we're gone?

As a general guideline, we don't mind experimentation but want to keep its influence limited and get agreement from the team beforehand. Often, boring is better when it comes to technology choices.

### Github
We store all of our client projects in Github. We keep `staging` as our base branch, and we reserve the `master` branch for live deployments.

With our Heroku setup detailed below in the hosting section, when code is changed in the `staging` branch, it is automatically deployed to the Staging environment, and when `staging` (or any other branch) is merged to `master`, the `master` branch is automatically deployed to the production environment.

This means the `master` branch is always an accurate reflection of what's running in production, and gives us a place to commit emergency bug-fixes if the `staging` branch has work in it that's being tested but isn't ready to deploy.

### Code review
We use pull requests and code reviews for new changes unless we're sure they're not necessary (typo fixes, config changes, etc). These promote knowledge sharing, improve code quality, and reduce our [bus factor](https://en.wikipedia.org/wiki/Bus_factor).

**A note on pull request size:** When developing, we should focus on keeping pull requests small. Smaller pull requests where every code change is in persuit of the same goal are much easier to review than huge ones that change all sorts of things. If you have 5 bugs to fix, raising a pull request for each bug could be an example of this. Generally, however, just consider how you can chunk work down to make code review easier for others.

### Continuous integration
We set up CI on all of our projects, and on all branches. CI should run all of the project tests and linting, and either block deployments or fail pull requests on Github if it doesn't pass. We should consider using [Heroku CI](https://devcenter.heroku.com/articles/heroku-ci) for this if we're deploying to Heroju, but failing that, we've had success with [CircleCI](https://circleci.com) in the past.

### Hosting
Unless a client has other hosting arranged, we host most of our projects on [Heroku](http://heroku.com), setting up an [Organisation](https://devcenter.heroku.com/articles/org-users-access) for each client, and using a [Pipeline](https://devcenter.heroku.com/articles/pipelines) to create a staging environment linked to the `staging` branch on Github, and a production environment linked to the `master` branch on Github.


## Writing code

### Developer experience
In order to work efficiently, we need to keep our projects hassle-free to work with. This is "developer experience". Signs of good developer experience on a project include:

 - A setup process that a newbie can follow
 - Tests that are easy to run, and pass consistently (when the code is working)
 - Appropriate documentation for anything that might be unclear or confusing to use.
 - Useful error messages when things break

These are just some indicators, but there are many. In general though, good developer experience means low frustration and more time spent writing code.

### Testing
We write automated tests on all our software projects. We recognise that like other code tests aren't free to write or maintain, so we try to test pragmatically, putting more importance on feature tests that check things work properly from a user perspective and giving the application a wide amount of coverage in the process, than unit tests which check individual lines of code work as intended.

Both have their place, so if in doubt ask and read up on different styles of testing, form an opinion of your own and discuss it with the team.

### Style
Specific linting rules can be discussed/agreed upon on a per-project basis, but we should be using some sort of automated linting on our code, it catches loads of easy to make mistakes, and saves helps to keep things readable and consistent.

Some good solutions for this are [Rubocop](https://github.com/rubocop-hq/rubocop) for ruby projects and [StandardJS](https://standardjs.com) for JavaScript.

### Config
As much as possible, config should be stored in the environment, not in application code itself. This keeps the app portable between different environments and easy to reconfigure for a CI, Staging or Live environment without needing to make any code changes. If in doubt, ask for examples of this in action.

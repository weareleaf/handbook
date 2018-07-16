# Handbook
Our handbook is where we try to share how we work as a company, and what we expect from each other and our projects, without getting prescriptive, or using patronising legal language.

If you're reading this for the first time, take note, question things and offer feedback where necessary.


## Projects

### Technology

We're fairly proficient in Rails, React, React Native, Node and vanilla JavaScript. While we don't have limit ourselves to these, we need to make a case internally for moving dramatically away from them. We need to consider:

 - **The impact to the project:** Will this make things take longer or cause un-necessary bugs?
 - **The impact to the team:** Will other team members be able to pick this new technology up and understand it?
 - **The impact to the client:** Will the client be able to easily find new hires of their own to continue working on this project after we're gone?

As a general guideline, we don't mind experimentation but want to keep its influence limited and get agreement from the team beforehand.

### Github
We store all of our client projects in Github. Where we keep `staging` as our base branch. We reserve the `master` branch for live deployments.

With our Heroku setup detailed below in the hosting section, when code is changed in the `staging` branch, it is automatically deployed to the staging environment, and when `staging` (or any other branch) is merged to `master`, the `master` branch is automatically deployed to the production environment.


### Pull requests & code review
We use pull requests and code reviews for new changes unless we're sure they're not necessary (typo fixes, config changes, etc). These promotes knowledge sharing, improves code quality, and reduces our [bus factor](https://en.wikipedia.org/wiki/Bus_factor).

**A note on pull request size:** When developing, we should focus on keeping pull requests small. Smaller pull requests where every code change is in persuit of the same goal are much easier to review than huge ones that change all sorts. If you have 5 bugs to fix, raise a pull request for each, but generally just consider how you might chunk work down to make it easier on the reviewer.

### Continuous integration (CI)
We set up CI on all of our projects, and on all branches. CI should run all of the project tests and linting, and either block deployments or fail pull requests on Github if it doesn't pass. We should consider using [Heroku CI](https://devcenter.heroku.com/articles/heroku-ci) for this, but failing that, we've had success with [CircleCI](https://circleci.com) in the past.

### Hosting
Unless a client has other hosting arranged, we host most of our projects on [Heroku](http://heroku.com), setting up an [Organisation](https://devcenter.heroku.com/articles/org-users-access) for each client, and using a [Pipeline](https://devcenter.heroku.com/articles/pipelines) to create a staging environment linked to the `staging` branch on Github, and a production environment linked to the `master` branch on Github.


## Writing code

### Testing
We write automated tests on all our software projects, period. We recognise that like other code tests aren't free to write or maintain, so we try to test pragmatically, putting more importance on feature tests that check things work properly from a user perspective and giving the application a wide amount of coverage in the process, than unit tests which check individual lines of code work as intended.

Both have their place, so if in doubt ask and read up on different styles of testing, form an opinion of your own and discuss it with the team.


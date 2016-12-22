# MentorBuddy

One Paragraph of project description goes here

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Assuming you have 64-bit Windows

### Installing

A step by step series of examples that tell you have to get a development env running

Install rails from [Here](https://s3.amazonaws.com/railsinstaller/Windows/railsinstaller-3.2.0.exe)

1. Install rails from [Here](https://s3.amazonaws.com/railsinstaller/Windows/railsinstaller-3.2.0.exe)
2. Install Heroku Toolbelt from [Here](https://cli-assets.heroku.com/branches/stable/heroku-windows-amd64.exe)
3. Ensure you have your favourite text editor installed.

At this point you should have all the necessary software installed
```
$ gem update --system 2.1.9
```

## Understanding the workflow

* You have two branches that always exist, master and develop.
* master represents the most stable version of your project and you only ever deploy to production from this branch.
* develop contains changes that are in progress and may not necessarily be ready for production.
* From the develop branch, you create topic branches to work on individual features and fixes.
* Once your feature/fix is ready to go, you merge it into develop, at which point you can test how it interacts with other topic branches that your coworkers have merged in.
* Once develop is in a stable state, merge it into master. It should always be safe to deploy to production from master.

Step by step, your workflow under this model might look like this:

1. You need to fix a bug.
2. Create a branch called myfix that is based on the develop branch.
3. Work on the bug in this topic branch until it is fixed.
4. Merge myfix into develop. Run tests.
5. You discover your fix conflicts with another topic branch hisfix that your coworker merged into develop while you were working on your fix.
6. Make more changes in the myfix branch to deal with these conflicts.
7. Merge myfix into develop and run tests again.
8. Everything works fine. Merge develop into master.
9. Deploy to production from master any time, because you know it's stable.

See https://vireshdhawan.github.io/DBATCPresentation for additional steps

## First-time system setup

```
$ git config --global user.name "Your Name"
$ git config --global user.email your.email@example.com
```
```
$ git clone https://github.com/mentorbuddy/mbProject.git
```
## Branch, Edit, Commit, Merge
```
$ git checkout -b topic-branch
$ <Make your Changes Now>
$ git add .
$ git commit -a -m "Your Message Here"
$ git merge topic-branch
$ git checkout master
$ git branch -d topic-branch
```
Unlike the -d flag, the -D flag will delete the branch even though we haven’t merged in the changes.

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Ruby on Rails](http://rubyonrails.org/) - The web framework used

## Authors

* **Viresh Dhawan** - *Initial work* - [Viresh Dhawan](https://github.com/VireshDhawan)

See also the list of [contributors](https://github.com/mentorbuddy/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc

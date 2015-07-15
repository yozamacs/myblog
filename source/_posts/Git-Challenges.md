title: "Git Challenges"
date: 2015-05-13 18:12:28
tags:
- Git
---
I really haven’t been familiar with Git outside of its basic push and pull —rebase functionality. Today, I wanted to have the website in working condition. I have been trying to figure out how to use the links so that you don’t have to specify their path in the project. I have an example project with this functionality, but I’m not sure about how to replicate that.

In the meantime, I wanted to check out a working version of the project from about 10 commits prior. I could have just reverted the 10 commits, but I thought you should be able to just check out a previous version and go from there. I tried to make a branch, which worked, but I couldn’t figure out how to go from that branch to heroku master. I would try to pull from heroku master and then it would wipe out the changes that I wanted for my working version branch.

After searching all of the webpages, I finally found what I wanted, which was a reset hard and the push hard to origin. The stack overflow is [here](http://stackoverflow.com/questions/17667023/git-how-to-reset-origin-master-to-a-commit). I’m not sure if that was the best solution. It was okay for a personal project, but in a large project, force pushing would probably cause a lot of issues. What was puzzling me was how to manually merge the checked out branch with master and then push that to the remote heroku branch. Definitely needs more investigation.

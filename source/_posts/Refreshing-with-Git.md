title: "Refreshing with Git"
date: 2015-05-13 18:13:06
tags:
- Git
- tutorials
---

Version control is so important for software development, and it never hurts to make sure you have a great foundation. As a refresher of the basics, I did the really popular command line git tutorial. I have a finished [certificate](http://jlord.us/patchwork/) and everything. The tutorial was really helpful, and I look forward to creating a helpful tutorial one day.

Even though I’m familiar with how to use git, some of the more complicated cases still elude me. The other day we pushed a commit and merged, but then we reverted the merge. However, we wanted the code from the revert to be on a local branch. When we reverted the revert on our local machine, the changes were there, but the created files were not. After trying to just check out the commit that we created, which didn’t work, we ended up using the IDE to restore our missing files.

Knowing how to handle the tricky situations can’t really be learned in a tutorial. The next time that I come to a situation like that I will try to figure how to solve it from the command line.

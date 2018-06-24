# Github

Github is great place to share your code with other people. It's the perfect place to have your code on in a group project.

## Meesterproef project

Before the Meesterproef project, I used to drag my files to my directory on the Github website like a complete pleb. During the project I had to get used to the command line way of using Github, because of the large amount of code synchronizing we had to do.

## Starting off

One of us made a repository on Github and invited the rest of the team. The first thing you do is 'clone' your repository. That means you have a local copy of the files. You can work with those files in your local code editor.

## The command line interface

Open up your CLI of chose and navigate to the location where you copied the Github repository to. Use `cd \*yourmaplocationhere*` to do so.

## Creating branches

Now that you navigated to the location your copied your repository to, you can start off. In my project group's case, we created a branch for every different or new thing we started on. You can create a branch like so: `git checkout -b *your-branch-name-here*`. In my case it was quite important to spar about the branch name with one of my groupmates to keep the naming consistent.

## Pushing and pulling

After you are done with your first piece of code, you need to push it Github. Before you can push, though, you need to commit the changes made to the file. Like so: `git add .` to add all the changes to the commit, `git commit -am *yourcommitmessagehere*` to commit the changes you added before. After committing the changes you still need to push
the changes to Github. This is real simple: `git push`.

If you are working in group project, you will want to have the latest code at all times. It's real handy to synchronize often. You can type `git pull` in your terminal to pull all changes made on the branch. If you want to make sure you pull all the changes from the master branch, you can type `git pull origin master` aswell.

## Pull request

After you are done with your branch, you want everybody in your project group to see your awesome code. You can do so with a pull request. This is essentially a request to merge your branch with the main source, the master branch. This is best done on the Github site. You can click the green button that screams at you to make a request to do so. Make sure there are no conflicts in the code and merge the branch to the master!

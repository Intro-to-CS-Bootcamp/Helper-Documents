# Helper Document - GitHub


How does it work?
The way that GitHub works is that you have two versions of your code, the remote and the local. The remote is the code visible on GitHub to whomever has access to the repository, so that's the code that we'll be seeing and grading. The local is the code on your computer as you work on it.
So whenever you have a project on GitHub you will work on it on the local copy, and when you finish a task, you'll add it, commit, and push to the remote. This serves to share it with whomever you're collaborating with, and give you access to versioned back-ups. The second is particularly important as it means that if things break, you can use your commit log to find the last point things worked and see exactly what the changes made after that were so you can find the bug.



Before anything else, make your account:
![alt text]( "Create account")


Go to github.com, and make your account. Once you’re in, go to your profile by clicking on the icon at the top right and then on ‘Your Profile’:

Then click on ‘My repositories’ and then ‘New’


Name it something along the lines of ‘ics-bootcamp’, make sure it’s public, and initialize with a README:


Your repo should now look something like this, and be ready for cloning:

Cloning:

Now, open your terminal (you can find it in the Launchpad or using the Spotlight), or GitBash if on Windows.

Create a general folder to store all your coding classes/projects under (mine is called ‘dev’) using the `mkdir` or ‘make directory’ command.

Then move into it using the ‘cd’, or ‘change directory’, command. 

Use the command ‘ls’ to list everything within, here I’m just using it to show the difference once we clone our repository (yours should be empty, mine has stuff in it because it’s an old directory).

Then get the cloning url from your repository as shown here:




And clone the remote to your local with the command `git clone <url>`

Then use `ls` to see that it’s now under the directory



Pushing work to the remote.
Now, we start by moving into the repository using `cd`

And running `git status`

Note that it says we’re up-to-date, and have nothing to commit. 

We’re now going to create a file using the `touch` command so we can go through the process of pushing to the remote. During the course, you’ll be creating files for the actual assignments of course.

Also used `ls`, and we can see that the file is now there. If we run `git status` again…

We can see that there’s now an untracked file ‘dummy.txt’.

We can now run `git add dummy.txt` to add it to the staging area: the work that we want git to keep track of for our next commit.

A `git status` after that now shows ‘dummy.txt’ in the ‘changes to be committed’ section.

For the actual committing, there’s two options. You can run `git commit -m “<commit message>”` to automatically create the full commit like so:

Or do the full commit by typing `git commit`

Which will open the default text editor (vi on mac, emacs or vim on windows depending on your choice during the setup for GitBash).



On vi (or vim, they work the same way on basic terms), you type `i` to start editing, write your message, then click the `ESC` key to exit editing mode, and type `:wq` for ‘write and quit’. A final enter and you’ll be done!

For emacs, you can just start typing. When done, click Control-X and Control-C, then type ‘y’ to save and exit.

Either way, you’ll end up here:








A quick `git status` shows that you’re ahead of ‘origin/master’ by one commit (I’m ahead two because I did both types of commits).







As a final step, you do a `git push`, type in your username and password, and you’re done!


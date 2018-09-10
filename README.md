# { Git Basics Exercises. }

Now that you have learned the basics of Git workflow, try running through this a couple of times on your own:

1. Create a folder called learn_git_again.

 * mkdir learn_git_again

3. cd into the learn_git_again folder.

 * cd learn_git_again

5. Create a file called third.txt.

 * touch third.txt

7. Initialize an empty git repository.

 * git init

9. Add third.txt to the staging area.

 * git add .

11. Commit with the message "adding third.txt".

 * git commit -m “adding third.txt”

13. Check out your commit with git log.

  * git log

15. Create another file called fourth.txt.

 * touch fourth.txt

17. Add fourth.txt to the staging area.

 * git add .

19. Commit with the message "adding fourth.txt"

 * git commit -m “adding fourth.txt”

21. Remove the third.txt file

 * rm third.txt

23. Add this change to the staging area

 * git add .

25. Commit with the message "removing third.txt"

 * git commit -m “removing third.txt”

27. Check out your commits using git log 

 * git log

29. Change your global setting to core.pager=cat 

 * git config --global core.pager “cat”

31. Write the command to list all of the global configurations for git on your machine. You can type git config --global to find out how to do this

 * git config --global --list

# { Branching and Merging Exercises. }

### Part I

Answer the following questions:

1. What does git clean do?

 * It removes files that have not been staged yet

3. What do the -d and -f flags for git clean do?

 * It removes untracked directories and untracked files

5. What git command creates a branch?

 * git checkout -b

7. What is the difference between a fast-forward and recursive merge?

 * A fast forward merge happens when changes are being made to a branch while the master branch is not being edited.  A recursive merge happens when the two branches being merged have both been worked on since the branch was made

9. What git command changes to another branch?

 * git checkout

11. How do you remove modified or deleted files from the working directory?

 * git checkout

13 What git command deletes a branch?

 * git branch -D

15. What does the git diff command do?

 * Shows you the difference between two commits

17. How do you remove files from the staging area?

 * git reset HEAD or git rm --cached

18. How do merge conflicts happen?

 * When changes from two branches have been made to the same file, trying to merge these branches can result in a merge conflict, as git is not sure which version of the file we should be using.  

### Part II

Create your own merge conflict! Work on the same file on two separate branches and merge the two branches together. Fix the conflicts and finish your merge. In the real world you will never intentionally try to create merge conflicts, but it is important to understand how and why they are created. Most importantly, it's important not to be intimidated by merge conflicts, and to be able to fix them with confidence!

* Done

# { GitHub Exercises. }

### Part I

Let's start by taking a bit of time to practice the git workflow below. It is so valuable to just practice this workflow a couple times, since you will most likely doing it professionally as well as in your individual projects and open source contributions. Here are some things to do.

1. Create a local repository and add and commit some files

   1. mkdir github_exercise && cd github_exercise
   2. git init
   3. touch first.txt
   4. git add .
   5. git commit -m “first commit”
   6. touch second.txt
   7. git add .
   8. git commit -m “second commit”

2. Create a remote repository and push your code from the local repo to the remote

   1. Go to: <https://github.com/new> and new create repo called “github_exercise”
   2. git remote add origin git@github.com:PrismaPhonic/github_exercise.git
   3. git push -u origin master

3. Fork the repo[ https://github.com/rithmschool/git_practice](https://github.com/rithmschool/git_practice) - clone it and submit a pull request

   1. Go on the page and choose “fork”
   2. git clone git@github.com:PrismaPhonic/git_practice.git
   3. Submit pull request

4. Create a new branch locally and push it to GitHub

   1. git checkout -b awesomechanges
   2. echo “totally awesome” > awesomechanges.txt
   3. git add .
   4. git commit -m “totally awesome commit”
   5. git push -u origin awesomechanges

5. Submit a pull request with your new branch against the master branch on the git_practice repo.

   1. Did this through the website

### Part II - Command Line Murder Mystery

If you have gone through our Terminal and UNIX course, take the time to combine your knowledge of the Terminal, Git, and GitHub to complete a murder mystery! You can find the exercises[ here](https://github.com/veltman/clmystery). Fork and clone the repository and try to solve the mystery!

    Solved: Jeromy Bowers!
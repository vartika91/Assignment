# Assignment
1. What are the advantages of using Git?
-Able to merge all the source codes written by multiple people in the team. It does source code management
-Maintaining all the versions saved by multiple people.
-It is a distributed version control system used for tracking changes in computer file.
-Git supports all the files. (programmers can write code in any language C, PHP, Java, Python)
2. What language is used in Git?
Programmers can write in any language like C, PHP, Java, Python etc.
3. What is the meaning of “Index” or “Staging Area” in Git?
The Git index is used as a staging area between your working directory and your repository. You can use the index to build up a set of changes that you want to commit together. When you create a commit, what is committed is what is currently in the index, not what is in your working directory.
4. What is the process for creating a repository in Git?
Step 1: Create an account on Github
Step 2: Click on Repository
Step 3: Click New → Give repository a name under Repository Name field → Description → Check box “Public” → Check box “Initialize this repository with a README”
Step 4: Click Create Repository 
5. What is ‘head’ in Git and how many heads can be created in a repository?
By default, there is a head in every repository called master. HEAD is the another word for current branch. There can be any number of heads in a GIT repository.
6. Why do we need branching in Git? 
Branches serve as an abstraction for the edit/stage/commit process. You can think of them as a way to request a brand new working directory, staging area, and project history. New commits are recorded in the history for the current branch, which results in a fork in the history of the project.
7. Write a way to create a new branch in Git?
You can also use the git checkout -b <branch-name> <hash> syntax, which will create the branch and check it out, all in one command.
8. How do you define a ‘conflict’ in Git?
A conflict arises when two separate branches have made edits to the same line in a file, or when a file has been deleted in one branch but edited in the other.
9. How to resolve a conflict in Git?
Open Terminal.
Navigate into the local Git repository that has the merge conflict.
Generate a list of the files affected by the merge conflict. In this example, the file README.md has a merge conflict.
Open your favorite text editor, such as Atom, and navigate to the file that has merge conflicts.
Decide if you want keep the removed file. You may want to view the latest changes made to the removed file in your text editor.
Commit your changes with a comment.
10. What is the function of ‘git config’?
The git config command is a convenience function that is used to set Git configuration values on a global or local project level. These configuration levels correspond to Git config text files. Executing git config will modify a configuration text file.
11. What is Git fork?
A fork is a copy of a repository. Forking a repository allows you to freely experiment with changes without affecting the original project. Most commonly, forks are used to either propose changes to someone else's project or to use someone else's project as a starting point for your own idea.
12. Difference between fork, branch and clone?
Difference between fork and clone: When you fork a repository, you create a copy of the original repository (upstream repository) but the repository remains on your GitHub account. Whereas, when you clone a repository, the repository is copied on to your local machine with the help of Git.
Difference between fork and branch: When you fork a repository, you're creating your own copy of the entire project including the repository. A branch is simply a separate set of commits within a repository that already exists. Forking is something you'll typically do once when you start working on the project.
13. What's the difference between a "pull request" and a "branch"?
A branch is just a separate version of the code. A pull request is when someone take the repository, makes their own branch, does some changes, then tries to merge that branch in (put their changes in the other person's code repository).
14. What is the difference between "git pull" and "git fetch"?
Git fetch really only downloads new data from a remote repository but it doesn't integrate any of this new data into your working files. Fetch is great for getting a fresh view on all the things that happened in a remote repository.
Git pull, in contrast, is used with a different goal in mind: to update your current HEAD branch with the latest changes from the remote server. This means that pull not only downloads new data; it also directly integrates it into your current working copy files.
15. How to revert previous commit in Git?
Use the commit hash that you get from the git log command: git revert <commit hash>
This command will create a new commit with the “Revert” word in the beginning of the message. After this, if you check your repository status, you’ll notice that you have the HEAD detached at the commit you tested before.
16. Explain the advantages of Forking Workflow
1. The Forking Workflow is fundamentally different than other popular Git workflows. Instead of using a single server-side repository to act as the “central” codebase, it gives every developer their own server-side repository. This means that each contributor has not one, but two Git repositories: a private local one and a public server-side one. The Forking Workflow is most often seen in public open source projects.
2. The main advantage of the Forking Workflow is that contributions can be integrated without the need for everybody to push to a single central repository.
3. The Forking Workflow typically follows a branching model based on the Gitflow Workflow. This means that complete feature branches will be purposed for merge into the original project maintainer's repository.
4. The result is a distributed workflow that provides a flexible way for large teams to collaborate securely. This also makes it an ideal workflow for open source projects.
17. Difference between HEAD, working tree and index, in Git?
Working trees: They are nothing but the files that you are currently working on.
HEAD: is a pointer to the branch or commit that you last checked out, and which will be the parent of a new commit if you make it. For example, if you're on the master branch, then HEAD will be pointing to master, and when you commit, that new commit will be a descendant of the revision that your master pointed to, and master will be updated to point to the new commit.
Index: The git "index" is where you place files you want commit to the git repository. The index is a staging area where the new commit is prepared. Essentially, the contents of the index are what will go into the new commit. The command git add will add or update files from the working tree into your index.
18. How to identify if a certain branch has been merged into master?
The -a flag will show both local and remote branches, and the -r flag shows only the remote branches. You can use the git merge-base command to find he latest common commit between the two branches. If that commit is the same as your branch head, then the branch has been completely merged.
19. What is the use of a Git clone?
Git clone is primarily used to point to an existing repository and make a clone or copy of that repository at in a new directory, at another location. The original repository can be located on the local file system or on remote machine accessible supported protocols. The git clone command copies an existing Git repository.
20. What is Git stash?
Git stash temporarily shelves (or stashes) changes you've made to your working copy so you can work on something else, and then come back and re-apply them later on. Stashing is handy if you need to quickly switch context and work on something else, but you're mid-way through a code change and aren't quite ready to commit.
21. When should I use "git stash"?
Use git stash when you want to record the current state of the working directory and the index, but want to go back to a clean working directory. The command saves your local modifications away and reverts the working directory to match the HEAD commit.
22. What is Git stash drop?
In case we do not need a specific stash, we use git stash drop command to remove it from the list of stashes. By default, this command removes to latest added stash. To remove a specific stash we specify as argument in the git stash drop <stashname> command.
23. What is Git stash save?
The git stash command takes your uncommitted changes (both staged and unstaged), saves them away for later use, and then reverts them from your working copy.
24. What README.MD ? What is its purpose? What does MD stands for?
A README file contains information about other files in a directory or archive of computer software. A form of documentation, it is usually a simple plain text file called READ.ME , README. TXT , README.md (for a text file using markdown markup),MD stands for markdown.
25. How to create repository from command prompt?
Done in five steps:
Step1: Go into the directory containing the project.
Step2: Type git init .
STep3: Type git add to add all of the relevant files.
Step4: You'll probably want to create a . gitignore file right away, to indicate all of the files you don't want to track. Use git add . gitignore , too.
Step5: Type git commit .
26. What is the function of ‘git checkout’ in Git?
The git checkout command lets you navigate between the branches created by git branch . Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.
27. How can you bring a new feature in the main branch?
First we run git checkout master to change the active branch back to master. Then we run the command git merge new-branch to merge the new feature into the master branch. Note that git merge merges the specified branch into the currently active branch. 
28. What is the function of ‘git rm’?
The git rm command can be used to remove individual files or a collection of files. The primary function of git rm is to remove tracked files from the Git index. Additionally, git rm can be used to remove files from both the staging index and the working directory.
29. What is the function of ‘git stash apply’?
30. What is the use of ‘git log’?
The most basic and powerful tool to do this is the git log command. By default, with no arguments, git log lists the commits made in that repository in reverse chronological order; that is, the most recent commits show up first.
31. What is ‘git add’ is used for?
The git add command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. However, git add doesn't really affect the repository in any significant way—changes are not actually recorded until you run git commit .
32. What is 'git diff' is used for?
Diff command is used in git to track the difference between the changes made on a file. Since Git is a version control system, tracking changes are something very vital to it. Diff command takes two inputs and reflects the differences between them. It is not necessary that these inputs are files only.
33. What is ‘git status’ is used for?
The git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven't, and which files aren't being tracked by Git. Status output does not show you any information regarding the committed project history.
34. Can we create multiple branch with one command?
Git offer a feature referred to as a worktree, and what it does is allow you to have multiple branches running at the same time. It does this by creating a new directory for you with a copy of your git repository that is synced between the two directories where they are stored. 
35. what is the command that is used to delete a branch?
If you are sure you want to delete it, run 'git branch-D my-branch' . This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.
36. What is another option for merging in git?
Using the "git merge" command is probably the easiest way to integrate changes from one branch into another. However, it's not your only option: "git rebase" offers another, slightly different way of integration.
37. How to remove a file from git without removing it from your file system?
38. Use of "git rebase" instead of "git merge"?
Using the "git merge" command is probably the easiest way to integrate changes from one branch into another. However, it's not your only option: "git rebase" offers another, slightly different way of integration.
39. What is a repository in Git?
Git repository is just a file location where you are storing all the files related to your project. When you git commit your code, a version/snapshot is created in your local repo. Remote repository: A remote repository generally lies somewhere outside your system, on a remote machine.
40. Command used to write a commit message?
You can use commit in multiple ways to commit changes to your repository, but every commit requires a log message. You can add a message by adding -m "your message".
41. What does commit object contain?
Commit: A commit object contains the reference to another tree object and some other information(author, committer etc.) tag — A tag or a tag object is just another reference to a commit object and just makes for easier referencing.
42. Write one use-case of Github?
43. Name some alternative of Git?
Bitbucket, GitLab, Mercurial, Perforce, C.
44. What is a gist in Git?
Gist is an easy method to share snippets or excerpts of data with others. A gist can be a string of code, a bash script or some other small piece of data. These bits of information are hosted by GitHub as a repository.
45. What is a gist programming?
46. Name any two Git repository hosting services which are common?
GitLab and Bitbucket

### Answer the following questions in you own words.

> It's not necessary that you havee to know and answer all the questions. Just answer the ones
> you know and write in your own words.

1. Give the difference between the remotes - upstream and origin - with an example.

You answer: Upstream is the original repository which is forked and orgin is the own copy of the repository.
* Ex: https://github.com/whilstsomebody/GDG-FOSS-WING-SELECTION-2025 This is the UPSTREAM.(original repo)
* https://github.com/Lochit-Vinay/GDG-FOSS-WING-SELECTION-2025 This is the ORIGIN.(copy of repo)

2. You have two branches A and B and you have currently made some changes in branch A.
You want to move into branch B but do not want to commit the current changes in branch A.
What will you do?

You answer: I'll use git switch B command.

3. You were assigned a work to implement a feature and create a PR to your organization's remote repository.
For this you made a branch (say A) and made some changes and commited them. Now you moved to some other branch 
(say B) to do some other assigned work. But later you realisd that have to complete the task assigned earlier 
first and commited some changes in branch B which are meant for branch A. How will you use git to bring the 
changes from branch B to branch A?

You answer:I'll use git cherry pick command which specifies a specific commit which applies to other without merging with other.
firstly I'll check the history of the branch by using git checkout and git log -- oneline I'll make the possible changes which are required previously then I'll switch to branch A by using git checkout A, then cherry pick the commit and at last I'll git push origin A.

3. What is the difference between fetching changes and pulling changes?

Your answer: Fetching changes:Downloads commits, branches, and files from the remote repository but doesn’t update the local branch automatically it is a fast process, where as pulling changes refers to which downloads commits and then it immediately merges them in the current or existing branch and it is a slight slow process.

4. What does -i flag stand for? What is it's significance in git?

You answer:-i stands for interaction,it is used for seeing the git menu.

5. You are working in an organization that follows very strict guidelines for PRs and commits.
You made three commits in your PR and the maintainer says you were supposed to make a single commit.
What will you do in this case?

You answer:

6. Explain `git merge` and `git rebase` with example(s).

You answer: 
* Git merge is used to Combine two branches by creating a merge commit.
* Git rebase is used to Reapply commits of one branch on top of another.

7. Write the flow how you create a repository and push changes to it. Also mention the commands used at each step.

You answer: 
* Firstly I'll go to my github profile and I'll click on new repository,I'll create a new repository by giving a name to it then I'll copy the repo link.
* Then I'll come back to my file on which I have made changes which I wanted to push.
*  I'll open the terminal line for pushing the file to the repository.(git init used for initializing)
*  I'll use git remote add origin <my url link>
*  git remote -v (which is used for verification of remote)
*  I'll check the branch by git branch
*  If I want to rename the branch then git branch -M -branch name
*  git add . to save the changes made 
*  git commit -m "initial commit"
*  Then I'll get the options whether to pull or push then we need to give the command git push origin main(given branch name)


8. How would you prevent a file or folder from getting tracked by git?

Your answer: I'll create a .gitignore file and then I'll store the essential or required info.

9. You did not implement the step you mentioned in question 8 and now you have committed and pushed your database's
secret key to the github. How will you remove the key from your git's commit history to avoid any misuse?

You answer: I'll remove the entire file from the Git History by using git filter-repo command.

---
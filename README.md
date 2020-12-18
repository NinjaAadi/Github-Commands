<h1> Git Commands and their description</h1>

<p>Initialize git in your local repository</p>

```c
git init
```
<h2>What is a staging area?</h2>
<p>Staging Area is the area where you add files so that git can track it before making any commits</p>
<p>Command to add files to the staging area:</p>


```c
git add filename
```
To add all the files for staging

```c
git add .
```

<p>Remove from staging</p>

```c
git rm --cached ["filename"]
```
<h2>What is a commit?</h2>
<p>A commit is a change that is made and saved to your local git repository.</p>

```c
git commit -m ["Commit message"]
```
<h2>What is a push?</h2>
<p>Pushing is storing the local commits to the remote repository in Github.</p>

```c
git push
```
<h2>Git status</h2>
<p>Git status shows the status of the tracked files in your repository</p>

```c
git status
```

<h2> Cloning a repository</h2>

```c
git clone repository-link
```

<h2>Git difference</h2>
<p>Git diff is used to track the changes that are made in your files</p>

```c
git diff
```
<h2>What is fork?</h2>
<p>When you fork a repository, you make a copy of that repository in your Github account.Now you can clone the repository to your local workbase to work on it.</p>
<br/>

<p>Adding remote name to your repository so that other commands can be executed with ease.In this case the name is origin</p>

```c
git remote add origin 
```
<h2>Who are collaborators?</h2>
<p>Collaborator are persons who you give permissions to make change to your own repository.</p>

<h2>Branching</h2>
<p>Branching means to create a copy of the orgin of the repository such that you can modify the code without effecting the original code. If the branch code is successfull you can merge the two branches which will update the changes made to the main branch. This is the coolest feature of github</p>

<h3>Branching and Merging Commands</h3>
<ul>
<li>Show all the branches of local repository

```c
git branch
```

<li>Show all the branches of the remote repository.</li>

```c
git branch -a
```
<li>Create a new branch</li>

```c
git branch [Branch name]
```

<li>Delete a branch</li>

```c
git branch -d ["branch Name"]
```
<li>Create a branch and switch to it</li>

```c
git checkout -b ["branch name"]
```
<li>Rename a local branch</li>

```c
git branch -m ["old branch name"] ["new branch name"]
```
<li>Switch to a branch</li>

```c
git checkout ["branch name"]	
```
<li>Merge a branch to the current branch</li>

```c
git merge ["branch name"]
```
<li>Merge two branches</li>

```c
git merge ["branch name 1"] ["branch name 2"]
```
</ul>

<h2>All about stashing</h2>
<p>After commiting some changes you modify some files. Now you want to temporarily remove the changes to see the last commit. So you save the changes to stash.After viewing we can get back the changes saved in the strash</p>
<br/>
<p>Command to stash the changes</p>

```c
git stash
```
<p>Now after viewing the changes now we want to get back the changes that we made</p>

```c
git stash pop 
```

<p>Command to clear all the slashed entries</p>

```c
git stash clear
```

<h2>What is remote</h2>
<p>Remote/Remote repository means the main repository where all the developers share their changes. A remote reposity is usually stored in a code hosting service like Github.</p>

![alt text](https://github.com/NinjaAadi/Github-Commands/blob/master/remote-meaning.png)
<br/>
Image taken from https://www.javatpoint.com/git-remote

<p>Check your remote repo name</p>

```c
git remote
```
<p>Check your remote repository URL</p>

```c
git remote -v
```

<p>Add remote repository</p>

```c
git remote [name] [url]
```
<p>Exampe </p>

```c
git add origin https://github.com/NinjaAadi/Github-Commands.git
```

<h2>What is the difference between git fetch and git pull</h2>
<p>Git fetch is used to just check what changes are made in the repository without actually changing anything in the local repository.It is just for checking what changes are made. Where as git pull actually makes the changes in the remote repo to your local repository.We can see the changes in git fetch using git log/master/branchname</p>

Command to fetch a specific branch of a specific remote

```c
git fetch ["remote name"] ["branch name"]
```

Command to fetch all
```c
git fetch --all
```

See the commits that were made
```c
git log ["remote name"]/["branch name"]
```

Command to pull all the changes in the remote origin to local repo

```c
git pull ["remote origin name"]
```

Command to pull a change of certain branch of a remote repo

```c
git pull ["remote name"] ["branch name"]
```

<h2>Merging vs Rebasing</h2>
<p>When it comes to join two branches we have two options </p>
<ol>
<li>Merge two branches</li>
<li>Rebase the branch with its master branch</li>

<p>Here is the images showing difference between branching vs rebasing

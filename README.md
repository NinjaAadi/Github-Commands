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
<li>Show all the branches of the current repository

```c
git branch
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
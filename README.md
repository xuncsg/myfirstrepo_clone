# myfirstrepo_clone
Rerun for FSD repo with Markdown notes

## Notes
Markdown Format (.md) based off 'Markdown Cheat Sheet' at [MarkdownGuide](https://www.markdownguide.org/cheat-sheet/)


### This covers Scenario 1 (Standard Add/Commit/Push)

### Step 1: Cloning Repo from GitHub
1. Create New Repository from Github 
*No Repo template, Basic Descriptor, Public, gitignore set to 'Node'*
2. Within Visual Studio Code environment, *git clone https://github.com/xuncsg/myfirstrepo_clone.git .* **Note the  " ." after the repo https**

### Step 2: Create html file 
1. File -> index.html
*The file will be untracked*
2. Within *index.html* add some code into it via the emmet abbreviation to autofill code *!*

### Step 3: Push local repo to Github (Add,Commit,Push)
*At this point after the additon and modification of index.html the file is in the 'Staging Phase' ready to be commited and pushed to GH.*
1. git add index.html (Moves file to Staging area)
2. git commit -m "Homepage"
3. git push (this pushes the local repo to GH)

### Step 4: Making changes within index.html 
1. Modify index.html 
2. git add .
3. git commit -m "Updated homepage" *'-m' denotes message*
4. git push 
5. The changes will be reflected on GH 

### Other Steps (Done without collaborator)
1. Created contact.html and added internal notes
2. Created about.html 
3. Created product branch (git checkout -b products) *Shift+Ctrl+down*



| Syntax            | Description |
| :-----------       | :----------- |
| git clone <.>     | Clone a repository’s contents to the root of a local, working folder, observe appended ‘.’|
| git status        | Review modified and untracked files on a local, working branch.    |
| git add index.html about.html |Add modified and/or untracked files by its individual names to the staging area of a local, working branch before committing.|
|git commit **-m** "Comments"|Commit file(s) that were added to the staging area of a local, working branch - using a meaningful message to the commit.|
|git branch         |View available local branches AND the currently local, working branch.|
|git push           |Push a local branch on Github - works when an upstream has been established, see point #9. |
|git push **–force**    |Forcefully push changes to a remote repository, overriding any potential conflicts or discrepancies between our local branch and the remote branch|
|git push **-u origin** about_page| Push a specific branch to Github, same as running: git push --set-upstream origin about_page|
|git checkout main  |Checkout the EXISTING branch called main to work on.|
|git checkout **-b** about_page|Checkout a NEW branch called about_page from an existing branch.|
|git log            |Displays the commit history.|
|git log *--graph --decorate --oneline*|helpful for tracing branch activities visually|
|git fetch          |Fetch ALL updates from the remote repository without merging them.|
|git fetch **origin** about_page|Fetch updates from the remote branch called about_page.|
|git remote **-v**      |Displays the URLs of the remote repositories.|
|git pull           |Fetches AND merges updates from the remote repository into the current branch.|
|git pull **origin** about_page|Executing this command incorporates any updates from the about_page branch into our main branch (fetch + merge).|
|git **merge** products |Merges the branch products into the current branch.|
|git branch **-D** products|Forcefully deletes a local branch named ‘products’.|
|git branch **-m** product products_page| Renames an existing branch named ‘product’ to ‘products_page’.|
|git rebase main|Note #1: You may not have run into a situation where this is required; but good to know that git rebase <branch_name> combines a sequence of commits to a new base commit. 
|git rebase main|Note #2: It is important to note that during a rebase, conflicts may occur. Git will pause at each conflicting commit, and you will need to resolve the conflicts manually. Once resolved, run git rebase –continue to continue the rebase process.|
|git rebase main|Note #3: A rebase WILL rewrite commit history, which can cause traceability issues if you're working on a shared branch. It’s generally recommended to avoid rebasing commits that have already been pushed to a shared repository.|

Last Modified 6th August 2024








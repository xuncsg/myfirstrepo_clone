# myfirstrepo_clone
Rerun for FSD repo with Markdown (.md notes)

## Notes
Markdown Format (.md) based off 'Markdown Cheat Sheet' at [MarkdownGuide](https://www.markdownguide.org/cheat-sheet/)


##This covers Scenario 1 (Standard Add/Commit/Push)

### Step 1: Cloning Repo from GitHub
1. Create New Repository from Github 
*No Repo template, Basic Descriptor, Public, gitignore set to 'Node'*
2. Within VSC environment, *git clone https://github.com/xuncsg/myfirstrepo_clone.git .* **Note the ' .' after the repo https**

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

###Other Steps (Done without collaborator so without branch checkout)
1. Created contact.html and added internal notes
2. Created about.html 
3. Created product branch (git checkout -b products) *Shift+Ctrl+down*

| Syntax            | Description |
| -----------       | ----------- |
| git clone <.>     | Clone a repository’s contents to the root of a local, working folder, observe appended ‘.’|
| git status        | Review modified and untracked files on a local, working branch.    |
| git add index.html about.html |Add modified and/or untracked files by its individual names to the staging area of a local, working branch before committing.|
|git commit -m "Comments"|Commit file(s) that were added to the staging area of a local, working branch - using a meaningful message to the commit.|
|git branch         |View available local branches AND the currently local, working branch.|
|git push           |Push a local branch on Github - works when an upstream has been established, see point #9. |
|git push –force    |Forcefully push changes to a remote repository, overriding any potential conflicts or discrepancies between our local branch and the remote branch|





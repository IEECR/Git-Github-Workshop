# **MODULE 2: Local version control with Git** 

In this module, you will create your own local repository, create files and put them under local version control.
You will do that using the Git command-line interface (CLI); it means you will work from the terminal.

**Prerequisites:** VSCode, Git, a folder called *workshop-playground*. <br />
For more information about installing the prerequisits, consult the README.md. <br />

## Steps:
1. **Create a new folder *local-repo*:** <br />
*How:* - Create the folder in *workshop-playground*. <br />
*Note:* A repository naming convention is to use lower-case letters and dashes ('-') instead of spaces or underscores. <br />

2. **Create two .txt files in *local-repo*:** <br />
*How:* - Name the files: *animals.txt* and *words.txt*. <br />
&emsp; &emsp; - Write the name of your favourite animal into the file *animals.txt* and save. <br />

3. **Initialize a repository:** <br />
*How:* - In the terminal, move into *local-repo*. <br />
&emsp; &emsp; - Type: <span style="color:green"> git init</span>. <br />
&emsp; &emsp; - To check if it worked, use: <span style="color:green"> git status</span>. What can you see? <br />
*Note:* Initializing a repository does not mean that its content is tracked by Git automatically.<br />

4. **Track a file with Git:** <br />
*Note:* Files/ folders and changes to them are tracked by Git when they have been added to the index/ staging area. <br />
*How:* - Type: <span style="color:green"> git add *</span>. <br />
&emsp; &emsp; - Check with <span style="color:green"> git status</span>. What happened? <br />
&emsp; &emsp; - Type: <span style="color:green"> git rm --cached words.txt</span>.  What happened? <br />

5. **Commit the staged file:** <br />
*Note:* In a commit, all staged files are commited at once. For every commit you have to provide a commit-message. Think about what a good commit message could look like! <br />
*How:* - Type: <span style="color:green"> git commit -m "type your commit message"</span>. <br />
&emsp; &emsp; - Check with <span style="color:green"> git status</span>. <br />

6. **Edit *animals.txt*, stage, commit:** <br />
*How:* - Write the name of your least favourite animal into the file and save. <br />
&emsp; &emsp; - To stage only one file, use: <span style="color:green"> git add name-of-file</span>. <br />
&emsp; &emsp; - Type: <span style="color:green"> git commit -m "type your commit message"</span>. <br />

7. **Edit *words.txt*, stage, commit:** <br />
*How:* - Write 3 words starting with A into the file and save. <br />
&emsp; &emsp; - Stage the file. <br />
&emsp; &emsp; - Commit the file. <br />

8. **Undo a pervious commit:** <br />
*How:* - Delete the file *words.txt*. <br />
&emsp; &emsp; - Stage all files (<span style="color:green"> git add *</span>).<br />
&emsp; &emsp; - Commit. <br />
&emsp; &emsp; - To undo the last commit and recover the file, type: <span style="color:green"> git revert \-\-no-edit HEAD</span>. <br />
&emsp; &emsp; - Check with <span style="color:green"> git status</span>. <br />

10. **Edit *words.txt*, stage, commit:** <br />
*How:* - Add 3 words starting with B and save. <br />
&emsp; &emsp; - Stage the file. <br />
&emsp; &emsp; - Commit the file. <br />

11. **Check the commit history:** <br />
*How:* - Type: <span style="color:green"> git log</span>. <br />
&emsp; &emsp; - Can you figure out what git revert does? <br />
*Note:* git log shows you the commits to this repository, starting with the most recent one. Use the space key or arrow-down key to move through the list of commits. Use the q key to exit. <br />
<br />


##### Helpful links:
- The Git staging area: https://www.developernation.net/blog/git-internals-part-3-understanding-the-staging-area-in-git/
- Information about reverting to a previous commit: https://www.atlassian.com/git/tutorials/undoing-changes/git-revert
- Undoing things in Git: https://git-scm.com/book/en/v2/Git-Basics-Undoing-Things (Note: check the commit --amend option)
- Bonus: Stashing changes: https://www.atlassian.com/git/tutorials/saving-changes/git-stash#stashing-your-work

# **MODULE 3: Remote version control with Git & Github** 

There are two ways to connect a local and remote repository, depending on what exists first: <br />
1. You have a remote repository and want to clone it to your local machine. <br />
2. You have a local repository and want to connect it to a remote one. <br />

The first case is the more common one and you have done that in module 1, so we will not repeat it here. The second case can be useful if you have e.g. a folder with a lot of content that you want to turn into a Github repository without copying/moving everything. In this case you would turn it into a local Git repository (as we did in Module 2), track all files, and then connect it to a remote repository. We will do this now... <br />

**Prerequisites:** VSCode, Git, Github account, a local Git repository called *local-repo* with two .txt files named *animals.txt* and *words.txt*. <br />
For more information about installing the prerequisits, consult the README.md. <br />

## Steps:
1. **Create a new repository on Github.com:** <br />
*How:* - Go to [www.github.com](https://github.com/), click on your profile picture in the upper right corner<br />
&emsp; &emsp; - Select *Your repositories* <br />
&emsp; &emsp; - Create a new repository <br />
&emsp; &emsp; - Name it as you like and make it private <br />
&emsp; &emsp; - Copy the repositories URL <br />
*Note:* A repository naming convention is to use lower-case letters and dashes ('-') instead of spaces or underscores. <br />

2. **Connect the Github repository to your local repository:** <br />
*How:* -In the terminal, move into *local-repo* <br />
&emsp; &emsp; - Type: <span style="color:green"> git remote add origin url-of-your-github-repo</span>. <br />
*Note:* *origin* is the standard alias for the remote repository, but you could also name it oregano (or any other spice). <br />

3. **Push the committed files to the remote repository:** <br />
*Note:* You need to specify the name of the branch of the local repository you want to push from (the concept of branches will be treated in a later session, don't worry for now). <br />
*How:* - In the terminal, type: <span style="color:green"> git branch</span> <br />
&emsp; &emsp; - Type: <span style="color:green"> git push -u remote-repository-alias local-branch-name</span> <br />
&emsp; &emsp; - Online, refresh the page of your repository<br />
*Note:* After specifying it the first time, you can use the short form <span style="color:green"> git push</span>. <br />

4. **Check commit history online:** <br />
*How:* - Online, go to your repository. <br />
&emsp; &emsp; - Click on *Commits* below the green *Code* buttton <br />
&emsp; &emsp; - Compare to what you see with <span style="color:green"> git log</span> in your terminal <br />

5. **Edit *words.txt* on Github:** <br />
*How:* - Online, go to your repository and select the file *words.txt* <br />
&emsp; &emsp; - Click on the pencil on the right side of the window<br />
&emsp; &emsp; - Enter 3 words starting with C and commit <br />

6. **Pull changes from the remote to the local repository:** <br />
*How:* - In your terminal, type: <span style="color:green"> git pull </span> <br />
&emsp; &emsp;  In case of problems, try: <span style="color:green"> git pull remote-repository-alias local-branch-name</span> <br />
*Note:* The pull command actually performes two operations. You could perform them separately by using <span style="color:green"> git fetch</span>, this only downloads any changes from the remote repository but does not affect the current state of your local repository, and <span style="color:green"> git merge</span>, which does the merging magic and updates your working tree as well. <br />

7. **Create conflicting commits:** <br />
*How:* - Add 3 words starting with D in *words.txt* and save (locally, not on Github) <br />
&emsp; &emsp; - Stage the file <br />
&emsp; &emsp; - Commit it <br />
&emsp; &emsp; - Online, edit *words.txt*: enter 3 words starting with E and commit<br />
&emsp; &emsp; - In your terminal, type: <span style="color:green"> git fetch</span> <br />
&emsp; &emsp; - Check with <span style="color:green"> git status</span> <br />
&emsp; &emsp; - Try: <span style="color:green"> git merge</span> <br />

8. **Handle a merge conflict:** Decide which changes to keep!<br />
*Note:* It is important that you have committed your local changes, and performed a pull action before you proceed (step 7). <br />
*How:* Keep local changes: <br />
&emsp; &emsp; - <span style="color:green"> git checkout --ours name-of-file</span> <br />
&emsp; &emsp; - Stage it <br />
&emsp; &emsp; - Commit it <br />
&emsp; &emsp; - Push it <br />
&emsp; &emsp; Keep remote changes: <br />
&emsp; &emsp; - <span style="color:green"> git checkout --theirs name-of-file</span> <br />
&emsp; &emsp; - Stage it <br />
&emsp; &emsp; - Commit it <br />

9. **Push to anothers remote repository:** <br />
*How:* - Open the repository you cloned in module 1 (*Git-Github-Workshop*) <br />
&emsp; &emsp; - Open the file 001.txt in the folder *txt-files* in *session_1* <br />
&emsp; &emsp; - Answer the question in it and save <br />
&emsp; &emsp; - Stage it using <span style="color:green"> git add *</span> <br />
&emsp; &emsp; - Commit it <br />
&emsp; &emsp; - Push it. What happens? <br />
<br />


##### Helpful links:
- Managing remote repositories: https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories
- About Git fetch: https://www.freecodecamp.org/news/git-pull-remote-branch-how-to-fetch-remote-branches-in-git/
- Some tips on resolving merge conflicts: https://stackoverflow.com/questions/161813/how-do-i-resolve-merge-conflicts-in-a-git-repository
- Some troubleshooting for 'repository not found'-error: https://stackoverflow.com/questions/37813568/git-remote-repository-not-found
- Some information about git init --bare: https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-init

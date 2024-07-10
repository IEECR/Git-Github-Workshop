# **MODULE 5: What makes a good repository** 

In this module, you will create a repository structure for a bunch of pseudo files representing the types of files
you find in a research project. You will also create a gitignore file and fill the README.md with sensible information.
<br />

**Prerequisites:** VSCode, Git, Github account, a local git repository that is connected to a remote one. <br />
For more information about installing the prerequisits, consult the README.md. <br />

## Steps:
1. **Download data from Sciebo:** <br />
*How:* - Go to the [Sciebo folder](https://uni-bonn.sciebo.de/s/qgWbEE7XvLTuPw4) we prepared<br />
&emsp; &emsp; - Download all data <br />
&emsp; &emsp; - Move them into the repository you created in module 4 <br />

2. **Structure your Repository!** <br />
*How:* - Create folders and sort the downloaded files into them <br />
&emsp; &emsp; - Which repository structure makes the most sense to you?  <br />

3. **Create a gitignore file:** <br />
*Note:* In science projects, there are often data of huge size that you do not want to track with Git. Furthermore, auxiliary files that are generated when writing code for example, you ideally do not want to track. This is done using a gitignore file. <br />
*How:* - Create a new file in the main repository folder  <br />
&emsp; &emsp; - Name it *.gitignore* (the dot is intentional, no extension!) <br />
&emsp; &emsp; - Enter all names of files & folders that should be ignored <br />
- So called wildcards (*,**) are very useful here. A wildcard is like a placeholder: if you add *.txt to your gitignore file, all files in your repository that have the extension .txt are ignored.<br />
- There are good templates for gitignore files for different application cases (see links below). <br />
- When creating a Github repository online, you can select a template and the gitignore file is automatically created. <br />

4. **Sync with your remote repository:** <br />
*How:* - Stage all files <br />
&emsp; &emsp; - Commit<br />
&emsp; &emsp; - Sync (Pull & Push) <br />
&emsp; &emsp; - Did it work? Were there any warnings? <br />

5. **Add previously committed file/folder to .gitignore:** <br />
*How:* - Add the file to .gitignore and save <br />
&emsp; &emsp; - In the terminal, type: <span style="color:green"> git rm --chached file-or-folder-to-ignore</span> <br />
&emsp; &emsp; - Stage all files <br />
&emsp; &emsp; - Commit <br />
&emsp; &emsp; - Sync (Pull & Push) <br />
*Note:* If you want to remove all files of one format you can use a wildcard: <span style="color:green"> git rm --chached *.format-to-ignore</span>. <br />

6. **Make the README file informative:** <br />
*How:* - Enter all necessary imformation to help users (others or future you) to make sense of the repository <br />
&emsp; &emsp; - What do you think should be in it?<br />

7. **Sync with your remote repository:** <br />
*How:* - Stage all files <br />
&emsp; &emsp; - Commit<br />
&emsp; &emsp; - Sync (Pull & Push) <br />
<br />


##### Helpful links:
- Some information on the gitignore file: https://linuxize.com/post/gitignore-ignoring-files-in-git/
- gitignore templates: https://github.com/github/gitignore
- gitignore (incl. section on ignoring previously committed files): https://www.atlassian.com/git/tutorials/saving-changes/gitignore
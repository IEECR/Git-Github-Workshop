# **MODULE 4: Basics of VS Code Git integragion** 

In this module, you will use the Git integration for VSCode, so it will be buttons instead of commands.
<br />

**Prerequisites:** VSCode, Git, Github account, a folder called *workshop-playground*. <br />
For more information about installing the prerequisits, consult the README.md. <br />

## Steps:
1. **Create a new repository on Github.com:** <br />
*How:* - Create a new repository on [www.github.com](https://github.com/).<br />
&emsp; &emsp; - Name it as you like and make it private. <br />
&emsp; &emsp; - Copy the repositories URL. <br />

2. **Clone the repository using VSCode:** <br />
*How:* -In VSCode, open a new window: *File* > *New Window*. <br />
&emsp; &emsp; - Click on to the *Source Control* tab in the menu bar at the left side. <br />
&emsp; &emsp; - Click on *Clone Repository*.<br />
&emsp; &emsp; - Enter the URL into the text field at the top of the VSCode window. <br />
&emsp; &emsp; - Select *Clone from URL*. <br />
&emsp; &emsp; - Save it in the folder *workshop-playground*. <br />
&emsp; &emsp; - Open the repository and trust the authors if asked. <br />
*Note:* Alternatively, you can select *Clone Git Repository...* in the main window right after opening a new VSCode window.
 <br />

3. **(Add and) Edit the README file:** <br />
*How:* - If there is not yet a README.md in your cloned repository, go to: <br />
&emsp; &emsp;  *File* > *New File* > *Text File*. <br />
&emsp; &emsp; - Save it as *README.md*.<br />
&emsp; &emsp; - Write your name and the date into the file.<br />

4. **Use VSCode's Source Control Tab:** <br />
*Note:* In the Source Control tab (third item in toolbar at left side of VSCode window), you see a section 'Changes' and a 'M' behind the README.md. This indicates that a file that is tracked by Git has been modified. <br />
&emsp; &emsp; - To stage specific files, click on the *+* behind the file(s).<br />
&emsp; &emsp; - To commit, enter a commit message and click on *Commit*. <br />
&emsp; &emsp; - To push to the remote repository, click on *Sync*. <br />
*Note:* The *Sync* operation in VSCode performs first a git pull and then a git push operation. <br />
<br />


##### Helpful links:
- Git source control in VSCode: https://code.visualstudio.com/docs/sourcecontrol/overview
- Auto fetch in VS Code: https://code.visualstudio.com/docs/sourcecontrol/overview#_remotes
# **MODULE 1: Setting it up** 

*Welcome to the first module.*

The goal of the (very short) first module is simply to check if everything is working. You will also get to know a few commands in order to work from the terminal.

Furthermore, you will clone your first repository from Github.

**Prerequisites:** VSCode, Git, Github Account, 2-Factor-Authentification or SSH key pair. <br />
For more information about installing the prerequisits, consult the README.md. <br />

## Steps:
1. **Open a folder** in **VSCode** in which you want to work during the workshop. <br />
*How:* - *File* tab on top > *Open Folder...* <br />
&emsp; &emsp; - Trust the authors when asked. <br />

3. **Open a terminal** in VSCode. (You could also do this in a terminal outside of VSCode) <br />
*How:* *Terminal* tab on top > *New Termial*

4. **Create folders from the terminal:** <br />
*How:* Using only the terminal, check what content you find in your current folder and create a new folder named *workshop-playground*. Move into it and create two new folders named *zip-repo* and *cloned-repo*. <br />

| Function                   | Windows            | Linux              |
| :--------                  | :-------           | :-------           |
| Show current location      | cd                 | pwd                |
| Move to subdirectory       | cd dir-name        | cd dir-name        |
| Move to parent directory   | cd..               | cd ..              |
| Move to another drive      | drive-name:        | ?                  |
| Move to specific directory | cd /absolute/path  | cd /absolute/path  |
| List content               | dir                | ls                 |
| Create a new directory     | mkdir new-dir-name | mkdir new-dir-name |
| Remove a directory         | rmdir -p dir-name  | rm -r dir-name     |

4. **Check if Git is working**: <br />
*How:* Type into the terminal: <br />
&emsp; &emsp; - <span style="color:green"> git</span>: It should display an overview of possible commands. <br />
&emsp; &emsp; - <span style="color:green"> git \-\-version</span>: It should display the version of git you have.

5. **Connect git and Github:** <br />
*How:* Type into the terminal: <br />
<span style="color:green"> git config user.email "email_of_your_github_profile"</span>  <br />
<span style="color:green"> git config user.name "your_github_profile_name"</span>  <br />
*Note:* To check if it worked you can type only <span style="color:green"> git config user.email</span> and likewise for the name <br />

6. **Download the zip repository** - the *ugly* way:  <br />
*How:* - Go to the Github repository from step 1 ([(Git-Github-Workshop](https://github.com/IEECR/Git-Github-Workshop/tree/main)) <br />
&emsp; &emsp; - There is a green button *Code*, click on it and select *Download ZIP*. <br />
&emsp; &emsp; - Unpack the ZIP folder into the folder named *zip-repo* that you created. <br /> 

7. **Clone the repository:** <br />
*How:* - Go to the Github repository from step 1. <br />
&emsp; &emsp; - Click on the green *Code* button and copy the repository's URL. <br />
&emsp; &emsp; - In the terminal, move to *workshop-playground*. <br />
&emsp; &emsp; - Type into the terminal: <span style="color:green"> git clone url-to-repo cloned-repo </span> <br />
*Note:* This will clone the repository you indicate to the folder you indicate (in our case *cloned-repo*). You can also leave away the folder name, then a folder with the repository's name is created automatically. <br />

8. **Check if the cloning worked:** <br />
*How:* - In the terminal, move into the folder of your cloned repository. <br />
&emsp; &emsp; - Type: <span style="color:green"> git status</span>. What do you see? <br />
*Note:* git status gives you an overview of the changes tracked by git.

9. **Compare zipped and cloned repository:** <br />
*How:* - In the terminal, move into the folder *Git-Github-Workshop-main* in your folder *zip-repo*. <br />
&emsp; &emsp; - Type: <span style="color:green"> git status</span>. What do you see? <br />
&emsp; &emsp; - Inspect the content of the zipped and cloned repository. <br />
 <br />



##### Helpful links:
- 2-Factor Authentification for Github:https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication#configuring-two-factor-authentication-using-a-totp-app
- Generate and add a new SSH key: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh,
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account
- Git clone documentation: https://git-scm.com/docs/git-clone
- Updating Git: https://phoenixnap.com/kb/how-to-update-git

## Setting up git on mac:

### 1. Installing Git on Mac
Git can be installed on Mac in many ways. One of the best approach is using homebrew
Homebrew can be installed by running the blow command in terminal
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
The above command may request for password, once you enter your mac password, homebrew should be installed.
Now install git by entering the below command in terminal
```bash
brew install git
```
To verify if git has been successfully installed or not, run the below command
```bash
Git --version
```
Refer:
"https://git-scm.com/book/en/v2/Getting-Started-Installing-Git"
"https://www.freecodecamp.org/news/setup-git-on-mac/"

### 2. Configure git on Mac 
To work with Git, you must set up your Git environment using the git config command. 
Before getting started with the git commands, lets do some git configuration settings
    
### Personal Access token
1. Go to "Setting" in git hub
2. Go to "Developer Settings"
3. Click on "Personal access token" 
4. Select "Tokens(classic)"
5. Click on "Generate new token"
    
### Name
To set up your Git config file, open a WSL command line and set your name with this command 
(replacing "Your Name" with your preferred username):
```bash
git config --global user.name "Your Name"
```
### Email
Set your email with this command (replacing "youremail@domain.com" with the email you prefer):
```bash
git config --global user.email "youremail@domain.com"
```
### Username
Add your GitHub username to link it to git (remember, it is case sensitive!):
```bash
git config --global user.username "GitHub username"
```
### Token
Add your token
```bash
git config --global github.token <your token>
```
Refer : 
"https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token"
    


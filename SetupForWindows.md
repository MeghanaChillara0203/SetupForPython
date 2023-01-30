# Setup For Windows

## Setting up for WSL ( Windows Subsystem for Linux) and git on windows:

### 1. Install Linux on windows
Right click on Windows Powershell and click "Run as Administrator"
Then run the below commands
```
wsl --install
```
To check the version of wsl you installed :
```bash
wsl -l -v
```
To set the default version to WSL 1 or WSL 2 when a new Linux distribution is installed:
```bash
wsl --set-default-version <Version#>
```
Replace <Version#> with either 1 or 2
    
Refer: 
    "https://learn.microsoft.com/en-us/windows/wsl/install"
    "https://learn.microsoft.com/en-us/windows/wsl/"
    https://learn.microsoft.com/en-us/windows/wsl/basic-commands?source=recommendations

### 2. Switch to WSL from Powershell/Command prompt when you open command prompt on windows

```bash
wsl
```
    
### 3. Configure git on windows (Linux)
Git comes installed with most Linux distributions, but you can make sure you're using the latest stable version 
by running the following command:
```bash
sudo apt-get install git
```
To verify if git is successfully installed or not, type the following command
```bash
git --version
```
    
### 4. Logging into git 
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
Refer : https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token
    


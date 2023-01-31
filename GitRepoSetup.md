## Git Repo

### 1. To clone a repository

1. Go to the git hub repository
1. In the github repository, click on "Code"
2. Copy the link to clone the repository
3. Open terminal/command prompt in your local machine
4. Navigate to the directory in which you want to clone the git hub repository using **cd** command
5. Execute the following command to clone the repository
```bash
git clone <link>
```
Replace <link> with the link of the repository you would like to clone, It may require your github credentials
6. Use **cd** command to navigate into the repository
7. Now you are all set to work with the repository.

### 2. Git branch

#### To create branch 
1. Clone the repository and navigate to directory of the repository (Ignore this step if you have already cloned the repository)
2. Execute the following command to see all the branchs in the repository
```bash
git branch
```
3. Execute the following command to create a new branch
```bash
git branch <branchname>
```
Replace branchname with the name you would like to give for the branch. Remember the name should not have spaces or special characters and it is case sensitive.
4. To change branch from "main" or current branch to a different branch, execute:
```bash
git checkout <branchname>   
```
Replace branchname with an existing branch name

### 3. Git pull
1. Clone the repository and navigate to directory of the repository (Ignore this step if you have already cloned the repository)
2. Before making any changes locally or pushing changes to the repository, it is advisible to run pull command, to make sure the local and git repository are in sync. 
3. Execute the following command to pull changes from github repository
```bash
git pull
```
3. In case you are using any branch, to pull changes in git repository to your branch, run:
```bash
git merge origin <branchname>
```
Replace branchname with the name you are working with.


### 4. Git push
1. Clone the repository and navigate to directory of the repository (Ignore this step if you have already cloned the repository)
2. Before making any changes locally or pushing changes to the repository, it is advisible to run pull command, to make sure the local and git repository are in sync. 
3. Before pushing the changes to github repository, you have to first add and commit the changes
4. Run the following steps in sequential steps
5. To add your changes to the commit, run:
```bash
git add .
```
6. To commit the changes, run:
```bash
git commit -m "Message"
```
Replace Message with any message you want to add for your commit
7. Finally, If you are not using any branch, run:
```bash
git push
```
8. If you are using branch run:
```bash
git push origin branchname
```
Replace branchname with the name you are working with.

### 5. Other git commands and indepth information about each command and its usage
Refer: "https://git-scm.com/docs"



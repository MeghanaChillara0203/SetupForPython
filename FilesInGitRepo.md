## Files in git repo

### 1. README.md
The Readme file is typically the first file that users read. It is a text file that gives users information about the software, project, code, or game. It may also give users instructions, help, or information about patches or upgrades.
Your README.md should conatin summary of details and steps of your project and instructions on how to reproduce the results.

#### To create a README.md file
1. In your github repository, click on "Add file"
2. Select "Create new file"
3. Give the file name as **"README.md"**
4. Add information in your README.md file and commit the changes for it to reflect in your repo.

Refer: "https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes"

### 2. The .gitignore file
The .gitignore file is a text file that tells Git which files or folders to ignore in a project.
A local .gitignore file is usually placed in the root directory of a project. You can also create a global .gitignore file and any entries in that file will be ignored in all of your Git repositories.
It is generally used to tell git to ignore system files and large data files such as ( .DS_Store, .csv)
Enter each extension in a seperate line.

The ".gitignore" files are not visible in the folder, it see the files press "cmd + ." (cmd and dot seperator at the same time)

#### To create .gitignore file on github
1. In your github repository, click on "Add file"
2. Select "Create new file"
3. Give the file name as ".gitignore"
4. Add the extenstions you want git to ignore in your ".gitignore" file and commit the changes for it to reflect in your repo.

#### To create .gitignore file on local system
1. Navigate to the root directory folder on your local system
2. Open notepad or textfile 
3. Enter each extension you want git to ignore in a seperate line.
4. Give the file name as **".gitignore"** and save it in the root directory for your git repository on your local system.
5. Commit the changes to github

Refer: "https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files"
    
### 3. requirements.txt 
A requirements file is a list of all the dependencies of a project. This includes the dependencies that the dependencies require. Additionally, each dependency's specific version is included, denoted by a double equals sign (==).
A Requirements file typically consists of a collection of pip install arguments that have been stored in a file. Please take note that pip will not necessarily install the things in the file in the order specified in the file.
For example, at requirements.txt file can look like:
```bash
matplotlib==3.6.2
    # via
    #   -r requirements.in
    #   seaborn
numpy==1.23.5
    # via
    #   -r requirements.in
    #   contourpy
    #   matplotlib
    #   pandas
    #   scipy
    #   seaborn
```
To execute a requirements.txt file:
```bash
pip install -r requirements.txt
```

#### To create requirements.txt 
1. In your github repository, click on "Add file"
2. Select "Create new file"
3. Give the file name as **"requirements.txt"**
4. Add information in your requirements.txt file and commit the changes for it to reflect in your repo

Refer: "https://gist.github.com/kaniket7209/9aa972b9d6b5d1542e1731d28de77efc"
    
### 4. A folder for your data files (mostly .csv files)
This is not mandatory but it is a good practice to keep your repo organized. It would help a third person looking at your repository to understand where each file is stored. 
A folder can be added to your github by cloning the repository and running the command in terminal

#### To create a data folder
1. In your github repository, click on "Code"
2. Copy link to the repository
3. in your local system, open terminal
4. Change path to the directory where you want to clone your repository
5. Execute the following command
```bash
git clone <link>
```
Replace <link> with the link to your repository
6. Change path to your repository by :
```bash
cd repositoryname
```
7. To create data folder, run:
```bash
mkdir data
```
8. This would create data directory/folder in your repository locally
9.To add this folder to the github repo, commit the changes for it to reflect in your repo.

### 5. A folder for your script files (Python, R, or any other script files ending with .py, .r, .java, etc)
This is not mandatory but it is a good practice to keep your repo organized. It would help a third person looking at your repository to understand where each file is stored. 
A folder can be added to your github by cloning the repository and running the command in terminal

#### To create a src(source files/ scripts) folder
1. In your github repository, click on "Code"
2. Copy link to the repository
3. in your local system, open terminal
4. Change path to the directory where you want to clone your repository
5. Execute the following command
```bash
git clone <link>
```
Replace <link> with the link to your repository
6. Change path to your repository by :
```bash
cd repositoryname
```
7. To create src folder, run:
```bash
mkdir src
```
8. This would create src directory/folder in your repository locally
9.To add this folder to the github repo, commit the changes for it to reflect in your repo.

### 6. A folder for your media files ( files with media extesions such as .png, .jpeg, etc)
This is not mandatory but it is a good practice to keep your repo organized. It would help a third person looking at your repository to understand where each file is stored. 
A folder can be added to your github by cloning the repository and running the command in terminal

#### To create a figs(figures/images/media) folder
1. In your github repository, click on "Code"
2. Copy link to the repository
3. in your local system, open terminal
4. Change path to the directory where you want to clone your repository
5. Execute the following command
```bash
git clone <link>
```
Replace <link> with the link to your repository
6. Change path to your repository by :
```bash
cd repositoryname
```
7. To create figs folder, run:
```bash
mkdir figs
```
8. This would create figs directory/folder in your repository locally
9.To add this folder to the github repo, commit the changes for it to reflect in your repo.

### 7. Makefile
Developers specify the build procedure for their programs in text files called makefiles. The instructions in the Makefile can then be readily executed using the make command. It is one of the most important files in your repository based on your project requirements.
The make commands help others execute and reproduce the results without have to go through all the files in the repository.
For example, a Makefile would look like:
```bash
.PHONY: data

command1:
	python -B src/pythonscriptfile.py

```
#### To create a Makefile file
1. In your github repository, click on "Add file"
2. Select "Create new file"
3. Give the file name as **"Makefile"** without and any extensions
4. Add information in your Makefile and commit the changes for it to reflect in your repo.

Refer: "https://github.com/teamniteo/Makefile"

### 8. LICENSE

#### To create a LICENSE file
1. In your github repository, click on "Add file"
2. Select "Create new file"
3. Give the file name as **"LICENSE"** without and any extensions
4. Add information in your LICENSE file and commit the changes for it to reflect in your repo.

Refer: "https://www.fastcompany.com/3014553/what-coders-should-know-about-copyright-licensing"
"https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository"

### 9. Any other files or folders that you want to add based on your project or requirement
based on your reuirement, you can add files and folders to your repository

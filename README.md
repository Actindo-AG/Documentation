# Documentation

This documentation covers all (current) modules of the Core1 Platform.

## Gitub Workflow  

In the following, the setup of all necessary software as well as the cloning of the GitHub documentation repository and the Git documentation workflow from creating a new branch up to merging the branches is described.

### Software setup

The following software needs to be installed and configured:
- [Code editor](#code-editor)
- [Git](#Git)
- [GitHub](#GitHub)


#### Code editor

The documentation is written in markdown. To do so, you should use an code editor. If you have already worked with an code editor and you are used to a certain one, you can use this one. If not, there are several free editors you can use, such as Atom (https://atom.io/), Sublime Text (https://www.sublimetext.com/), Visual Studio Code (https://code.visualstudio.com/), etc.

Download the application and install it on your local machine.


#### Git

Git is a modern version control system which is perfect to use in teams. It tracks all changes in the documentation.
Depending on the operating system, Git may already been installed. Follow the guide to check if Git is already installed on your system or to install it:  https://github.com/git-guides/install-git

If you are working on Windows machine, it is recommended to install Git Bash as a terminal instead of the windows command prompt. If you use the Windows Installer for Git in the link above, Git Bash is included in the download.


#### GitHub

Github is the website, where Git repositories are hosted. Open https://github.com/ in your browser to sign up for a new account using your Actindo email-address. Note your user name and contact Julian Seyfried to invite you to the Actindo documentation repository by sending him you user name.


### Git Basics

To understand Git and GitHub, it is important to understand the basic terminology and commands below.

#### Git Terms

- *Directory*   
  A directory equals to a folder on your computer.

- *Terminal*   
  A terminal is an application that runs on your computer, such as Git Bash. It is the interface where you enter the text commands, navigate around files and folders, create files, change updates and so on. Alternatively, the term *Command Line* is used.

- *Repository*   
  A repository equals to a project or the folder, where a project is stored. The short version *repo* is often used.

- *Branch*   
  A branch is a parallel version of a repository. By default a repository has a main or master branch representing the initial state. When creating a new branch, this branch copies the current state of the main branch and allows you to make changes on the new branch without affecting the main branch. By merging the branches, the changes can be included into the main branch.

#### Git Commands

- *clone*    
  Use this command to bring a repository that is hosted somewhere into a folder on your local machine.   

- *status*   
  Use this command to display changes and untracked files in Git.

- *add*   
  Use this command to track files and changes in Git.

- *commit*    
  Use this command to save your files in Git.

- *push*   
  Use this command to upload your Git commits to a repository in GitHub (opposite of *pull*).

- *pull*   
  Use this command to download changes from the remote repository in GitHub to your local machine (opposite of *push*).

- *checkout*      
  Use this command to switch to another branch.

- *branch*   
  Use this command to show all existing branches in the repo.

- *merge*   
  Use this command to include all changes from one branch to another branch.

- *clear*   
  Use this command to clear the terminal.


### SSH Key for GitHub

Generate a SSH Key and add it to your GitHub account in order to use it for authentication.

#### Create a new SSH Key

1. Open Git Bash.

2. Enter the following code:   
        ssh-keygen -t rsa -b 4096 -C "YourGithubEmail@actindo.com"

  The SSH key pair is generated. By default, the key is saved in your user directory in the .ssh directory named *id_rsa* .

3. If desired, enter an alternative filename for the key. Otherwise, push [ENTER].

4. Enter a passphrase for your key to make it more secure. Push [ENTER] to confirm the passphrase.

  > [Info] Nothing is displayed when you enter the passphrase.

5. Enter the same passphrase again and push [ENTER] to confirm the passphrase.


#### Add the public key to your account



#### Add your private key to the ssh-agent



### Clone the repository

When you have created your GitHub account and you are invited to the Documentation Repository, you can prepare your GitHub account to clone the repository.

Open your

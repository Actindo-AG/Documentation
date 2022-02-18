# Documentation workflow

In the following, the setup of all necessary software as well as the cloning of the GitHub documentation repository and the Git documentation workflow from creating a new branch up to merging the branches is described.

## Software setup

The following software needs to be installed and configured:
- [Code editor](#code-editor)
- [Git](#Git)
- [GitHub](#GitHub)


### Code editor

The documentation is written in markdown. To do so, you should use an code editor. If you have already worked with an code editor and you are used to a certain one, you can use this one. If not, there are several free editors you can use, such as Atom (https://atom.io/), Sublime Text (https://www.sublimetext.com/), Visual Studio Code (https://code.visualstudio.com/), etc.

Download the application and install it on your local machine.


### Git

Git is a modern version control system which is perfect to use in teams. It tracks all changes in the documentation.
Depending on the operating system, Git may already been installed. Follow the guide to check if Git is already installed on your system or to install it:  https://github.com/git-guides/install-git

If you are working on Windows machine, it is recommended to install Git Bash as a terminal instead of the windows command prompt. If you use the Windows Installer for Git in the link above, Git Bash is included in the download.


### GitHub

Github is the website, where Git repositories are hosted. Open https://github.com/ in your browser to sign up for a new account using your Actindo email-address. Note your user name and contact Julian Seyfried to invite you to the Actindo documentation repository by sending him you user name.


## Git Basics

To understand Git and GitHub, it is important to understand the basic terminology and commands below.

### Git Terms

- *Directory*   
  A directory equals to a folder on your computer.

- *Terminal*   
  A terminal is an application that runs on your computer, such as Git Bash. It is the interface where you enter the text commands, navigate around files and folders, create files, change updates and so on. Alternatively, the term *Command Line* is used.

- *Repository*   
  A repository equals to a project or the folder, where a project is stored. The short version *repo* is often used.

- *Branch*   
  A branch is a parallel version of a repository. By default a repository has a main or master branch representing the initial state. When creating a new branch, this branch copies the current state of the main branch and allows you to make changes on the new branch without affecting the main branch. By merging the branches, the changes can be included into the main branch.

### Git Commands

- *git clone*    
  Use this command to bring a repository that is hosted somewhere into a folder on your local machine.   

- *git status*   
  Use this command to display changes and untracked files in Git.

- *git add .*/*git add [file_name]*   
  Use this command to track files and changes in Git. You can either track all changes and files using the *git add .* command or you track a single file using the *git add [file_name]* command, by replacing the *[file_name]* with the name of the file you want to track.

- *git commit -m "title" -m "description"*    
  Use this command to save your files in Git. You have to add a commit message to the command. The first message is the title of the message. For documentation purposes, use the JIRA ticket number you are working on for the title. The second message is the description. Add some information about the changes you made in the description.

- *git commit -am "title" -m "description"*    
  Use this command to track and save your files in Git. This command is only possible for modified files. Untracked files have to be added separately with the *git add* command. The commit message rules are the same as for the *git commit* command.  

- *git push origin [branch_name]*   
  Use this command to upload your Git commits to a repository in GitHub by replacing *[branch_name]* with the name of the branch you are working on. The *git push* command is the opposite of the *git pull* command.

- *git pull*   
  Use this command to download changes from the remote repository in GitHub to your local machine (opposite of *push*).

- *git checkout*      
  Use this command to switch to another branch.

- *git checkout -b [branch_name]*      
  Use this command to create a new branch and switch to it by replacing *[branch_name]* with the name of the new branch. For documentation purposes, use the JIRA ticket number for the branch name. If you are working on a single ticket, use this number, if you are working on a ticket which makes part of an epic, use the epic ticket number as braanch name.

- *git branch*   
  Use this command to show all existing branches in the local repo. The branch you are currently working on is highlighted.

- *git branch -a*   
  Use this command to show all existing branches in the local repo as well as in the remote repo. The branch you are currently working on is highlighted.

- *git branch -r*   
  Use this command to show all existing branches in the remote repo. The branch you are currently working on is highlighted.

- *git merge [branch_name]*   
  Use this command to include all changes from the branch you are indicating in the command into the branch you are currently working on. Replace the *[branch_name]* with the name of the branch from which you want to include the changes. For instance, to include the changes of the main branch into a feature branch, you have to switch to the feature branch and use the command *git merge main*.

- *git fetch*   
  Use this command to get commits, files, and chagnes from the remote repo into your local repo and see, what other team members has been working on.

- *clear*   
  Use this command to clear the terminal.

- *cd*   
  Use this command to change the directory.

## SSH Key for GitHub

Generate a SSH Key and add it to your GitHub account in order to use it for authentication.

### Create a new SSH Key

1. Open Git Bash.

2. Enter the code below to generate a new SSH key.

        ssh-keygen -t rsa -b 4096 -C "YourGithubEmail@actindo.com"

  The SSH key pair is generated. By default, the key is saved in your user directory in the .ssh directory named *id_rsa* .

3. If desired, enter an alternative filename for the key. Otherwise, push [ENTER].

4. Enter a passphrase for your key to make it more secure. Push [ENTER] to confirm the passphrase.

  > [Info] Nothing is displayed when you enter the passphrase.

5. Enter the same passphrase again and push [ENTER] to confirm the passphrase.


### Add the public key to your account

To add your public key to your account, you can either copy it in your terminal or navigate to the file in your file explorer, open the public key file and copy it from there. in the following, it is described how to get your public key by using your terminal.

1. Enter the code below to navigate to the directory where you saved the SSH key. By default, this is the .ssh directory in your user directory.   

        cd ~/.ssh

2. Enter the code below to display the public key. By default, your public key was saved as *id_rsa.pub*. If you created your key with a different name, replace *id_rsa.pub* in the command with the name of your public key file.

        cat id_rsa.pub

    Your public key is displayed in the terminal. It starts with *ssh-rsa* and ends with your e-mail address.

3. Copy the key in your terminal. To do so, highlight the key in your terminal.   
  The highlighted text is copied to your clipboard. Alternatively, use the shortcut *Ctrl* + *Ins* or right-click the highlighted text in your terminal and click *Copy* in the displayed context menu.

  > [Info] Note that copying in the terminal is not working the same way as in a text editor. Do **never** use the shortcut *Ctrl* + *C* as it has another function in your terminal!  

4. Log in to your GitHub account in the browser.

5. Click the avatar of your profile in the upper right corner of your GitHub account and select the menu entry *Settings* .   
  Your account settings are displayed.

6. Click the entry *SSH and GPG keys* in the section *Access* of the left menu column.   

7. Click the button [New SSH key].

8. Enter a title for your public SSH key in the field *Title*.

9. Click the field *Key* and paste the copied key from your clipboard. If necessary, remove all blank spaces at the end of the key.

10. Click the button [Add SSH key] to add the key to your GitHub account.   
  The login to your GitHub account is displayed.

11. Enter your password to confirm the adding of the SSH key.


### Add your private key to the ssh-agent

To authorize in you local Git terminal (Git Bash), you have to add your private key to the ssh-agent.

1. Enter the code below to start the ssh-agent in the background.

        eval "$(ssh-agent -s)"

2. Enter the code below to add your private key to the ssh-agent. If you created your key with a different name, replace *id_rsa* in the command with the name of your private key file.

        ssh-add ~/.ssh/id_rsa

3. Enter your passphrase for the private key and push [ENTER].   
  The message *Identity added* is displayed in the terminal.


#### Auto-launching the ssh-agent

To run the ssh-agent automatically when you open Git Bash, follow the instructions below.

1. Open a new file in your code editor.

2. Copy the code below and save the file as *.bashrc* in your user directory (C:\Users\Username).

          env=~/.ssh/agent.env

          agent_load_env () { test -f "$env" && . "$env" >| /dev/null ; }

          agent_start () {
          (umask 077; ssh-agent >| "$env")
          . "$env" >| /dev/null ; }

          agent_load_env

          # agent_run_state: 0=agent running w/ key; 1=agent w/o key; 2=agent not running
          agent_run_state=$(ssh-add -l >| /dev/null 2>&1; echo $?)

          if [ ! "$SSH_AUTH_SOCK" ] || [ $agent_run_state = 2 ]; then
          agent_start
          ssh-add
          elif [ "$SSH_AUTH_SOCK" ] && [ $agent_run_state = 1 ]; then
          ssh-add
          fi

          unset env

3. Open a new file in your code editor.

4. Copy the code below and save the file as *.bash_profile* in your user directory (C:/Users/Username).  

        test -f ~/.profile && . ~/.profile
        test -f ~/.bashrc && . ~/.bashrc

5. Open Git Bash.    
    You are prompted for your passphrase.

6. Enter your passphrase and push [ENTER].   
    The ssh-agent process will continue to run until you log out, shut down your computer, or kill the process.


## Clone the repository

After you have created your SSH Key and configured the Git Bash terminal, you can clone the documentation repository to your local machine.

1. Open the Documentation Repository in your GitHub account.

2. Click the green button [Code].   
  The *Clone* window is displayed.

3. Click *SHH* in the window and copy the displayed remote URL in the text field.

4. Open Git Bash.

5. Enter the code below, replace *ssh_url* in the command with the copied remote URL and *path_directory* with the desired directory where you want to clone the repository. Note that the indicated directory should be empty!

        git clone ssh_url path_directory

      The repository is cloned to the indicated directory.

6. Open your code editor.

7. Add the directory where you cloned the repository as a project folder.


## Git workflow in documentation

The following scheme shows the documentation workflow via Git. Each step is described in detail in the following chapters.

![Git workflow](/Assets/GitWorkflow.jpg "[Git workflow]")

To start your documentation, you need to prepare as described below.

1. Open JIRA, navigate to the ticket you will work on and note the ticket-number.

  > [Info] When you start working on a JIRA ticket, switch the workkflow status in JIRA to **IN PROGRESS**.

2. Open your code editor and the repository project.

3. Open Git Bash and navigate to your main repository. Replace *path_directory* in the command with the path of your repository directory.

        cd path_directory

  > [Info] In the command line, **~** equals to your user directory, so instead of entering **cd C:/Users/Username**, you can just enter **cd ~**.

  The path of your repo as well as the git branch you are currently working on are displayed in Git Bash.


### Create a branch

The initial documentation is situated in the main branch. When working on a documentation task, you **never** work directly on this main branch, but you create a feature branch for each documentation task you are working on. A documentation task equals to a JIRA ticket and is therefore named like the corresponding JIRA ticket number.

When you start working on a new ticket, you have to create first a new branch for this ticket.

1. Enter the code below in Git Bash to switch from the main branch to the new created feature branch. Replace *feature_branch* in the command with the JIRA ticket number of your documentation task.

        git checkout -b feature_branch

    The new feature branch is displayed in Git Bash after the repo path.

2. Let the Git Bash terminal open and switch to you code editor to start working on the branch.

  > [Info] Note, that every change you are doing from now on will be tracked on the created branch.


### Insert changes to GitHub

To get the changes you made on your documentation to GitHub, you have to stage your changes first, commit your changes and finally push your changes. Sometimes, you can combine the staging and committing part.

1. Enter the code below in Git Bash to check if any changes have to be added or committed in your branch.

        git status

      All files to be staged as well as all files to be committed are displayed.

**Add your changes to Git**

It is necessary to track (untracked) files and changes in Git and stage them before you can commit them. You can either add a single file or add all files.

2. Enter the code below in Git Bash to track all files and changes that you made on your current branch in Git. If you want to add only a single file, replace *.* in the command with the file name.

        git add .

    All files are tracked in Git and can be committed.

    > [Info] The changes are not yet saved in Git!


**Commit your changes to Git**

All changes must be committed in Git before you can push them to Github. When committing changes, you have to include a commit message which contains of a title and a description. For documentation, the title of the commit message equals to the JIRA ticket number. The description should include some information about the changes done.

3. Enter the code below in Git Bash to save the changes on your current branch in Git. Replace *title* in the command with the corresponding JIRA ticket number and *description* with a information text about your changes.

        git commit -m "title" -m "description"

    All changes are saved in Git and can be pushed to GitHub.   


**Push your changes to GitHub**

To upload your changes to GitHub, you have to push them in Git. When pushing your changes, you have to indicate the location of your git repo as well as the branch you are pushing the changes to. You have to be authorized wth your GitHub account to be able to push changes to GitHub.

4. Enter the code below in Git Bash to push the changes on your current branch in Git to GitHub. Replace *feature_branch* in the command with the corresponding JIRA ticket number.

        git push origin feature_branch

    All changes are pushed to GitHub. You can open the repo in your browser and check for your changes.   


### Switch the branch

If you want to work on another task, you have to switch the branch. When the branch you want to work on, is not yet created, follow the instructions in the chapter [Create a branch](#create-a-branch). Sometimes, you are working on several existing branches. So you just have to switch the branch without creating a new one.

1. Enter the code below in Git Bash to display all existing branches in your repo.

        git branch

      All existing branches are displayed. The branch you are currently working on is highlighted.

2. Enter the code below to checkout from the current branch and switch to another branch. Replace *branch* in the command with the name of the branch you want to switch to (which is either the JIRA ticket number or *main*).

        git checkout branch

      The branch you switched to is displayed in Git Bash after the repo path.

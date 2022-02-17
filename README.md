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

4. Copy the code below and save the file as *.bash_profile* in your user directory (C:\Users\Username).  

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

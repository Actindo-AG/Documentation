# Main account and sandboxes

**Main account**

The main account is also called live or productive system. Each tenant has one main account that usually runs in productive mode. Each instance (main account or sandbox) has a specific host-prefix which determines how the main account/sandbox can be accessed:

- main account: https://[host-prefix].actindo.com

- sandbox: https://[host-prefix].dev.actindo.com

  > [Info] You can use the URL to identify if you are logged in to a sandbox or the main account. Additionally, the dropdown list in the upper right corner of the *Actindo Core1 Platform* displays the instance on which you are currently working.

   ![Sandbox URL](../../Assets/Screenshots/Core1Platform/AdministratingCore1/SandboxURL.png "[Sandbox URL]")

Licenses, vCores, and available storage are bound to the main account and must be shared with all sandboxes.   

The main account and each sandbox have their own separated databases. This means, that you cannot synchronize databases between the main account and the sandbox.

**Sandboxes**  

Sandboxes have the following characteristics:  
- You can create a sandbox as a copy of the main account with all data that is currently available in the main account. After this, however, the sandbox and the main account is not synchronized.

- You can install pre-release plugins in case you have access to the source code. On a main account, you can install released versions only.

- Each sandbox has an owning user. As an owning user, you can access the file system of the sandbox via SSH, if your user has been marked as a developer account by Actindo:   
  ssh username@login.dev.actindo.com   
  cd ~/sandboxes/[host-prefix]

- The owner of a sandbox must have access to the owning main account but does not need to own the main account.

- vCores, which are a measure for parallel computing performance, and storage are to be assigned to a sandbox. The assigned vCores and storage get subtracted from the budget of the main account.   
  This means, if you expect a lot of processes and database entries in a sandbox, you have to consider that this computing power is to be shared with the main account.   
  The same is valid for licenses, so that you have to sum up all licenses for which you assign rights in the main account and in a sandbox.

**Overview**   

The following overview shows the main differences between a main account and a sandbox:
Topic | Main account | Sandbox   
--- | --- | ---
**URL** | [host-prefix].actindo.com | [host-prefix].dev.actindo.com    
**Licenses** |owned by account | shared with main account  
**Custom code** | NO | YES   
**Unreleased plugins** |NO | YES   
**User creation** | YES |NO 
**Direct DB access** | NO | YES   
**Own database**| YES| YES
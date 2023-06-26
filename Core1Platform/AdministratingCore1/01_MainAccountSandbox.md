# Main account and sandboxes

Each tenant has one live-system. This is also called a main account. Licenses, vCores and available storage are bound to the live system and have to be shared with all sandboxes. Each live-account or sandbox has a specific host-prefix which determines how the account/sandbox can be accessed:

- live-account: https://[host-prefix].actindo.com

- sandbox: https://[host-prefix].dev.actindo.com

Note, you can determine from the URL if you are logged in a sandbox or the main account.   
![Sandbox URL](../../Assets/Screenshots/Core1Platform/AdministratingCore1/SandboxURL.png "[Sandbox URL]")

Each sandbox and main account has its own separated database. This means, that you cannot share data between the main account and the sandbox.

**Sandboxes**
Each sandbox has an owning user. As an owning user, you can access the file system of the sandbox via SSH:

ssh username@login.dev.actindo.com
cd ~/sandboxes/[host-prefix]

The owner of a sandbox must have access to the owning main account, but does not need to be owned by the main account.

vCores and storage are to be assigned to a sandbox. The assigned vCores and storage get subtracted from the budget of the main account. This means, if you expect a lot of processes and database entries in a sandbox, you have to consider, that this performance is to be shared with the main account.   
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
**Own database**| YES| yes
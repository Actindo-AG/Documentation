# Main account and Sandboxes

Each tenant has one live-system. This is also called a main account. Licenses, vCores and available storage are bound to the live system and have to be shared with all sandboxes. Each live-account or sandbox has a specific host-prefix which determines how the account/sandbox can be accessed:

- live-account: https://[host-prefix].actindo.com

- sandbox: https://[host-prefix].dev.actindo.com

Note, you can determine from the URL if you are logged in a sandbox or the main account.   
![Sandbox URL](../../Assets/Screenshots/Core1Platform/AdministratingCore1/SandboxURL.png "[Sandbox URL]")

Each sandbox and main account has its own separated database. This means, that data cannot be shared between the main account and the sandboxes.



Topic | Main account | Sandbox   
--- | --- | ---
**URL** | [host-prefix].actindo.com | [host-prefix].dev.actindo.com    
**Licenses** |owned by account | shared with main account  
**Custom code** | NO | YES   
**Unreleased plugins** |NO | YES   
**User creation** | YES |NO 
**Direct DB access** | NO | YES   
**Own database**| YES| yes
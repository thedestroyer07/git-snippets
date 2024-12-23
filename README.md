### Git command

---

#### Setting-up ssh

Just enter all the command on your terminal

```
> ssh-keygen -t ed25519 -C "your_email@example.com"

dont enter password if you dont like

> eval "$(ssh-agent -s)"

> cat ~/.ssh/id_ed25519.pub

copy the contents and paste it to github
when you addig new ssh key

to test enter the command:
   > ssh -T git@github.com

```
---

**Encounter error**  

*   this is the case when, newly created repo on github and    
    if your not downloading the repo and you make git init on your local pc  
    and uploading it to your git repository emidiately using command line

**This is the command to set the repo origin if you encounter error**

```
to make it main not master branch:
    git branch -M main

use ssh to upload:
    git remote add origin git@github.com:thedestroyer07/sampleRepo.git

    git remote set-url origin git@github.com:thedestroyer07/sampleRepo.git
```

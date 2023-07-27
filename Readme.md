# Git & Github - The Full Cource

A fact-paced cource for getting upto speed with Git and Github.

## To commit and add at once
use ``` git commit -a -m "my Comments" ```

<br/>OR<br/>

use ```git commit -am "my Comments" ```

## To show the list of urls
use ```git remote -v```

## For details
use ``` git remote show origin ```

## To pull and push at once
use ``` git push origin master -u ```

## To fetch all the data from origin
use ``` git fetch ```  
* but then we have to manually merge

  * instead

    use ``` git merge origin /master```

> **__To Combine Both__** <br/>
use ```git pull orign BranchNameHere```

***

# To Create a Clone into new Folder
use ``` git clone repo url folderNameHere ```

## To see all the changes in repo

use ``` git log ```

***

# SoMeThiNg ExtrAA

To use an online VS code  >>
* Go inside repo
* Press ```"."```
  * it will open up an online editor 😉, ENjoY
      * side Note: For Termainal we need codeSpace (Pay/Sec)

***

# Branches

To See Current Branch / Branches

use ```git branch```

## To Rename a Branch

use  ```git branch -M yourRenameBranchName```

## Create our Custom Feature Branch

use ```git branch BranchToBeCreated```

## To Delete a Branch

use  ```git brannch -d BranchToDelete```
* this command deletes the branch carefully, and if it has been merged to master

### Alternatively we can
use ``` git branch D BranchToDelete```
* even though things are not merged

## To Switch New Barnch
use ```git checkout TheBranchNameToSwitch```

### Note:
* If we are making any changes while we are in other branch, those won't be visibe in Mater (until merged and is commite in the Other Branch)

### Some Cool Technique

> **__If You Wana Create and Checkout to a New Branch at the same time__**<br/>
use ```git checkout -b myNewCoolBranch``` (similar to git pull)

***

> **__To Switch to Previous Branch__** <br/>
use ```git checkout -```

## Merge Conflict
we can megre the coflict manually using editor OR <br/>

use ```git merge --abort``` to go back to Original State

> Post that make sure you add and commit your changes

# GitHUB
***
<button>
<svg aria-hidden="true" height="12" viewBox="0 0 16 16" version="1.1" width="12" data-view-component="true">
    <path d="M5 5.372v.878c0 .414.336.75.75.75h4.5a.75.75 0 0 0 .75-.75v-.878a2.25 2.25 0 1 1 1.5 0v.878a2.25 2.25 0 0 1-2.25 2.25h-1.5v2.128a2.251 2.251 0 1 1-1.5 0V8.5h-1.5A2.25 2.25 0 0 1 3.5 6.25v-.878a2.25 2.25 0 1 1 1.5 0ZM5 3.25a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Zm6.75.75a.75.75 0 1 0 0-1.5.75.75 0 0 0 0 1.5Zm-3 8.75a.75.75 0 1 0-1.5 0 .75.75 0 0 0 1.5 0Z"></path>
</svg>
Fork
</button>

***
When we fork a repo, it will be copied to our __Own Github Account__, the Fork maintains a linke to the original repo, i.e., __we can pull in future chnages when needed__.

## Step 1 :
> * Create a New Branch ```git branch myBranch```
> * Checkout to newbranch created  ```git checkout myBranch```
### OR (Single Command)
***
> Create and CheckOut @ once
> ``` git checkout -b myBranch```

## Step 2 :
Make te necessary changes and Push them back to Github
> ```git add .```<br>
> ``` git commit -m 'my New Changes'```<br>
> ```git push origin myBranch```

## Step 3 :
Go to Repo in Github
Click the Button that says <button>Comapre and pull Request</button> and Create a __Pull Request__.

## <i>Pro Tip**</i>
When working with a fork Locally, we can __keep it in Sync with the Original by adding a remote link to the upstream repo__.
> ```git remote add upstream https://github.com/src-github-ac/repo.git```

Now if any changes in Original Repo,
> we can ``` git fetch ``` to download the changes

and then
> ``` git rebase upstream/master ```<br>
to add those changes on top of our current changes.
***
***

# RESET
Once we have added a file for Commit, the file gets into stagging area and it ready to be pushed after a commit to Github.

## we can unstage the file withoit modifying ir deleting it by running

> ``` git  reset fileNameHere```<br>
OR<br>
> ``` git reset``` to remove all from stagging

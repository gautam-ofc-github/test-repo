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
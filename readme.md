GIT
====

# Multiple people works in same repository so we create a user name and password for the particular user

Create User Name:   git config --global user.name 'dhanesh'
Create User Email:  git config --global user.name 'dhaneshprabu2705@gmail.com'
TO check Name :  	git config user.name
TO Check Email :  	git config user.email



# Then we need to tell one git Repo present in this folder and set the main branch(default branch)

Set Default branch:  git config --global init.defaultBranch main  (here main is just a name of main branch)
Check             :  git init   (to check repository create or not)



# Then create some random file like index.html, readme.md, index.js

check the status of git file:  git Status
TO Add file in git 			:  git add readme.md  (Now this file added to git to get Track)
TO Commit in git(Store)		:  git commit -m 'readme' (readme-- this is just a message for th commit)
Git log command				:  git log
Exit for log File			:  wq
TO add all the files        :  git add .    (Not add single file like readme.md Add all the files in git)
TO commit all files         :  git commit -m 'JustMessage'  -- Same as before commit



# Checkout 
TO Check the previous verion of file :  git checkout 'hassh value of commit'
Come back to orginal version		 :  git checkout main
Without change come to main 		 :  git checkout -f main (Force checkout)




# then Sign In to hit hub using google account in github.com
# Create repository in git hub in this put any repository name  and Submit
TO Connect Local git to remote git Hub :  git remote add origin https://github.com/DhaneshPrabu/GIT-PROJECT.git
TO Create Main in Git Hub              :  git branch -M main
TO Push all Local git File to git Hub  :  git push -u origin main (It redirect to authrization Screen finish 
                                            authorization)




# now add muliple sub branch to the main branch
TO Create branch            :  git branch 'bug' (bug is the branch name)
TO checkout the branch      :  git checkout bug (switch to bug branch)

TO create and checkout both :  git checkout -b 'feature' (It will create a feature branch inside the bug branch
                                    bcz we are in bug branch inside bug branch we create a another checkout branch so inside the bug branch feature branch is presentk)

TO create branch from specefic Branch:   git checkout -b feature2 bug (bug is exiting branch in that bug branch
                                            we create a new branch as a feature2 branch)



# -------------- This is a Bug Branch which contains both feature and feature-2 beanch ----------------


TO See the list of local branch         :  git branch
To see all branch include remote branch :  git branch -a

# To push the this branch to remote repository like gitHub
Push particular branch to git hub : git push --set-upstream origin bug (bug is a branch name)
Simple Command to push branch     : git push -u orgin feature
Push branch                       : git push (Only the first time it need the full command like 
                                        --git push -u orgin feature once it done --git push this command is enough to push to the remote repo when the commit complete)




# Merge sub branch to main Branch

Merge the sub branch to main branch                            :  git merge(not recommended)
when we create branch in remote repo fetch to git local        :  git fetch
fecth and merge in local when we create branch in remote repo  :  git pull (used for both fetch and merge)


# While conflict is occurs when we merge the sub branch to main branch
Objective :-
    - 1st we need to merge the main branch to sub branch (main -> subBranch Flow like this main to subBranch 
            bcz sub branch not cotain the main branch details so we merge the main branch to sub branch)
    -we need to check our  local repository have the updated main so checkout to main and (-- git pull ) to
             fetch and merge the github main to local git main.Now we got the updated main.
    - the checkout to sub branch main use ( -- git merge main ) to merge the local main branch to local sub
             branch 
    - Now it show options like -- (>>> main (Incoming change) )(main branch change come to sub branch)
                               -- (<<< HEAD (Current Change) )(sub branch go to main branch)
                               -- accept both change (merge the sub branch change (have both main and sub 
                                        branch change))
                               -- Compare changes 
    -  -- click (resolve in mere editor) now it shows compare screen and we can edit the Result screen for the 
                final change.

    - click complete merge then click complete with confilcts
    - git add . (add this modified to git local)
    - git commit -m 'redme conflict merge'
    - git push
    - new pull Request(PR) (need to Complete the PR steps)
    - after complete the PR (pull request)  -- git pull for the main branch to update the github main branch 
            to the git local main branch

    
    





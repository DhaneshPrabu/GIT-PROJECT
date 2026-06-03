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











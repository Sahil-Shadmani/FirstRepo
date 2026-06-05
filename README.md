# FirstRepo
Git-- it is a version control System that has tools that helps us to track changes in our code basically when we do some changes or when we add some sort of new file so it will keep track of it and helps to collaborate with others. Git ko hame install krna padta he apne pc pr.
<br><br>
GitHub-- it is a website that allows us to store and manage their code using git and we can upload our whole code to github and we can share our github link in resume also, we upload in folders and we can called it repository and we also see others code and copy it and also change them.
<br><br>
Configuring Git
<br><br>
There are two types of configuration one is global which means we can change with one global account and it is one time and we dont need to setup again and again it is reffered to our whole account and local means we can change with multiple different emails or accounts like working in a team.
<br><br>
git config --global user.name "username of git hub"
<br><br>
git config --global user.email "email of git hub"
<br><br>
git config --list  (iska matlab apn check kr sakte he apnne kya setup kiya git config se) if this doesnot work we can use (git config --global user.name) (git config --global user.email) this commands to check username and email
<br><br>
SOME GIT COMMANDS
<br><br>
CLONE-- it is used to copy github repository into our local machine like pc,laptop the syntax is git clone <link>
<br><br>
cd-- it is used to change the directory like we can switch between folders and the syntax is cd foldername
<br><br>
ls-- it will list all the files in that particular folder in which we 
<br><br>
pwd-- it will give us the current directory in which we are basically give full path
<br><br>
For listing all hidden files we will use (ls -a) command if we are not in powershell or we can use (dir -Force) or (Get-ChildItem -Force)
<br><br>
STATUS-- it will display the status of the code using (git status) command
<br><br>
there are four types of status in git when we use git status command
<br><br>
1. Untracked-- it means when we add new file and even we have made changes in it it doesn't show M and git doesnot have track of it ,it shows U
2. Modified-- it means we have done some changes to the existing file which is present in the github ,it shows M
3. Unmodified-- it means the file is unchanged
4. Staged-- when we change anyrhing in the file or add new file and when we add these changes so it status is staged means they are ready to commit 
<br><br>
THis is testing new line
<br><br>
ADD-- it is used save changes that we made to our files in the folder and make them staged so that they are ready to commit or we can say that (adds new or changed files in your working directory to the Git staging area) using (git add filename) or if we want to add all the files to the staging area we can use (git add .) and when we add new file to the folder and then we add that file to staging area so it will show A

<br><br>
Commit-- it is used to save the changes to your local computer it doesnot affect github repository we have to push it then it will apply those changes to the github this will save the changes that we had made in our pc basically it will take us ahead of one commit,  using (git commit -m "message about what change")

<br><br>
Pull-- it is used for when we to import changes from the github and then all the new changes will come here and we have to accept it using above given options and then save it and push to the github
<br><br>
Push-- it is used to push the local repo to the remote repo basically after the commiting the repo we will push it to the github so that it will reflect changes in the github that we had made in the code editor using (git push origin main) in which origin is the nickname of our repo and main is the branch name it could be any and if we had made or write one time this command then again we dont need to type origin main because git already knows it so only write git push or pull 2nd time
<br><br>
(git push --force origin nameofbranch)-- it forces github to match the local repo
<br><br>
if you want to go out of the directory you must type cd ..
<br><br>
If you want to make new directory in exsisting folder basically creating new folder inside that folder we must use (mkdir nameofolder) to make new folder/directory or we can create directly in vs code their are options
<br><br>
git init-- it is used to make any directory a git repository by going to that folder and using git init command it will now react as a git repository but now we have to push it to git in a new repository so we will go to github and create new repo and then we will use next command which is 
<br><br>
git remote add origin <link>-- we have to copy that new repo link and run this command so that our code will be added to this new repo and then we need to push it
<br><br>
git remote -v-- it is used to verify remote repo that which file we have pushed to it 
<br><br>
git branch-- it is used to check in which branch are we now and also show all the branches
<br><br>
(git branch nameofnewbranch)-- it will only create new branch
<br><br>
git branch -M newname-- it is used to change the name of the branch or rename it but we have to be present in that branch so that its name would be changed
<br><br>
git push -u origin main-- it means we will create a shortcut so that we use only git push from next time we will give this command when we are working for a long time in the same project and pushes in the same repo than only we use this command so that git remember it -u stand for upstream
<br><br>
Branch Commands-- we can create another branch here and checkout to that branch and if we change any sort of code in any file it doesnt affect out main code it will only change in that branch in which we are changing the code and then if we want to reflect that changes in the github then we run push command on that branch name not on main
<br><br>
1. git checkout -b newbranchname-- it is used to create new branch so that individual developer can work on their module and it will be automatically switched to the new branch that we have created using this command
<br><br>
2. git checkout branchname-- it is used to switch between branches by giving thier name
<br><br>
3. git branch -d nameofbranch-- it is used to delete the branch that we want to and make sure that we cant delete the branch in which we are currently now so we need to switch to another branch 
<br><br>
Merging code commands-- it is used to merge the feature or another branch to the main or other branch that we want to
<br><br>
1. git diff <-branch name->-- it is used to compare the differences between two branches,files,commits and more we have to give branch name of that branch that we want to compare with the branch in which we are standing or currently now
<br><br>
git diff-- it will show all the current unstaged changes means which are not added
<br><br>
(git diff --staged)-- it will give all the changes that are added or basically they are ready to commit
<br><br>
git diff nameofbranch1 nameofbranch2-- it means difference between two branches
<br><br>
git diff commit1 commit2-- it means differnce between two commits that we had made
<br><br>
There are two ways to merge two branches
<br><br>
1. using PR(pull request) in github-- pull request means that we are trying to push our branch into main and we create our pull request and send to our senior developer so now its upto his hands that he will accept or reject our request of merging in the main branch and give comments that what is mistake and what is merged
<br><br>
for using this we need to push our code into the github then there will be a button of compare and pull request now to accept the pr we will click on compare and pull request and then give comment if we want and then click on create pull request then github will check if there is any conflict between both branches or not and then we click on merge pull request and then click on confirm merge and then finally our branch is merged and then we need to pull it in our local repo (basically in vs code)
<br>
conflict means that we have written same code in the same line or changes it in the branch in comparision to the main branch
<br><br>
Resolving Merge Conflicts-- it is an event when git is unable to understand which change it should keep when there is a conflict
<br><br>
2. git merge nameofanotherbranch-- when we change in both branches at the same line and then we run this command it will give conflict and we have to handle it manually because vs code gives us many options what to keep and what to not keep and then we will save and push (and we can also merge these changes in another branch by using this command)
<br><br>
git cherry-pick hashcodeofCommit-- it is used when we want one commit of that branch into another branch so instead of merging whole branch into that branch we will take hash code of that commit and go to that branch and run this command so it will create a copy of that commit and paste to this branch in which we ran this command and make the changes that we had made in that commit it may arise conflict if there is no same line of code available (basically it is helpful for fixing a bug in another file and then run this command in main file)
<br><br>
Undoing changes-- it means to undo change that we had made in our local repo we can revert it using commands
<br><br>
1. staged changes-- it means those changes that are added but not committed so we can revert added changes using (git reset filename) or we can use (git reset) for all the changes in all the files that we had made to revert
<br><br>
2. commited changes-- it means when we added and committed those changes and afterward then we want to undo that changes then we will be using (git reset HEAD~1) this means that when we commit git saves all the commit and head is the latest commit that we had made and 1 is the step how many commits we want to go back
<br><br>
(git reset <-hashcode->)-- Now if we want to go multiple commits behind we will use this command by giving hash code and that will move our Latest HEAD~ to that commit
<br><br>
Now there are multiple types of reset which are
<br><br>
1. (git reset --soft hashcode)-- result will be commits removed and changes are kept in staging area
<br><br>
2. (git reset hashcode)-- result will be commits removed and changes kept in file but not staged
<br><br>
3. (git reset --hard hashcode)-- result will be commits removed changes removed and files will be restored this is dangerous because changes are lost
<br><br>
4. git revert hashcodeofthatcommit-- it means when we use this command we are moving branch ahead of that commit and that commit that we want is gone but is saved but in reset we will move our branch backward and history is deleted but in this history is not deleted but is saved in another commit and we can also move back to that deleted commit(changes) 
<br><br>
git log-- it is used to check all the commits that we had made on the branch we are standing now the first commit will be the latest commit that we had made reading from sky
<br><br>
(git log --all)-- it is used to show all the commits of all the branches or we can use (git log --online --graph --all) command
<br><br>
(git log --oneline)-- it will give one line per commit
<br><br>
(git show hash)-- it will give the details of the commit
<br><br>
git restore filename-- it is used to get back all the lines that we have added or removed and then we used this undo commands so this commands will revert back those lines from staging area and to get back we will use this command
<br><br>
(git restore --staged filename)-- it is used to move back changes from staging area(when we add) to unstaging area(working directory) it is used when we want to commit other files but not one specific file so we use this command same as (git reset) command
<br><br>
git reflog-- it will recover all the commits that we had deleted using reset hard command and move back our head to that where it was earlier before deleting and it is also useful in recovering lost or deleted branches
<br><br>
Stash commands-- stash commands are used to save temporarily work and brings them back when we need it
<br><br>
1. git stash-- it is used to save our work when we have to do some other work and it hides all the changes that we had made we will now discuss some another versions of this command
<br><br>
a. git stash push-- same as git stash
<br><br>
b. (git stash push -m "message")-- it is used to save the work with message so that we can identify easily and this message will be shown on stash list command when we use it
<br><br>
c. git stash push filename-- it means that we can stash only one file among all the modified files
<br><br>
d. (git stash push -u) or (git stash push --include-untracted)-- it is used to save untracked files also
<br><br>
2. git stash pop-- this command will bring the unfinished work that is hidden back when we use this command
<br><br>
3. git stash list-- it means when we create multiple stashes and we want to view it we can use this command
<br><br>
4. git stash apply-- it is used to keep the stash in the list and also bring back our work and save the stash
<br><br>
5. git stash drop hashcode-- it is used to delete the stash using hashcode that is present in the stash list
or we if want to delete all the stashes we will use git stash clear
<br><br>
Fork-- it is used to copy others code,files,repos into our github and we can do this by going to their repo and their is a option called fork we will fork it into our account and we can contribute to their projects by making any useful changes in their code and then pull request to them so that they can see and accept


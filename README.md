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
git config --list  (iska matlab apn check kr sakte he apnne kya setup kiya git config se)
<br><br>
SOME GIT COMMANDS
<br><br>
CLONE-- it is used to copy github repository into our local machine like pc,laptop the syntax is git clone <link>
<br><br>
cd-- it is used to change the directory like we can switch between folders and the syntax is cd foldername
<br><br>
ls-- it will list all the files in that particular folder in which we are
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
git branch -M newname-- it is used to change the name of the branch or rename it but we have to be present in that branch so that its name would be changed
<br><br>
git push -u origin main-- it means we will create a shortcut so that we use only git push from next time we will give this command when we are working for a long time in the same project and pushes in the same repo than only we use this command so that git remember it -u stand for upstream 


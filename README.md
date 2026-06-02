# FirstRepo
Git-- it is a version control System that has tools that helps us to track changes in our code basically when we do some changes or when we add some sort of new file so it will keep track of it and helps to collaborate with others. Git ko hame install krna padta he apne pc pr.
<br>
GitHub-- it is a website that allows us to store and manage their code using git and we can upload our whole code to github and we can share our github link in resume also, we upload in folders and we can called it repository and we also see others code and copy it and also change them.
<br>
Configuring Git
<br>
There are two types of configuration one is global which means we can change with one global account and it is one time and we dont need to setup again and again it is reffered to our whole account and local means we can change with multiple different emails or accounts like working in a team.
<br>
git config --global user.name "username of git hub"
<br>
git config --global user.email "email of git hub"
<br>
git config --list  (iska matlab apn check kr sakte he apnne kya setup kiya git config se)
<br>
SOME GIT COMMANDS
<br>
CLONE-- it is used to copy github repository into our local machine like pc,laptop the syntax is git clone <link>
<br>
cd-- it is used to change the directory like we can switch between folders and the syntax is cd foldername
<br>
ls-- it will list all the files in that particular folder in which we are
<br>
For listing all hidden files we will use (ls -a) command if we are not in powershell or we can use (dir -Force) or (Get-ChildItem -Force)
<br>
STATUS-- it will display the status of the code using (git status) command
<br>
there are four types of status in git when we use git status command
<br>
1. Untracked-- it means when we add new file and even we have made changes in it it doesn't show M and git doesnot have track of it ,it shows U
2. Modified-- it means we have done some changes to the existing file which is present in the github ,it shows M
3. Unmodified-- it means the file is unchanged
4. Staged-- when we change anyrhing in the file or add new file and when we add these changes so it status is staged means they are ready to commit
<br>
ADD-- it is used save changes that we made to our files in the folder and make them staged so that they are ready to commit or we can say that (adds new or changed files in your working directory to the Git staging area) using (git add filename) or if we want to add all the files to the staging area we can use (git add .)

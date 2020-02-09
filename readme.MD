# This repo is just to learn git commands - master

## get code to local 

1. cd directory-name-here (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)

(All branches will be pulled to local and the default branch will be set to, usually master.)

## get code to local and set a specific branch to default.

1. cd directory-name-here (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone -b branch-name git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)

## merge two branches in local when there are no conflicts

1. git checkout master  ( set the current branch to master -in this case merging to master)
2. git merge branch-name

## overwite old_branch with code in new_branch

1. git checkout new_branch
2. git merge -s ours old_branch
3. git checkout old_branch
4. git merge new_branch




## Once repo is created in  github, Use the below commands upload a code into that repository:

1. echo "# arjun-test01" >> README.md  
2. git init  
3. git add README.md  
4. git commit -m "first commit"  
5. git remote add origin git@github.com:acsekhar2000/arjun-test01.git  
6. git push -u origin master 

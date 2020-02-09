# This repo is just to learn git commands - dev
## when repo already exists - get the code to local.

1. cd <directory-name-here> (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)

(The default branch, usually master, will be pulled from git hub as no branch is specified)

## when repo already exists - get the specific branch code to local.

1. cd directory-name-here (navigate to the directory where you want the code to be copied. The below command will create a directory)
2. git clone -b <branch-name> git@github.com:acsekhar2000/learn-git-commands.git
3. cd learn-git-commands ( and use ls to see the code that is down loaded)




## Once repo is created in  github, Use the below commands upload a code into that repository:

1. echo "# arjun-test01" >> README.md  
2. git init  
3. git add README.md  
4. git commit -m "first commit"  
5. git remote add origin git@github.com:acsekhar2000/arjun-test01.git  
6. git push -u origin master 
